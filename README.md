# ⚖️ 模拟法庭训练智能体

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

一个基于 Claude Code 的民事案件模拟法庭训练工具，专为法学生和法律从业者设计。通过角色扮演和互动式训练，帮助用户提升法律思维、庭审表达和应变能力。

---

## ✨ 功能亮点

- 🎭 **三种角色切换** — 法官、对方律师、案件当事人，全真模拟庭审场景
- 📋 **双模式训练** — 出题模式（AI 出题你应对）和咨询模式（你提问 AI 分析）
- 📊 **三级难度** — 基础 → 标准 → 困难，从典型案情到极端情形逐步进阶
- 📝 **五维评分** — 法律知识、逻辑推理、语言表达、应变能力、庭审礼仪
- 🏛️ **三大案由** — 合同纠纷、婚姻家庭、侵犯类案件全覆盖
- 🇨🇳 **中国法律** — 所有分析基于中国现行民事法律体系

---

## 🚀 快速开始

### 前置条件

- 安装 [Claude Code](https://docs.anthropic.com/en/docs/claude-code)

### 方式一：克隆仓库（推荐）

```bash
git clone https://github.com/YOUR_USERNAME/moot-court-agent.git
cd moot-court-agent
claude
```

CLAUDE.md 会自动加载，智能体将以模拟法庭导师身份启动。

### 方式二：仅使用 Slash 命令

1. 将 `commands/moot-court.md` 复制到你当前项目的 `.claude/commands/` 目录下
2. 在任意 Claude Code 会话中输入 `/moot-court` 即可启动

```bash
mkdir -p .claude/commands
cp commands/moot-court.md .claude/commands/
```

---

## 🎮 使用演示

启动后，智能体会引导你完成设置：

```
⚖️ 模拟法庭训练智能体

欢迎！请选择：
1️⃣ 模式：出题模式 / 咨询模式
2️⃣ 类型：合同纠纷 / 婚姻家庭 / 侵犯类
3️⃣ 难度：基础 / 标准 / 困难
```

### 出题模式示例

```
【模式：出题 | 类型：合同纠纷 | 难度：标准 | 回合：1】

【原告律师】：我的当事人与被告签订设备采购合同，
约定3月1日交付。被告逾期30天交货，且设备存在严重缺陷。
现请求解除合同、返还货款并赔偿损失。
请问学生律师，您将为被告提出何种抗辩？
```

你以律师身份回应后，智能体会给出合理性判断：

```
合理性判断：部分合理
理由：你提出了不可抗力抗辩，但未考虑减损义务和
因果关系的时间节点……
```

训练结束时自动输出完整案件分析 + 五维评分表。

---

## 📁 文件结构

```
moot-court-agent/
├── CLAUDE.md                  # 智能体系统提示（自动加载）
├── commands/
│   └── moot-court.md          # Slash 命令（/moot-court）
├── README.md                  # 本文件
└── LICENSE                    # MIT 许可
```

---

## 🔧 自定义

你可以修改 `CLAUDE.md` 来调整智能体行为：

- 增加新的案件类型
- 调整评分维度权重
- 添加常用案例库
- 修改角色扮演风格

---

## 📄 许可

MIT License © 2025

---

## ⚠️ 免责声明

本工具仅供教学训练使用，所有法律分析和案情设计不构成正式法律意见。真实案件请咨询持证律师。
