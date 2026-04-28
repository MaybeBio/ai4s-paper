# ai4s-paper

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://docs.anthropic.com/en/docs/claude-code)

一个用于 AI for Science (AI4S) 学术论文深度分析的 Claude Code Skill，采用 10 维度系统性分析框架，生成中英双文结构化报告，含精确原文引用。

> **English summary**: A Claude Code skill for deep analysis of AI4S academic papers. Features a 10-dimension systematic framework (Core Problem, Theoretical Anchoring, Methodology, Empirical Evidence, Critical Flaws, Boundaries, Literature Validation, Contributions, Future Research, Reproducibility), bilingual output (Chinese+English), and original text citations with line numbers and section locations.

---

## 功能亮点

- **10 维度系统性分析框架**：从核心问题提取到可复现性评估，全方位解构文献
- **中英双文输出**：生成中文版（个人理解）和英文版（PPT 展示）两份独立报告
- **精确原文引用**：所有关键论点必须标注原文行号和位置，避免幻觉
- **AI4S 领域专业化**：针对生物医学、药物发现、蛋白质科学、基因组学等交叉学科优化
- **批判性思维导向**：以审稿人标准识别方法论漏洞、边界条件和局限性

---

## 快速开始

### 前置条件

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) CLI 已安装

### 安装

```bash
npx skills add <your-username>/ai4s-paper
```

> 也可以手动克隆：`git clone https://github.com/<your-username>/ai4s-paper ~/.claude/skills/ai4s-paper`

### 使用

在 Claude Code 中，直接用自然语言触发：

```
/ai4s-paper 分析这篇关于蛋白质结构的论文
/ai4s-paper deep read this medical imaging paper
/ai4s-paper 帮我分析这篇药物发现论文的方法论漏洞
/ai4s-paper evaluate the experimental design of this genomics paper
```

---

## 分析框架

本技能按照以下 10 个维度系统性地分析每篇文献：

| 维度 | 英文 | 核心内容 |
|------|------|----------|
| 1 | Core Problem Extraction | 识别研究的原始张力与核心缺口 |
| 2 | Theoretical Anchoring | 识别支撑研究的基础理论与技术范式 |
| 3 | Methodology Deconstruction | 将研究设计逆向工程为可理解的技术蓝图 |
| 4 | Empirical Evidence Review | 提取核心、显著的实证发现 |
| 5 | Critical Flaw Detection | 识别研究设计中的致命缺陷 |
| 6 | Boundary Conditions & Limitations | 界定研究发现的适用范围 |
| 7 | Literature Cross-Validation | 将研究置于更大的学术对话中 |
| 8 | Core Contribution Distillation | 提炼研究的根本价值 |
| 9 | Future Research Fission | 基于本文裂变出新的研究问题 |
| 10 | Reproducibility Assessment | 评估研究的可复现性 |

---

## 引用规范

这是本 skill 的核心设计，确保分析的严谨性：

**混合引用格式**

```
# 引用块格式（长段落）
> We hypothesize that very long contiguous segments with nonregular secondary structure (NORS regions) differ significantly from regular, well-structured loops（行号27-28）【位置：Introduction/Unstructured Regions Define a New Heterogeneous Structural Reality】

# 行内引用格式（短句）
作者在【摘要】中指出「Natively unstructured or disordered protein regions may increase the functional complexity of an organism」（行号4-5）
```

**引用三要素**
1. **必须使用原文**：不得改写或转述，直接引用论文原始英文
2. **必须标注行号**：使用 Read 工具读取论文时记录行号
3. **必须标注位置**：标注原文所在的 section/subsection

---

## 输出结构

每次分析生成两个独立文件：

### 中文版：`[论文标题]_review_ch.md`
- 适合个人深度理解
- 中文主导，技术术语保留英文
- 含原文引用

### 英文版：`[论文标题]_review_en.md`
- 适合学术展示和 PPT 使用
- 英文学术规范
- 原文引用保持英文，不翻译

**两版内容完全对应，结构一致，方便对照阅读**

---

## AI4S 领域覆盖

本技能专注于 AI for Science 领域：

- **医疗影像**：医学成像、诊断影像、医学图像分析
- **药物发现**：药物设计、分子对接、药物筛选
- **蛋白质科学**：蛋白质结构、蛋白质预测、无序蛋白、NORS
- **基因组学**：基因表达、DNA/RNA 分析、基因测序
- **生物医学**：生物信息、计算生物学、临床研究
- **科学计算**：物理仿真、化学计算、科学计算建模

---

## 文件结构

```
ai4s-paper/
├── SKILL.md                        # Skill 主配置（Claude Code 入口）
├── README.md                       # 本文件
├── LICENSE                         # MIT 许可证
└── references/
    ├── templates.md                # 中英双文输出模板
    ├── citation-rules.md           # 原文引用详细规范
    └── quality-checklist.md       # 反幻觉和质量检查清单
```

---

## 反幻觉机制

本技能内置以下质量控制机制：

| 机制 | 说明 |
|------|------|
| **强制引用** | 所有涉及原始证据的分析必须引用原文内容 |
| **行号定位** | 引用时标注原文所在的具体行号 |
| **位置标注** | 标注原文所在的 section/subsection |
| **不确定性标记** | 信息缺失时标注 `[未明确给出]`，有歧义时标注 `[不确定]` |
| **技术术语保留** | 模型名称、算法名称、数据集名称保留英文 |

---

## License

MIT License — Copyright (c) 2026

本项目以 MIT 许可证开源。你可以自由使用、修改和分发，但需保留原始版权声明。

完整许可证文本见 [LICENSE](LICENSE) 文件。

---

## Contributing

欢迎提交 Issue 和 Pull Request。

如果你在使用中发现引用错误、分析偏差或输出格式问题，欢迎在 Issue 中附上复现步骤（论文链接 + 触发词 + 错误输出片段）。