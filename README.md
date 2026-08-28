# Qwen CTF 技能包

面向 Qwen Agent 的 CTF 技能分享包，包含 Crypto、Misc/取证、PWN、Web/逆向审计以及统一的 CTF 分诊路由技能。

## 技能包

当前仓库同时提供可直接浏览/安装的标准 skills 目录，以及便于分发的 ZIP 压缩包。

### 标准 skills 目录

| 目录 | 内容 |
| --- | --- |
| [`skills/ctf-router`](skills/ctf-router) | 新题目分诊，并路由到专项技能 |
| [`skills/ctf-crypto-solver`](skills/ctf-crypto-solver) | RSA/ECC、格、PRNG、古典密码等密码学题型 |
| [`skills/ctf-misc-forensics`](skills/ctf-misc-forensics) | Misc、磁盘/内存/网络取证、隐写、编码等 |
| [`skills/ctf-pwn-exploit`](skills/ctf-pwn-exploit) | 栈/堆利用、ROP、格式化字符串、内核与沙箱等 |
| [`skills/ctf-web-reverse-audit`](skills/ctf-web-reverse-audit) | Web 安全、源码审计与逆向分析 |

每个目录都包含顶层 `SKILL.md`，可按 Qwen Agent 的 skills 目录结构直接复制。

### ZIP 分发包

| 文件 | 内容 |
| --- | --- |
| `CTF技能包-CTF-Crypto解题.zip` | 密码学题型、RSA/ECC、格、PRNG、古典密码等 |
| `CTF技能包-CTF-Misc取证.zip` | Misc、磁盘/内存/网络取证、隐写、编码等 |
| `CTF技能包-CTF-PWN利用.zip` | 栈/堆利用、ROP、格式化字符串、内核与沙箱等 |
| `CTF技能包-CTF-Web逆向审计.zip` | Web 安全与逆向分析、认证、注入、反分析等 |
| `CTF技能包-CTF分诊路由.zip` | 根据题目类型选择和分发到对应技能的路由器 |

每个压缩包都包含一个顶层 `SKILL.md`；需要时可将其解压到 Qwen Agent 的 skills 目录中使用。

## 使用

建议先使用 `skills/ctf-router` 对题目分诊，再进入对应专项 skill。Windows 用户可按 skill 中的说明通过 WSL 使用 Linux 专属工具。

## skills.sh

本仓库的标准 `skills/` 目录可直接通过 skills.sh 分发，支持 Claude Code、Cursor、Codex、GitHub Copilot、Windsurf、Gemini CLI、OpenClaw 等 agent。

```bash
npx skills add yxy050208/qwen-ctf-skills
```

单个 skill 页面：

- [ctf-router](https://skills.sh/yxy050208/qwen-ctf-skills/ctf-router)
- [ctf-crypto-solver](https://skills.sh/yxy050208/qwen-ctf-skills/ctf-crypto-solver)
- [ctf-misc-forensics](https://skills.sh/yxy050208/qwen-ctf-skills/ctf-misc-forensics)
- [ctf-pwn-exploit](https://skills.sh/yxy050208/qwen-ctf-skills/ctf-pwn-exploit)
- [ctf-web-reverse-audit](https://skills.sh/yxy050208/qwen-ctf-skills/ctf-web-reverse-audit)

## 校验

各压缩包的 SHA-256 校验值记录在 [`SHA256SUMS.txt`](SHA256SUMS.txt) 中。

## 使用声明

这些内容用于 CTF 竞赛、靶场和经授权的安全研究。请仅在获得明确授权的环境中使用其中的技术与工具。
