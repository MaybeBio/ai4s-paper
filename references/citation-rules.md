# Citation Rules & Format

## 核心原则

**所有涉及原始证据的分析必须引用原文内容！** 这是本技能的最高优先级要求。

---

## 引用格式

### 引用块格式（长段落）

用于独立段落或开头陈述时，使用引用块：

```markdown
> 原文内容（行号 X-Y）【位置：XX部分/XX小节】
```

**示例**：
```markdown
> Natively unstructured or disordered protein regions may increase the functional complexity of an organism; they are particularly abundant in eukaryotes and often evade structure determination.（行号4-5）【位置：摘要】
```

---

### 行内引用格式（短句）

用于在分析文本中嵌入引用：

```markdown
作者认为「原文片段」（行号X，位置：XX部分）
```

或者：

```markdown
作者在【摘要】中指出「原文片段」（行号4-5）
```

**示例**：
```markdown
作者在【Introduction/Unstructured Regions Define a New Heterogeneous Structural Reality】部分指出「We hypothesize that very long contiguous segments with nonregular secondary structure (NORS regions) differ significantly from regular, well-structured loops」（行号27-28）
```

---

## 引用三要素

### 1. 必须使用原文

- **不得改写或转述**：直接引用论文原始英文
- **保持原文拼写**：包括拼写错误、大小写等
- **保留专有名词**：数据集名称、模型名称等

### 2. 必须标注行号

- 使用 Read 工具读取论文时记录行号
- 引用时标注准确的行号范围
- 单行标注：`行号27`，多行标注：`行号27-28`

### 3. 必须标注位置

标注原文所在的 section/subsection：

- **中文位置**：【摘要】、【引言】、【Results/Performance】、【Methodology/Training】
- **英文位置**：保持论文原始英文命名
- **详细定位**：如果有小节，标注 `XX部分/XX小节`

---

## 位置标注示例

| 场景 | 格式 | 示例 |
|------|------|------|
| 摘要部分 | `【摘要】` | 作者在【摘要】中指出「...」（行号4-5） |
| 英文小节 | `【Introduction/Unstructured Regions Define a New Heterogeneous Structural Reality】` | 作者在【Introduction/Unstructured Regions Define a New Heterogeneous Structural Reality】部分指出「...」（行号11） |
| 结果子节 | `【Results/DisProt Dataset】` | 作者在【Results/DisProt Dataset】部分报告「...」（行号46） |
| 方法子节 | `【Methodology/Training and testing set】` | 作者在【Methodology/Training and testing set】中说明「...」（行号120） |
| 通用部分 | `【引言】` | 作者在【引言】中提到「...」（行号30） |

---

## 高亮标注

原文片段用 `「...」` 包裹，突出显示：

- ✅ `作者认为「natively unstructured regions may increase functional complexity」（行号4-5）`
- ✅ `> 「NORS regions differ significantly from regular loops」（行号27-28）【位置：Introduction】`
- ❌ `作者认为natively unstructured regions may increase functional complexity`（无高亮）
- ❌ `作者说无序区域很重要`（无原文引用）

---

## 证据对应

每个关键论点必须有对应的原文证据支撑：

| 论点类型 | 引用要求 |
|---------|---------|
| 作者声称的观点 | 原文直接声明，标注 `「原文片段」` |
| 模型归纳的推断 | 标注 `[模型归纳]` 并说明依据 |
| 实验结果 | 引用原文数值，标注来源表/图 |
| 方法描述 | 引用原文方法描述，标注所在章节 |

---

## 双文输出中的引用

**中文版**和**英文版**中的引用规则完全一致：

- 原文引用部分保持英文原文（不翻译）
- 行号标注与中文版一致
- 位置标注与中文版一致

**示例对照**：

| 版本 | 引用 |
|------|------|
| 中文版 | 作者在【摘要】中指出「Natively unstructured or disordered protein regions may increase the functional complexity of an organism」（行号4-5） |
| 英文版 | The author states in the Abstract that "Natively unstructured or disordered protein regions may increase the functional complexity of an organism" (Line 4-5, Location: Abstract) |

---

## 禁止行为

- ❌ 改写原文引用
- ❌ 仅提供页号不提供行号
- ❌ 仅提供章节不提供具体位置
- ❌ 翻译原文引用内容
- ❌ 无引用的断言性陈述
- ❌ 猜测未明确给出的信息