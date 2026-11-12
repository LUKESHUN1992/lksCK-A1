# GitHub 热门笔记

记录 GitHub Trending 官方榜单，追踪开源社区的技术风向。

## 这个仓库是做什么的

每天或每周抓取 [GitHub Trending](https://github.com/trending) 页面，把热门仓库整理成中文笔记，方便回看「某个时间点大家在关注什么」。

每篇笔记包含：

- 仓库全名（owner/repo）与链接
- 总 Star 数、周期内新增 Star 数
- 主要编程语言
- 一句话简介
- 趋势解读与关注建议

## 目录结构

```
github-trending-notes/
├── README.md          # 本文件，仓库说明
├── 2026-11-12.md      # 当日榜单笔记
└── YYYY-MM-DD.md      # 之后按日期追加
```

## 榜单口径

| 项目 | 说明 |
| --- | --- |
| 排序依据 | 按**周期内新增 Star 数**降序排列 |
| 时间窗口 | 今日 `daily` / 本周 `weekly` / 本月 `monthly` |
| 数据性质 | 官方公开页面的**实时快照**，与页面当前展示可能有细微差异 |
| 注意事项 | 热度反映社区短期关注，**不等同于项目质量评价**，仅作技术情报参考 |

## 常用抓取入口

```
全语言今日：https://github.com/trending
本周榜单：  https://github.com/trending?since=weekly
本月榜单：  https://github.com/trending?since=monthly
Python 榜： https://github.com/trending/python?since=daily
Rust 榜：   https://github.com/trending/rust?since=weekly
```

把 `python`、`rust` 换成 `javascript`、`typescript`、`go`、`java` 等即可切换语言。

## 如何更新

1. 打开 [github.com/trending](https://github.com/trending)，选择时间窗口与语言
2. 在本仓库新建 `YYYY-MM-DD.md`，按已有笔记的格式填写
3. 网页端可直接 `Add file → Upload files` 拖入文件，或用 Git 提交

## 可选：把笔记变成网页

在仓库 `Settings → Pages` 中，Source 选择 `Deploy from a branch`，分支选 `main`、目录选 `/ (root)`，保存后即可通过
`https://<用户名>.github.io/<仓库名>/` 访问。

## 小提示

- 仓库名只能用英文字母、数字、`.`、`-`、`_`，且不超过 100 字符
- 仓库描述（Description）和文件内容**可以写中文**
- 内容不想公开就把仓库设为 Private，免费账户也无数量限制

---

数据来源：GitHub Trending 官方页面 · 首篇笔记记录于 2026-11-12
