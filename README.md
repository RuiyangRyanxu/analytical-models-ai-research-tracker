# Analytical Models & AI Research Tracker

> A curated, continuously updated paper archive for researchers working on analytical models, game theory, AI, AI agents, platforms, and strategic behavior.

**公开网站：** https://ruiyangryanxu.github.io/analytical-models-ai-research-tracker/

## 项目目的

本项目旨在帮助聚焦 analytical models、game theory、AI、AI agents、platforms 与 strategic behavior 的研究者，快速了解最新研究进展。它不只是论文链接列表，而是将筛选、去重、来源核验、读前导览和详细总结整合到每日报告中。

## 项目概览

- 按日期归档每日文献报告，并默认展示最新检索日期。
- 通过来源、研究类型和发布状态分布快速了解当日论文构成。
- 支持按论文题目关键词或作者姓名跨日期检索，并直接定位到报告中的对应论文。
- 模型论文优先展示参与者、决策、博弈顺序、关键公式和比较静态；实证论文优先展示数据、识别策略、结果和机制。
- 公开归档从 `2026-07-14` 开始，只展示现行规则生效后的报告。

## 关注范围

- **方法与理论：** game theory、analytical model、mechanism model、strategic behavior。
- **研究主题：** AI、AI agents、platforms、digital markets 与 Economics-IO。
- **Working papers：** SSRN、arXiv、NBER、CEPR、IZA、作者主页与会议论文页面。
- **期刊 online：** 仅纳入 UTD Top 24、经济学五大刊、*RAND Journal of Economics*、*Journal of Economic Theory* 与 AEJ 全系列。

## 使用方式

1. 在首页分别选择年、月、日，查看当日论文分布。
2. 输入篇名关键词或作者姓名，跨报告检索论文。
3. 进入完整报告，阅读每篇论文的读前导览、核心结论和结构化分析。

## 使用声明

本站内容仅供学习与研究参考，不构成对论文质量、研究结论或实际决策的背书。结构化摘要不能替代对原文、版本记录和正式发表页面的阅读与核验。

## 仓库结构

GitHub Pages 公开文件位于 `site/`，内容由日报生成器同步。

## 更新公开文件

```bash
cd ..
python3 scripts/build_literature_portal.py \
  --outputs outputs \
  --output outputs/index.html \
  --minimum-date 2026-07-14 \
  --site-dir literature-portal-site \
  --github-pages-dir literature-portal-pages
```

推送 `main` 后，GitHub Actions 会把 `site/` 部署到 GitHub Pages。
