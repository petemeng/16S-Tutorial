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
  上一篇的 PCoA 已经说明： Baquedano 和 Yungay 两条 transect 的群落结构并不一样。但 PCoA 只告诉你“整体不同”，不会直接告诉你“到底是谁多了、谁少了”。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（七）：差异物种分析——谁真的变了](series/07.md)
  上一篇我们已经看到了两条 transect 的组成差异，但柱状图和热图只能告诉你“看起来不一样”。真正写结果时，你还需要回答：
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（八）：PICRUSt2 功能预测——它们能做什么](series/08.md)
  上一篇我们回答了“谁变了”。但审稿时常会被继续追问： 这些类群变化意味着什么功能差异？
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（九）：共现网络分析——谁和谁总在一起](series/09.md)
  前面几篇我们一直在看“某个 genus 在哪里多、哪里少”。但群落不是一个个 genus 独立存在的清单，很多类群会一起波动，也有些类群会呈现互相排斥的模式。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十）：随机森林 Biomarker 筛选——谁最能代表这个群落](series/10.md)
  第 7 篇的 LEfSe 和 ANCOM BC 告诉我们“谁变了”，但它们本质上都是 逐个 genus 检验 。
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十一）：SourceTracker 溯源分析——它们从哪里来](series/11.md)
  前面十篇一直在回答“这里有什么”“谁不同”“谁最重要”。这一篇换个问题： 裸地样本里的群落结构，有多少能被相邻 vegetated 土壤解释？
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十二）：微生物组-代谢组联合分析——跨组学的对话](series/12.md)
  但真实项目里，16S 往往不是终点。你拿到差异 genus、功能预测、biomarker 之后，下一步经常会被问：
- [:material-book-open-page-variant: 16S 微生物组最佳实践系列（十三）：发表级图表与结果整合——最后一公里](series/13.md)
  前面 12 篇已经把分析跑通了，但真正到写报告、写论文、做汇报的时候，还差最后一步：

</div>

## 使用方式

- 左侧导航按章节阅读。
- 顶部搜索可直接检索工具名、参数名和图表位置。
- 如果你想复用这套站点骨架，bundle 中已经包含 `mkdocs.yml` 和 GitHub Pages workflow。

## 结果图索引

结果图汇总见 [图表总览](figures.md)。
