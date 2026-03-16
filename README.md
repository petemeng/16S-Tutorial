# 16S 微生物组最佳实践系列

这套站点来自已经在服务器上顺序执行并补齐真实结果图的 16S 双端教程，主题是 QIIME2 官方 Atacama soils paired-end 数据集。

## 这版网页包含什么

- 共 5 篇正文页面，覆盖从双端 EMP 原始数据到 alpha/beta 多样性分析。
- 当前正文中嵌入了 11 张真实结果图，全部来自 Atacama soils 双端流程的实际运行产物。
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

</div>

## 使用方式

- 左侧导航按章节阅读。
- 顶部搜索可直接检索工具名、参数名和图表位置。
- 如果你想复用这套站点骨架，bundle 中已经包含 `mkdocs.yml` 和 GitHub Pages workflow。

## 结果图索引

结果图汇总见 [图表总览](figures.md)。
