# 16S 微生物组最佳实践系列

这套站点来自已经在服务器上顺序执行并补齐真实结果图的 16S 双端教程，主题是 QIIME2 官方 Atacama soils paired-end 数据集。

## 这版网页包含什么

- 共 13 篇正文页面，覆盖从双端 EMP 原始数据到发表级结果整合。
- 当前正文中嵌入了 27 张真实结果图，全部来自 Atacama soils 双端流程的实际运行产物。
- 页面源码和部署配置已整理成 MkDocs 结构，可直接同步到 GitHub Pages。

## 开始阅读

<div class="grid cards" markdown>

- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（一）：只测一个基因，怎么就能知道有哪些细菌](series/01.md)
  你手上有一批样本——可能是粪便、可能是土壤、可能是水体——你想知道里面有哪些微生物、它们的组成在不同条件下有什么变化。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（二）：搭建环境，拿到数据](series/02.md)
  上一篇我们搞清楚了 16S 分析的核心概念。这一篇我们开始动手——搭环境、下数据、和 QIIME2 打个照面。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（三）：DADA2 去噪——从噪声中找到真实序列](series/03.md)
  上一篇我们把原始数据导入了 QIIME2，做了解复用（demultiplexing）。现在每个样本的 reads 已经分好了——但这些 reads 里有噪声。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（四）：物种注释——给每个 ASV 一个名字](series/04.md)
  上一篇我们从带噪声的 reads 中推断出了 1,080 个 ASV。但目前每个 ASV 只有一串字母序列——你看到 TACGGAGGGGGCTAGCGTTGTTCG... 不会有任何感觉。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（五）：多样性分析——你的样本有多"丰富"，彼此有多"不同"](series/05.md)
  前四篇完成了上游处理——从原始 FASTQ 到过滤后的 ASV 表、物种注释和系统发育树。从这一篇开始，我们进入下游分析。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（六）：物种组成可视化——谁占了多少](series/06.md)
  上一篇的 PCoA 告诉我们"不同体位点的微生物组成整体上很不同"。但"不同在哪"还不清楚——肠道里是什么菌占优势？手掌上又是什么？
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（七）：差异物种分析——谁真的变了](series/07.md)
  上一篇我们"看见"了不同体位点的微生物组成差异——肠道以 Bacteroides 为主，手掌以 Staphylococcus 为主。但"看起来不同"不等于"统计上显著不同"。而且堆叠柱状图只展示了 top...
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（八）：PICRUSt2 功能预测——它们能做什么](series/08.md)
  上一篇我们找到了肠道和口腔之间"谁变了"。 Bacteroides 在肠道富集， Neisseria 在口腔富集——这些是 物种层面 的差异。但审稿人常常会追问：这些物种差异意味着什么功能差异？肠道微生物组和口腔微生物组在 代谢能力...
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（九）：共现网络分析——谁和谁总在一起](series/09.md)
  前面几篇我们一直在单独审视每一个物种：它在哪里多、在哪里少、有什么功能。但生态系统不是个体的简单集合——物种之间存在复杂的互作关系。有些细菌总是一起出现（比如 A 需要 B 的代谢产物），有些细菌互相排斥（比如它们竞争同一种营养物质）。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十）：随机森林 Biomarker 筛选——谁最能代表这个群落](series/10.md)
  第 7 篇的差异分析告诉我们"谁变了"，但差异分析的逻辑是"逐个检验每个物种"——它把每个物种孤立地看。如果我们换一个视角： 能不能用一组物种的组合来预测样本来自哪个组？ 而且不只是找到差异物种，还要排出 优先级...
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十一）：SourceTracker 溯源分析——它们从哪里来](series/11.md)
  前面十篇我们一直在研究"这里有什么"和"不同地方有什么不同"。现在换一个视角： 这些微生物是从哪里来的？
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十二）：微生物组-代谢组联合分析——跨组学的对话](series/12.md)
  到目前为止，我们的 11 篇教程都只用了一种数据——16S 扩增子序列。但在真实的研究中，微生物组几乎不会孤立存在。微生物影响宿主代谢，宿主的代谢环境又反过来塑造微生物组成。要理解这种双向互作，我们需要 同时分析微生物组和代谢组数据 。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十三）：发表级图表与结果整合——最后一公里](series/13.md)
  分析做完了，结果有了，但离发表还差最后一步—— 把分析结果变成审稿人满意的图表 。

</div>

## 使用方式

- 左侧导航按章节阅读。
- 顶部搜索可直接检索工具名、参数名和图表位置。
- 如果你想复用这套站点骨架，bundle 中已经包含 `mkdocs.yml` 和 GitHub Pages workflow。

## 结果图索引

结果图汇总见 [图表总览](figures.md)。