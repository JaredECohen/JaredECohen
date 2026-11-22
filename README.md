# Jared Cohen

I build systematic trading and investment research systems — turning market data, fundamentals, and filings into structured, explainable analysis. My work pairs quantitative methods and agent orchestration with deterministic checks and operator visibility, delivered as full-stack software.

[GitHub](https://github.com/JaredECohen) | [Email](mailto:jaredecohen17@gmail.com)

## Selected Work

| Project | Summary |
| --- | --- |
| [MarketMosaic](https://marketmosaic.ai) (private) | Multi-agent equity research platform ("Your AI Investment Committee") where specialist agents for sector, earnings, filings, valuation, comps, macro, risk, and technicals run in parallel and are synthesized by a Portfolio Manager orchestrator into structured research memos. Includes AI and factor screeners, an editable DCF lab with sensitivity analysis, comps and macro scenario modeling, portfolio construction, primary-document retrieval, and lineage-tracked long-term memory across research runs. Built with FastAPI, React, and Postgres. |
| [Fortior](https://fortior.app) (private) | Native SwiftUI iPhone and Apple Watch training and nutrition app with personalized programs, suggested working weights, progressive-overload analytics, cardio and recovery tracking, meal logging, and body-composition insights. Ask Fortior provides AI coaching grounded in the user's own records, with optional Apple Health, WHOOP, Oura, Strava, and InBody integrations. Includes a web Coach Workspace for athlete collaboration and a permission-scoped MCP connector for external AI tools. Cloud sync, AI, and coach sharing are opt-in. |
| Investing Workspace (private) | Multi-agent research workspace where four AI agents and I run fundamental and quantitative investment research under one written protocol. Key elements are dossiers on 2,471 issuers across a 163-sub-industry taxonomy, a frozen quant trial ledger, and independent cross-agent review of every contribution; it also feeds MarketMosaic's research agents. Built with Python tooling, Git, Markdown and CSV ledgers, Claude, Codex, and other LLM agents, and data from ThetaData, FMP, Alpha Vantage, and SEC EDGAR. |
| [Portfolio Health Check](https://github.com/JaredECohen/portfolio-health-check-scenario-lab) | Full-stack portfolio analysis platform for manually entered U.S. equity portfolios. Combines deterministic analytics, agent orchestration, research overlays, and scenario workflows to answer investor questions with structured memos instead of a static dashboard. |
| [Options Strategy Explainer](https://github.com/JaredECohen/options-AI-assistant) | Options research and education app that explains listed equity strategies, maps market views to trade structures, and calculates payoffs with deterministic checks and an evaluation harness. Includes option chains with IV and greeks, volatility analytics, a screener, an end-of-day backtesting engine, and a strategy finder. Built with FastAPI, React, Postgres, the Anthropic API, and ThetaData. |
| [MTG Deck Lab](https://github.com/JaredECohen/mtg-deck-builder) | Free Magic: The Gathering deck builder that generates legal, explainable decks from user constraints. A card-level simulator and optimizer drive the builds, and an LLM builder-and-critic loop reviews each candidate. Built with Next.js, FastAPI, and SQLite, using Claude and OpenAI models. Live at [mtgdecklab.app](https://mtgdecklab.app). |
| [Earnings Call Analyzer](https://github.com/JaredECohen/earnings-call-LLM-analyzer) | Earnings transcript intelligence tool that converts quarterly call transcripts into structured analysis around performance, guidance, sentiment, and risk. |
| Trading Strategies (private) | Automated trading platform on Interactive Brokers: scheduled paper strategies (0DTE short-vol, trend ensemble), a reusable backtest research engine with look-ahead guards, portfolio analytics including a private web and iPhone app, and cloud VM deployment with watchdog alerting. Reads from the live account and writes orders only to a paper account. Built with Python, SQLite, FastAPI, SwiftUI, and GCP. |
| Portfolio Rebalancing Research (private) | Research framework for tax- and cost-aware portfolio rebalancing, built as an IEOR 4737 project with an industry partner. Mixed-integer optimization over rebalancing policies, with a reproducible sweep harness, drift- and factor-based rebalance triggers, walk-forward out-of-sample evaluation, and static/equal-weight benchmarks. Deliverables include a paper, poster, and a generated master report covering every study. |
| NYC PropEngine (private) | Institutional-style NYC real estate valuation and opportunity platform. Hedonic and random-forest AVMs trained on Department of Finance sales, an expected-rent and NOI engine, full pro-forma metrics (cap rate, cash-on-cash, DSCR, 5/10-year IRR) with 2D sensitivity heatmaps, neighborhood market-color modeling, and an AI analyst copilot over a split-screen map and deal feed. |
| Card Market Intelligence (private) | Always-on trading-card market monitor that turns live eBay activity into emailed buy signals, using a two-model ML valuation (market nowcast band plus intrinsic value) over a 480k+-sale comp database, fee-aware flip economics, and point-in-time backtesting of its own signals. Built with Python, SQLite, and APScheduler, with Claude for listing matching. |
| Image Creation Pipeline (private) | End-to-end image generation and merchandising system for research, generation, review, upscaling, and publishing. Designed as an operator control plane rather than a collection of disconnected scripts. |
| BoutIQ (private) | Computer-vision, biomechanics, and tactical AI coaching platform for competitive épée fencing. Auto-clips touches from match footage by detecting scoring-box lights, runs pose kinematics on solo drills, maintains opponent scouting dossiers, and grounds an AI corner coach in the resulting telemetry. Built with Python, FastAPI, pose estimation, and a SwiftUI iOS companion. |
| Thoughtbound (private) | iOS-first reading app built on Expo and Supabase: personal library with search and barcode scan, ratings, shelves, and notes, plus AI summaries anchored on your own highlights and FSRS spaced-repetition review generated from your notes. Backend proxies all model calls; entitlements run on a shared allowance rather than per-feature counters. |
| CYPHER (private) | Native iOS app for voice-driven AI rap battles and flow coaching over hip-hop beats: round-based battles against AI personas, AI-vs-AI exhibitions, solo freestyle generation, and a rhyme and cadence judge, with on-device speech transcription. Built with SwiftUI, AVFoundation, Apple Speech, ElevenLabs, and OpenAI. Site live at [cypher-site](https://jaredecohen.github.io/cypher-site/). |
| AetherCast (private) | Autonomous AI podcast production and publishing platform behind a 50-show catalog: script generation with editorial review, voice synthesis, broadcast-standard audio mastering, scheduled weekly releases, directory distribution, and listening analytics. Built with Python, ElevenLabs, and Cloudflare (R2, Workers, D1). |
| [Umpteen](https://umpteen.gg) (private) | Hub of 90+ daily puzzle and trivia games (word, geography, logic, history) with streaks, stats, and spoiler-free sharing. Each game follows a written spec with automated tests and fact-checked content, and standouts such as [Guess the Year](https://guesstheyear.gg) have their own sites. Built as static JavaScript web apps on Cloudflare Pages. |
| Project Finance (private) | Private side-project financial ledger and cost-attribution workspace: bank and card CSV import, receipt and invoice matching, reviewed-record exports, and provider-level AI cost tracking across OpenAI, Anthropic, and ElevenLabs. Built with FastAPI and SQLite. |

## Multi-Agent Research Workflow

How the Investing Workspace runs, at a high level:

- **Fundamental research.** Thesis-driven, falsifiable cases built from filings, transcripts, and broker research. Each issuer has a living dossier, coverage moves through a tiered funnel from light screen to deep study, and every decision is tested against an explicit return hurdle at a verified price.
- **Quantitative research.** A code-and-test library in which hypotheses and trials are logged before results count as evidence. The trial ledger is frozen and hash-checked to keep multiple testing honest, strategies are tracked forward out of sample, data limits are documented alongside results, and nothing trades live.
- **Coordination.** Agents work in separate lanes with append-only records. Work moves from draft to reviewed to canonical only after another agent independently checks it, and disagreements are logged with both positions preserved.
- **Technology.** Python tooling, Git, Markdown, CSV, and JSON ledgers, Claude, Codex, and other LLM agents, and market data from ThetaData, FMP, Alpha Vantage, and SEC EDGAR.

## Technical Focus

- Systematic trading and investment research: equity screening, factor models, valuation (DCF, comps), and scenario analysis
- Market data and fundamentals pipelines pulling from sources like FMP, Alpha Vantage, SEC EDGAR, FRED, and ThetaData
- Multi-agent research workflows with deterministic checks, evaluation paths, and operator visibility
- LLM engineering: schema-validated tool use, retrieval over primary documents, builder and critic loops, offline evaluation harnesses, and cost-aware model routing with provider failover
- Optimization and applied ML beyond markets: mixed-integer policy search, hedonic and tree-based valuation models, simulation-driven optimization, and computer vision for pose and event detection
- Voice and audio AI pipelines: speech synthesis (ElevenLabs, OpenAI TTS), on-device speech recognition (Apple Speech), broadcast loudness mastering, and automated media production
- Python backends built with FastAPI and data-heavy ingestion or orchestration workflows
- Full-stack applications in React and TypeScript, plus native iOS in SwiftUI (SwiftData, AVFoundation, Speech, watchOS) and cross-platform mobile in React Native
- Cloud deployment on Render, Cloudflare, Vercel, Fly.io, Supabase, and GCP, with CI-gated releases

## Current Focus

- Agent-driven equity research that produces structured, lineage-tracked memos rather than static dashboards
- Systematic strategies and portfolio construction grounded in reproducible, explainable analysis
- Evidence-grounded AI features: retrieval over primary documents, reviewer loops, and out-of-sample measurement before anything ships
- Taking consumer iOS apps (Fortior, CYPHER, Thoughtbound) from prototype toward App Store release
- Decision-support software that turns market analysis into structured, actionable output

## Working Style

I build investment and trading tools that are grounded in real research workflows, explainable under pressure, and engineered to move cleanly from prototype to operational software.

## Contact

If you are building in systematic trading, investment research, fintech, or decision-support tooling, feel free to reach out at [jaredecohen17@gmail.com](mailto:jaredecohen17@gmail.com).
