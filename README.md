# Global Equity Research Library

> 面向全球权益市场研究的结构化资料库。
>
> 当前内容以中国 A 股为主，覆盖每日市场复盘、投资思想与访谈、行业研究框架、策略与资产配置报告等资料。

[![Repository](https://img.shields.io/badge/GitHub-findalphas%2Fglobal--equity-181717?logo=github)](https://github.com/findalphas/global-equity)
![Status](https://img.shields.io/badge/status-active-success)
![Focus](https://img.shields.io/badge/current%20focus-China%20A--Shares-red)
![Content](https://img.shields.io/badge/content-research%20archive-blue)
![Language](https://img.shields.io/badge/language-中文-lightgrey)

## 项目简介

`global-equity` 是一个持续维护的权益投资研究资料库，用于沉淀、分类和检索市场复盘、行业研究、投资方法与策略资料。

当前仓库主要聚焦中国 A 股市场，核心内容包括：

- 持续更新的 A 股每日市场总结；
- 投资人、基金经理、企业家与宏观研究者的思想资料；
- 覆盖主要行业的研究框架和产业知识图谱；
- 市场周期、资产配置、选股、择时与财务分析等策略报告；
- PDF、EPUB 与 Markdown 等多种研究资料格式。

本仓库是一个**研究知识库与资料索引**，不包含完整的量化交易系统、自动化回测框架或实盘交易程序。

## 内容导航

```text
global-equity/
├── README.md
└── china-equity/
    ├── A股每日总结.md
    ├── 投资文集/
    ├── 知识图谱/
    │   └── 长江证券行业研究框架合集/
    ├── 策略报告/
    └── 市场观点/
```

### `china-equity/A股每日总结.md`

按日期持续记录 A 股市场表现，通常包含：

- 主要指数涨跌；
- 两市成交额及量能变化；
- 上涨与下跌家数；
- 领涨、领跌板块；
- 涨停、跌停及市场情绪；
- 盘中与收盘阶段的主要市场特征。

适合用于：

- 快速回顾某一交易日；
- 观察热点轮动和市场风格；
- 建立历史行情事件索引；
- 辅助进行市场周期复盘。

### `china-equity/投资文集/`

收录投资、商业、宏观经济和产品研究等相关资料，形式包括 PDF、EPUB 和 Markdown。

主要内容方向：

- 价值投资与长期主义；
- 基金经理和投资人的访谈、演讲与思想整理；
- 企业经营、产品方法和商业分析；
- 宏观经济研究；
- 财务分析与交易方法资料。

部分主题涉及巴菲特、段永平、张磊、冯柳、张坤、高善文等投资和研究人物。

### `china-equity/知识图谱/`

以行业认知、产业链结构和研究框架为核心，当前包括：

- 新兴产业链图谱；
- 宏观经济与资产配置研究框架；
- 农林牧渔、食品饮料、医药、汽车、机械、电子、通信、计算机；
- 光伏、风电、新能源汽车、电力、公用事业；
- 化工、石油化工、煤炭、钢铁、基本金属、能源金属、贵金属；
- 银行、证券、保险、地产、建筑、建材；
- 传媒互联网、商贸零售、社会服务、纺织服装、家电、家居；
- 交通运输、军工、环保及其他行业。

该目录适合作为行业研究的入门地图，也可用于建立自己的产业链、公司池和跟踪指标体系。

### `china-equity/策略报告/`

收录市场策略、资产配置和投资方法类报告，主要涉及：

- 牛市与市场顶部复盘；
- 春季躁动及景气周期；
- 大类资产配置；
- 永久投资组合与全天候模型；
- 净利润断层等选股方法；
- 公募与私募基金经理择时、选股能力；
- 美元周期、大宗商品周期；
- 财务造假案例；
- 产业生命周期和叙事经济学；
- 分拆上市、跨境资金等专题。

### `china-equity/市场观点/`

收录当前买方和卖方机构的市场观点、周期、资产配置等研究资料。

## 快速开始

### 1. 克隆仓库

由于仓库包含较多 PDF、EPUB 和压缩文件，体积较大，建议根据需求选择下载方式。

完整克隆：

```bash
git clone https://github.com/findalphas/global-equity.git
cd global-equity
```

仅获取最新版本，减少历史记录占用：

```bash
git clone --depth 1 https://github.com/findalphas/global-equity.git
cd global-equity
```

### 2. 在线浏览

Markdown 文件可直接在 GitHub 中阅读。

对于 PDF、EPUB 或 ZIP 文件，可以：

1. 在对应目录打开文件页面；
2. 点击 **Download raw file** 下载；
3. 使用本地阅读器或解压工具查看。

### 3. 在本地检索资料

使用 `ripgrep` 搜索 Markdown 文本：

```bash
rg "新能源|光伏|储能" china-equity
```

使用系统文件名检索：

```bash
find china-equity -type f | grep "资产配置"
```

Windows PowerShell：

```powershell
Get-ChildItem -Recurse .\china-equity |
    Where-Object { $_.Name -match "资产配置" }
```

## 推荐研究工作流

### 市场复盘

1. 从 `A股每日总结.md` 找到目标日期；
2. 记录指数、成交额、热点和情绪；
3. 对照前后交易日判断风格切换；
4. 结合策略报告中的周期框架形成复盘结论。

### 行业研究

1. 在 `知识图谱/` 中阅读行业研究框架；
2. 梳理产业链、核心变量和关键指标；
3. 建立公司与产品清单；
4. 用最新公告、财报和公开数据更新框架；
5. 形成自己的行业跟踪表。

### 投资方法学习

1. 在 `投资文集/` 中选择投资人或研究主题；
2. 提炼其投资原则、研究方法和风险观；
3. 与 `策略报告/` 中的量化或周期框架交叉验证；
4. 将结论转化为可执行的研究清单。

## 文件与目录规范

为便于长期维护，建议新增内容遵循以下规则。

### 目录命名

- 按市场划分一级目录，例如：
  - `china-equity/`
  - `hk-equity/`
  - `tw-equity/`
  - `us-equity/`
  - `eu-equity/`
  - `jp-equity/`
  - `kr-equity/`
  - `sg-equity/`
- 按内容类型划分二级目录，例如：
  - `daily-review/`
  - `investment-anthology/`
  - `industry-frameworks/`
  - `strategy-reports/`
  - `company-research/`
  - `data/`

现有中文目录可继续保留，新目录应保持同一层级命名风格一致。

### 文件命名

推荐格式：

```text
主题_作者或机构_日期_版本.扩展名
```

示例：

```text
半导体行业研究框架_某证券_2026-07.pdf
A股每日复盘_2026-07-20.md
某公司_深度研究_某证券_2026Q2_v1.0.pdf
```

建议：

- 日期统一使用 `YYYYMMDD`；
- 避免使用 `最终版`、`最新版` 等难以追踪的名称；
- 文件名中尽量保留作者、机构、主题和时间；
- 同一文件更新时使用版本号或 Git 历史管理；
- 避免重复上传内容相同但文件名不同的资料。

### 大文件管理

仓库包含较多二进制文件。若后续持续扩充，建议考虑：

- 使用 [Git LFS](https://git-lfs.com/) 管理大文件；
- 避免重复上传相同资料；
- 对压缩包补充内容清单；
- 为超过 GitHub 单文件限制的资料提供合法外部来源链接；
- 定期检查仓库总体积和克隆体验。

Git LFS 示例：

```bash
git lfs install
git lfs track "*.pdf"
git lfs track "*.epub"
git lfs track "*.zip"
git add .gitattributes
```

## 建议的后续建设方向

当前仓库名称为 `global-equity`，内容阶段性集中于中国权益市场。后续可逐步扩展：

- 港股、美股、日股、欧洲股票等市场目录；
- 全球主要指数、行业和 ETF 资料；
- 宏观经济、利率、汇率和商品数据；
- 公司研究、财务模型和估值模板；
- 资料元数据索引；
- 可搜索的目录页和标签体系；
- 机器可读的 CSV、JSON 或 Parquet 数据；
- 自动生成目录与重复文件检测；
- 定期更新的研究日历和变更日志。

建议新增统一索引文件：

```text
catalog.csv
```

可包含以下字段：

```text
market, category, title, author, institution, date, file_path, source_url, tags, copyright_status
```

## 贡献指南

欢迎通过 Issue 或 Pull Request：

- 修正文件名、目录或错别字；
- 补充资料来源、作者、机构和日期；
- 完善目录索引；
- 添加合法公开且有研究价值的资料；
- 删除重复、损坏或来源不清的文件；
- 改进 Markdown 排版和检索体验。

### 提交步骤

```bash
git checkout -b docs/update-catalog
git add .
git commit -m "docs: update research catalog"
git push origin docs/update-catalog
```

随后在 GitHub 创建 Pull Request，并在说明中写明：

- 新增或修改了哪些文件；
- 资料来源；
- 文件版权或公开授权情况；
- 是否存在重复内容；
- 对目录结构的影响。

### Commit Message 建议

推荐使用清晰、可检索的提交信息：

```text
docs: update A-shares daily review for 2026-07-20
docs: add semiconductor industry framework
chore: reorganize strategy reports
fix: correct document filename
remove: delete duplicate research file
```

## 版权与资料来源

本仓库中的部分资料可能来自公开网络、研究机构、出版物、访谈整理或个人收藏。各文档的版权归原作者、出版机构或权利人所有。

维护和使用本仓库时应注意：

- 优先保存原始来源链接和版权信息；
- 不上传未经授权的付费报告、完整图书或受限制资料；
- 对版权状态不明确的文件及时核实；
- 权利人提出有效请求时，应配合删除或替换相关内容；
- 引用资料时应注明作者、机构、标题和来源。

如仓库用于公开长期维护，建议逐步将不确定版权的二进制文件替换为：

- 正版购买或官方获取方式；
- 出版信息和书目索引；
- 官方公开页面链接；
- 在合理引用范围内制作的原创摘要。

## 投资风险提示

本仓库仅用于学习、研究和信息整理，不构成：

- 投资建议；
- 证券推荐；
- 收益承诺；
- 交易指令；
- 法律、税务或财务意见。

历史表现不代表未来结果。市场资料可能存在时效性、遗漏或错误，任何投资决策均应基于独立研究并自行承担风险。

## License

仓库当前未声明统一开源许可证。

在正式添加许可证之前：

- 仓库维护者保留原创 Markdown 内容的相关权利；
- 第三方资料继续受其原有版权约束；
- 未经授权，不应默认仓库中的全部内容均可自由复制、修改或再分发。

如未来主要保留原创索引和研究笔记，可考虑为原创文本采用：

- [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)；
- 或其他符合维护目标的许可证。

代码、数据、原创文本和第三方文献宜分别声明许可证及使用边界。

## 致谢

感谢所有公开分享研究框架、投资思想、市场资料和行业知识的作者与机构。

---

<p align="center">
  <strong>持续积累，独立研究，尊重事实，敬畏市场。</strong>
</p>
