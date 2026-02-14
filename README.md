# ljg-skill-xray-paper

论文X光机 (Paper X-Ray Scanner) — 一个 **CodeX Skill**，解构学术论文，穿透学术黑话，还原作者最底层的逻辑模型。

## 功能

- 支持 PDF 路径、文本内容或论文链接输入
- 认知提取算法：去噪 → 提取 → 批判
- 大白话开场：10 秒内决定要不要继续读
- Introduction 概览图：领域时间线 + 本文定位
- 五维分析：核心痛点、解题机制、创新增量、批判性边界、餐巾纸公式
- 自包含输出：禁止裸公式，术语即用即释
- 生成 Org-mode 格式报告，含 ASCII 逻辑流程图

## 在 CodeX 中安装

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --url https://github.com/lijigang/ljg-skill-xray-paper/tree/main/skills/ljg-xray-paper
```

安装后重启 CodeX 以加载新 Skill。

## 在 CodeX 中使用

在 CodeX 中直接描述任务，例如：

```
请使用 ljg-xray-paper 分析这篇论文：<论文PDF路径、URL或粘贴内容>
```

## Claude 兼容说明

仓库保留 `.claude-plugin/` 元数据，方便已有 Claude 侧流程继续使用；CodeX 适配文件位于 `skills/ljg-xray-paper/agents/openai.yaml`。

## 输出示例

生成的 Org-mode 报告包含：

- **PLAIN TALK** — 大白话开场，外行能听懂的 2-3 句话
- **LANDSCAPE** — ASCII 概览图：历史时间线 + 本文位置
- **NAPKIN FORMULA** — 餐巾纸公式，一句话浓缩核心
- **PROBLEM** — 痛点定义与前人困境
- **INSIGHT** — 作者的灵光一闪
- **DELTA** — 相比 SOTA 的创新增量
- **CRITIQUE** — 隐形假设与未解之谜
- **LOGIC FLOW** — ASCII 逻辑结构图
- **NAPKIN SKETCH** — ASCII 餐巾纸图

## License

MIT
