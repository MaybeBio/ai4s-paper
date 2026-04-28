# AI4S 文献阅读技能 - 输出模板

> 供AI4S文献阅读skill使用的输出模板，包含中文版和英文版两个版本。

---

## 中文版模板

```markdown
# [论文标题] 阅读分析报告（中文版）

## 元信息
- **标题**：[论文标题]
- **作者**：[作者列表]
- **发表信息**：[期刊/会议，年份]
- **领域**：[AI4S 子领域]
- **链接**：[arXiv/官方链接]

---

## 原文引用说明

**引用格式**：必须包含行号和位置信息
- **行号**：标注原文所在的具体行号
- **位置**：标注原文所在的section/subsection（如【摘要】、【引言】、【Results/Performance】）

**引用格式示例**：
- `作者在【摘要】中指出「...」（行号4-5）`
- `作者在【Results/DisProt Dataset】部分报告「...」（行号46）`
- `作者在【Methodology/Training】中说明「...」（行号120）`

---

## 1. 核心问题提取
[此处填写中文分析内容，概括核心研究问题、瞄准的缺口、重要性判断]
**原文引用**：`> [原文段落]（行号X，位置：XX部分/XX小节）` 或 行内引用

---

## 2. 理论基准锚定
[此处填写中文分析内容，说明技术范式、理论基础、领域融合方式]

---

## 3. 方法论拆解
[此处填写中文分析内容，详细描述模型架构、数据处理、训练配置、评估方法]

---

## 4. 实证证据审查
[此处填写中文分析内容，说明假设验证结果、关键证据、基线对比]

---

## 5. 方法论漏洞查找
[此处填写中文分析内容，指出致命漏洞、问题类型、潜在影响、改进建议]

---

## 6. 边界条件与局限
[此处填写中文分析内容，界定数据边界、技术边界、已知局限、额外观察局限]

---

## 7. 文献交叉验证
[此处填写中文分析内容，说明学术对话定位、战略地位]

---

## 8. 核心贡献提炼
[此处填写中文分析内容，列出核心贡献及影响，说明范式转变]

---

## 9. 未来研究裂变
[此处填写中文分析内容，提出新研究方向、研究问题、方法升级]

---

## 10. 可复现性评估
[此处填写中文分析内容，评估代码、数据、文档的可得性及复现难度]

---

## 综合评分
| 维度 | 评分（1-5） | 说明 |
|------|-------------|------|
| 创新性 | [ ] | [ ] |
| 方法严谨性 | [ ] | [ ] |
| 实证充分性 | [ ] | [ ] |
| 领域价值 | [ ] | [ ] |
| 可复现性 | [ ] | [ ] |
| **综合** | **[ ]** | [ ] |

---

## 阅读总结
[此处用中文撰写 1-2 段话，总结这篇论文的核心价值和你是否会引用它，以及如何引用（用于支撑什么观点）]
```

---

## 原文引用说明

**引用格式要求**：
- **必须包含行号和位置信息**
- **行号**：标注原文所在的具体行号
- **位置**：标注原文所在的section/subsection（如【Abstract】、【Introduction】、【Results/Performance】）

**引用格式示例**：
- `作者在【Abstract】中指出「...」（行号4-5）`
- `作者在【Introduction/Unstructured Regions Define a New Heterogeneous Structural Reality】部分指出「...」（行号11）`
- `作者在【Results/DisProt Dataset】部分报告「...」（行号46）`
- `作者在【Methodology/Training and testing set】中说明「...」（行号120）`

---

## 英文版模板

```markdown
# Literature Analysis Report: [Paper Title] (English Version)

## Meta Information
- **Title**: [Paper Title]
- **Authors**: [Author List]
- **Publication**: [Journal/Conference, Year]
- **Field**: [AI4S Sub-field]
- **Link**: [arXiv/Official Link]

---

## 1. Core Problem Extraction
[Chinese report translated to academic English]

**Original Citation**: `> [Original text] (Line X-Y, Location: XX Section/XX Subsection)` or inline citation

---

## 2. Theoretical Anchoring
[Chinese report translated to academic English]

---

## 3. Methodology Deconstruction
[Chinese report translated to academic English]

---

## 4. Empirical Evidence Review
[Chinese report translated to academic English]

---

## 5. Critical Flaw Detection
[Chinese report translated to academic English]

---

## 6. Boundary Conditions & Limitations
[Chinese report translated to academic English]

---

## 7. Literature Cross-Validation
[Chinese report translated to academic English]

---

## 8. Core Contribution Distillation
[Chinese report translated to academic English]

---

## 9. Future Research Directions
[Chinese report translated to academic English]

---

## 10. Reproducibility Assessment
[Chinese report translated to academic English]

---

## Overall Rating
| Dimension | Score (1-5) | Notes |
|------------|----------------|-------|
| Innovation | [ ] | [ ] |
| Methodological Rigor | [ ] | [ ] |
| Empirical Adequacy | [ ] | [ ] |
| Domain Value | [ ] | [ ] |
| Reproducibility | [ ] | [ ] |
| **Overall** | **[ ]** | [ ] |

---

## Reading Summary
[Chinese report translated to academic English]
```