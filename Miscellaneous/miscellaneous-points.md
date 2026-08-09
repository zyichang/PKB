---
quizify:
  format: 1
  deck: Miscellaneous
  tags: [Miscellaneous]
---

+++
<!-- quizify-card
tags: [集成电路, 就业方向, added::2026-08-06]
-->

#### 1. 集成电路（IC）研究生有哪些就业方向？

***

按芯片产业链的环节划分，主要方向有：

1. **芯片设计（IC Design）** —— 数字 / 模拟 / 射频 / 数字后端，最主流的方向。
2. **验证（Verification / DV）** —— 用 SystemVerilog + UVM 验证设计正确性。
3. **制造与工艺（Fabrication & Process）** —— 工艺、器件工程师，就职于晶圆厂（中芯国际、TSMC）。
4. **封装与测试（Packaging & Testing）** —— 封装工程师、测试 / ATE 工程师。
5. **EDA 工具** —— 在 Synopsys、Cadence、华大九天等做工具研发。
6. **应用与系统** —— FAE（现场应用工程师）、系统 / 嵌入式 / 硬件工程师。
7. **科研与学术** —— 读博后进高校或研究所（如中科院微电子所）。
8. **其他** —— 产品经理、技术销售、国企 / 央企、公务员。

> [!TIP]
> 数字设计/验证岗位多、门槛相对友好；模拟/射频稀缺且薪资高；工艺/制造偏物理与产线。

+++
<!-- quizify-card
tags: [集成电路, 就业方向, 芯片设计, added::2026-08-06]
-->

#### 2. 芯片设计（IC Design）主要分为哪几类？

***

- **数字 IC 设计**：用 Verilog/VHDL 做 RTL，属**前端**逻辑设计。
- **模拟 IC 设计**：放大器、电源管理、ADC/DAC，难精通、薪资高。
- **射频 / 混合信号**：无线收发、通信。
- **数字后端 / 版图（Backend / layout）**：布局布线（place & route）、时序收敛。

+++
<!-- quizify-card
tags: [zsh, autosuggestions, shell, added::2026-08-08]
-->

#### 3. zsh-autosuggestions 的 `history` 和 `completion` 两种策略有什么区别？

***

`ZSH_AUTOSUGGEST_STRATEGY` 决定灰色建议从哪里来：

- **`history`**：从**命令历史**里补全——只建议“我以前真正敲过的命令”。
- **`completion`**：用**补全引擎**建议——只建议“系统里真实存在的命令”，即使我从没敲过。

```zsh
ZSH_AUTOSUGGEST_STRATEGY=history
```

> [!TIP]
> 想让它记住并复现自己敲过的命令，用 `history`；想让它提示合法可用命令，用 `completion`。

+++
<!-- quizify-card
tags: [zsh, history, hook, added::2026-08-08]
-->

#### 4. 怎样让 zsh **不记住失败的命令**（这样自动建议就不会提示错误命令）？

***

用两个 hook：先**推迟保存**每条命令，等它执行完，只有**退出码为 0（成功）**才写入历史。

```zsh
autoload -Uz add-zsh-hook

_record_last_command() {
  _LAST_CMD="${1%$'\n'}"
  return 1   # 先别存，交给 precmd 根据退出码决定
}
add-zsh-hook zshaddhistory _record_last_command

_save_if_success() {
  local ret=$?
  if [[ -n "$_LAST_CMD" && $ret -eq 0 ]]; then
    print -sr -- "$_LAST_CMD"
  fi
  _LAST_CMD=
}
add-zsh-hook precmd _save_if_success
```

- `zshaddhistory` 在命令执行**前**触发，返回非零即“暂不保存”。
- `precmd` 在下一个提示符前触发，此时 `$?` 是上一条命令的退出码；成功才用 `print -sr` 补写进历史。
- 效果：`command not found`（退出码 127）、`false`（退出码 1）等失败命令都不会进历史。

+++
<!-- quizify-card
tags: [zsh, history, oh-my-zsh, added::2026-08-08]
-->

#### 5. zsh 的命令历史保存在哪里？

***

默认在 `~/.zsh_history`。这个路径不是我自己设的，而是 Oh My Zsh 的 `~/.oh-my-zsh/lib/history.zsh` 设的：

```zsh
[ -z "$HISTFILE" ] && HISTFILE="$HOME/.zsh_history"
```

查看方式：`history`（当前会话）、`history 1`（全部）、`cat ~/.zsh_history`（原始文件，带 `: 时间戳:0;` 前缀）。

+++
<!-- quizify-card
tags: [oh-my-zsh, zsh, framework, added::2026-08-08]
-->

#### 6. Oh My Zsh 是怎么工作的？如果删掉 `~/.oh-my-zsh` 文件夹会怎样？

***

Oh My Zsh 不是 shell 本身，而是**架在 zsh 之上的配置框架**。真正的 shell 是 `/usr/bin/zsh`。启动链：

1. 启动 zsh → 读 `~/.zshrc`；
2. `~/.zshrc` 里 `export ZSH="$HOME/.oh-my-zsh"` 再 `source $ZSH/oh-my-zsh.sh`；
3. `oh-my-zsh.sh` 加载**主题**、`lib/` 库文件（如 `history.zsh`）、以及 `plugins=(...)` 里的**插件**；
4. 插件实际存放在 `~/.oh-my-zsh/custom/plugins/`（如 `zsh-autosuggestions`）。

**删掉 `~/.oh-my-zsh` 后**：zsh 本身仍能启动（`/usr/bin/zsh` 是独立程序），但 Oh My Zsh 全部失效——`source` 报错、主题丢失、**插件失效（自动建议、语法高亮都没了）**、库设置丢失。`~/.zshrc` 里自己写的 alias、代理块、历史 hook 仍有效。想干净卸载用 `uninstall_oh_my_zsh`，别直接 `rm -rf`。

+++
<!-- quizify-card
tags: [linux, filesystem, usr-merge, added::2026-08-08]
-->

#### 7. 为什么系统里有 `/usr/bin/zsh` 和 `/bin/zsh` 两个路径？它们一样吗？

***

**完全一样**——是同一个文件的两条路径。因为 `/bin` 是指向 `usr/bin` 的**软链接**：

```
/bin -> usr/bin
```

两条路径的 **inode 号相同**（同一磁盘文件，不是副本）。这叫 **/usr merge（/usr 合并）**：历史上 `/bin`（开机必需）和 `/usr/bin`（其余）分开，现代发行版（Fedora、Arch、Debian…）把所有二进制统一放进 `/usr/bin`，`/bin` 保留为软链接以兼容硬编码 `/bin/sh` 等的旧脚本。

> [!TIP]
> 平时直接敲 `zsh` 即可，`PATH` 会解析到 `/usr/bin/zsh`；全路径只在 shebang（`#!/bin/zsh`）或 `/etc/shells` 里才需要。

+++
<!-- quizify-card
tags: [linux, elf, dynamic-linking, added::2026-08-08]
-->

#### 8. 那个约 953K 的 zsh 文件就是 zsh 软件的全部吗？

***

不是占位符，它是**真正的可执行程序**（`file` 显示为 `ELF 64-bit ... dynamically linked, stripped`），但只是 zsh 的**核心**。zsh 是**模块化**的，核心之外还按需加载：

- `/usr/lib64/zsh`（约 1.4M）——编译好的**模块**（`.so` 机器码）。
- `/usr/share/zsh`（约 8.5M）——**架构无关**的 shell 脚本（补全、函数库，如 `add-zsh-hook`）。

所以完整安装约 11M，启动的二进制只是 953K 的核心。`dynamically linked` 说明它运行时还依赖系统共享库（如 `libc.so`）。类比：953K 是“引擎”，运行时再从“车库”取模块和脚本，而不是把所有零件都塞进一个文件。

> [!NOTE]
> Windows 的对应关系：核心 `.exe` ↔ `/usr/bin/zsh`；可加载库 `.dll` ↔ `/usr/lib64/zsh` 的 `.so`；数据/脚本 ↔ `/usr/share/zsh`。静态链接的程序能独立运行，动态链接的则依赖外部库。
