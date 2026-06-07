@C:\Users\chenz\.codex\RTK.md

--- project-doc ---

# AGENTS.md

## 项目背景
本项目用于高级宏观经济学博士课程的课堂汇报 slides。

汇报论文为：

`Long-Run Implications of Investment-Specific Technological Change.pdf`

论文相关材料位于：

`Long-Run Implications of Investment-Specific Technological Change/`

撰写 slides 时，应优先阅读原始 PDF 与已整理的相关材料。若后续生成了 Markdown、摘录笔记或 OCR 文档，应优先使用这些文本材料快速定位结构、段落、公式和图表；遇到公式、图表、页码、命题编号或引用不清楚时，再回到原始 PDF 核对。

汇报时间为 2026 年 6 月 16 日。最终汇报时长为 30 分钟，目标是对论文进行较为详细的介绍。听众应被视为已经具备研究生层次的宏观经济学、动态优化、增长理论和一般均衡基础，因此 slides 的重点应放在论文的问题意识、理论框架、关键假设、主要推导、核心结果、经济学直觉以及与宏观经济问题的联系上。

除了解释论文在 1997 年语境下的贡献，还应讲清楚：这篇文章对今天的研究有什么启示。汇报不应只停留在“作者当年做了什么”，还应回答“这个识别思路、建模方式、测量问题和结论，对当前关于技术进步、资本异质性、无形资本、AI、生产率放缓、增长核算和结构转型的研究意味着什么”。

## 主要交付物
主要交付物是一个 LaTeX Beamer 幻灯片项目，目前核心文件是：

`slides/Greenwood 1997 aer.tex`

编译后的输出文件是：

`slides/Greenwood 1997 aer.pdf`

`slides/Greenwood 1997 aer.tex` 中的 slides 正文应使用中文撰写，包括标题、bullet points、模型说明、结论和经济学直觉。论文专有名词、模型变量、公式符号、英文术语和必要引用可以保留英文或中英混写，例如 investment-specific technological change、neutral productivity、balanced growth path、`q`、`k_e` 等。

用于规划后续 slides 的 Markdown 文档（例如 `plan.md`）也应使用中文撰写；专有名词、论文术语、变量符号和拟用于正式 slides 的英文短语可以保留英文。

除非用户明确要求重新设计版式，否则修改 slides 时应尽量保留现有的中山大学 SYSU Beamer 风格。

## 汇报结构
汇报由 5 位成员完成，每人负责论文的一部分。建议分工如下：

成员：陈宇新、陈致远、邝逸、赵天驰、郑文绰

40 分钟汇报中，每位成员平均大约控制在 8 分钟。Slides 应足够支撑宏观理论课上的细致讲解，但不要写成逐字稿；每页应服务于口头解释。

建议结构可以围绕以下通用逻辑展开，并在阅读论文后根据实际内容调整：

- Motivation and research question.
- Economic environment, assumptions, and timing.
- Model solution, equilibrium conditions, and main mechanisms.
- Key propositions, quantitative exercises, or empirical facts, if applicable.
- Economic intuition, limitations, and broader macro implications.

## 内容优先级
本项目的核心是对一篇高级宏观经济学论文进行准确、清晰、有层次的课堂讲解。优先处理以下内容：

- 清楚说明论文研究的问题、背景和核心贡献。
- 定义模型中的主要主体、状态变量、控制变量、约束条件和均衡概念。
- 分步骤展示关键假设、最优化问题、均衡条件和主要推导。
- 对重要数学结果先说明公式内容，再解释经济学含义。
- 每个重要结论后都要给出直觉解释，避免只展示结论而不解释机制。
- 使用图示或表格帮助说明模型结构、变量关系、比较静态、校准结果或经验事实。
- 区分论文中的理论机制、定量结果、经验事实、政策含义和作者自己的解释。
- 明确总结这篇文章对当前研究的启示，包括它在今天仍然重要的问题意识、识别策略、测量框架和可能的局限。
- 对论文中暂时不确定或尚未核对的内容，应标注为待核对，不要直接写成确定结论。

背景、动机和文献综述应保持简洁。经验事实和历史背景只有在有助于理解模型机制或量化结果时才展开。

## Slides 写作规范
`slides/Greenwood 1997 aer.tex` 的正式 slides 内容使用中文。论文专有概念、模型变量、公式、英文术语和必要引用可保留英文或论文原符号；对于重要术语，优先采用“中文解释 + 英文术语”的方式，便于课堂讲解和与原文对应。

`plan.md` 及其他汇报规划文档也使用中文撰写；如果其中包含未来会直接放入 slides 的标题或 bullet，可以先写中文，并在括号中保留关键英文术语。

推荐的单页组织方式：

- 每个部分开头先说明本部分要回答的问题。
- 先给假设和符号，再给使用这些符号的公式。
- 避免大段文字；优先使用公式、简洁 bullet 和口头可展开的直觉。
- Slides 正文不必写完整句子；优先使用短语式 bullet，适当删减句子内容，只保留讲解所需的关键词、假设、变量、结果和直觉。
- Slides 中公式编号不必对应原文编号；除非用户明确要求引用原文公式编号，否则不要为了对应论文而强行使用 `\tag{...}`。
- Slides 中展示公式统一使用 `equation` 环境；需要多行、对齐或分组时，在 `equation` 内嵌套 `aligned`、`gathered`、`split` 等结构。除非用户明确要求，不要直接使用 `align`、`align*`、`\[`、`$$` 等展示公式环境。
- 长推导应拆成多页，不要把完整代数过程挤在一页。
- 适当使用 `block`、`theorem`、`lemma`、`proposition`、`proof` 和 `alertblock` 环境。
- 每个重要结果页最好同时包含 “Result” 和 “Intuition”。
- 如果用户需要排练友好版本，可以加入汇报人标签或更清晰的分段标题。

## 技术说明
这是一个 LaTeX Beamer 项目。由于可能使用 `ctex` 和中文字体，通常应使用 XeLaTeX 编译。

注意文件编码。如果在终端中看到中文乱码，不要贸然大范围修改 `.tex` 文件，应先确认编码。新建文件优先使用 UTF-8。

### Codex / Windows 沙箱注意事项
本项目路径包含中文目录，并位于 Nutstore 同步目录下。在 Windows managed sandbox 下，Codex 偶尔会在执行普通 PowerShell 命令前失败，报错类似：

```text
windows sandbox: spawn setup refresh
```

这属于 Codex 工具层的沙箱初始化问题，不是 LaTeX、Beamer 或源码语法错误。遇到该错误时，应按权限规则使用 `sandbox_permissions: "require_escalated"` 重新运行同一条必要命令；不要因为这个错误去修改 `.tex` 文件内容。若频繁出现，可在新的 Codex 会话中切换到更宽松的 filesystem sandbox，或将项目复制到不含中文路径的本地目录后再运行。

除非用户明确要求，不要修改以下 LaTeX 生成文件：

- `.aux`
- `.log`
- `.nav`
- `.out`
- `.snm`
- `.synctex.gz`
- `.toc`

## 编译命令
推荐使用 XeLaTeX 编译，例如：

```powershell
xelatex -synctex=1 "Greenwood 1997 aer.tex"
```

在 `slides/` 目录下运行该命令。如果需要从 PDF 反向跳转到对应 `.tex` 源码，必须保留 `-synctex=1` 以生成 `.synctex.gz`。如果目录、交叉引用或页码没有更新，运行两次 XeLaTeX。

## 编辑规则
修改 slides 时应遵守：

- 先阅读论文中相关部分，再改写 slides。
- 优先使用已转换或已整理的文本材料定位内容；涉及公式、图表和命题细节时回到 PDF 核对。
- 保留用户已有修改，不要覆盖未确认的内容。
- 修改范围应紧扣本次汇报任务。
- 不要虚构论文中不存在的假设、命题、校准结果或结论。
- 如果为了课堂讲解简化推导，应明确说明简化在哪里。
- 尽量忠实使用论文原有符号；如果为了清晰更换符号，需要说明对应关系。
- 未经明确指示，不要删除论文 PDF、图片、样式文件或编译生成文件。

## 质量检查清单
在认为 slides 已经完成前，检查：

- 总时长是否适合 40 分钟汇报。
- 论文的问题意识、研究背景和核心贡献是否交代清楚。
- 是否清楚说明了这篇 1997 年论文对当前研究的启示，而不只是复述历史贡献。
- 模型设定是否完整到足以支撑后续分析。
- 是否包含关键假设、均衡条件、推导步骤和主要结果。
- 重要推导是否被展示，而不是只给结论。
- 每个技术结果是否配有经济学直觉。
- 理论机制、定量结果、经验事实和政策含义是否区分清楚。
- 是否避免了未经核对的具体结论、参数值、命题或作者观点。
- 是否可以用 XeLaTeX 成功编译。
