# GithubCollection


GITHUB应用集
录屏软件：
Openscreen 平替付费软件screen studio

开发软件：
Oh-my-codex ，替代cursor，支持多个agent协作。

sherlock ，输入一个用户名，自动搜索300+平台。


量化交易

市场数据
## 1. AKShare (国内最火、开源免费)
如果你关注 A股、港股、甚至国内期货，AKShare 是绕不开的工具。
核心特色：它是目前国内最全的开源金融数据库，数据抓取自东方财富、新浪财经、腾讯证券等各大门户。
主要功能：涵盖股票、基金、期货、债券、外汇、宏观经济数据。
极客价值：它是一个 Python 库，不需要注册 Token（不像 Tushare），拿来即用。它能轻松抓取“新闻快讯”和“研报数据”，非常适合喂给你的 AI Agent 做情感分析。
GitHub: akfamily/akshare

## 2. OpenBB (原 GamestonkTerminal)
这是全球量化界最知名的开源项目，目标是打造“开源版的彭博终端”。
核心特色：提供了一个极强的数据聚合层。无论你想调取纳斯达克的实时行情，还是社交媒体上的散户情绪（Reddit/Twitter），它都有统一的接口。
2026 最新动态：OpenBB 现已深度集成 MCP (Model Context Protocol)，这意味着你可以让你的本地 AI Agent 直接调用 OpenBB 的能力去获取全市场的即时数据。
GitHub: OpenBB-finance/OpenBBTerminal

## 3. Vibe-Trading (2026 爆火的新秀)
这是近期由 HKUDS 团队开发的 AI 驱动多智能体工作空间。
核心特色：它不仅汇总信息，还自带 "Smart Data Access" 机制。它会自动切换 5 种以上的数据源（如 AKShare + CCXT），如果某个接口挂了，它会自动重试或 fallback 到备用数据。
技术适配：支持一键导出到 通达信/同花顺/TradingView 等平台，非常适合习惯国内交易软件的用户。
GitHub: HKUDS/Vibe-Trading

数据分析图像界面
## 1. 配合 OpenBB 使用（最接近专业终端）
这是目前最推荐的方案。OpenBB 是一个开源的金融终端，类似于“开源版 Bloomberg”。
如何实现：OpenBB 提供了一个 OpenBB Dashboard（Web 界面）。你可以通过安装特定的插件或使用 OpenBB Platform，将 AKShare 作为数据提供商（Backend）接入。
体验：你可以在浏览器里看到精美的 K 线图、基本面仪表盘，而底层数据是由 AKShare 实时抓取的。

## 2. Vibe-Trading（2026 年新趋势）
正如前面提到的，Vibe-Trading 是一个集成了 AKShare 的 AI 智能体项目。
图形界面：它自带了一个基于 Web 的 UI。
特点：你不仅能看到图形化的市场数据，还可以直接在界面里和 AI Agent 交流，让它调用 AKShare 数据并画出分析图表。

## 3. 搭配可视化框架（适合 DIY 研发）
如果你想利用自己的研发能力快速“撸”一个界面，通常开发者会配合以下工具：
Streamlit: 极其简单。只需几行代码，就可以把 AKShare 的 DataFrame 数据变成一个交互式的网页图表。
丁香园/数据观 (Datalore): 这种在线 NoteBook 也可以提供非常直观的表格和绘图展示。


从yahoo finannce获取财经数据
pip install yfinance

