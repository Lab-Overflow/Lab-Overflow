## Abstract

<!-- GitHub Insights -->
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Lab-Overflow&show_icons=true&hide_border=true&theme=github_dark&rank_icon=github&include_all_commits=true&count_private=true" width="49%" />
  <img src="https://streak-stats.demolab.com?user=Lab-Overflow&theme=github-dark-blue&hide_border=true&date_format=j%20M%5B%20Y%5D" width="49%" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Lab-Overflow&theme=github_dark" width="100%" />
</p>

<!-- Tech Stack -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=py,ts,js,pytorch,tensorflow,sklearn,fastapi,react,threejs,nodejs,kafka&perline=11" alt="Tech Stack Row 1" />
  <br/>
  <img src="https://skillicons.dev/icons?i=redis,nginx,mysql,docker,kubernetes,githubactions,linux,cloudflare,workers,vscode,grafana&perline=11" alt="Tech Stack Row 2" />
</p>

---

## AI-Powered Calorie Calculator & Health Platform

<p align="center">
  <a href="https://calculatorcaloriefree.com">
    <img src="https://img.shields.io/badge/Live-calculatorcaloriefree.com-00C853?style=for-the-badge&logo=google-chrome&logoColor=white" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React%2019-TypeScript-61DAFB?style=flat-square&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudflare-Pages%20%2B%20Workers%20%2B%20D1%20%2B%20KV-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/AI%20Agent-4%20Modes%20%C2%B7%20Function%20Calling-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/i18n-English%20%2B%20%E4%B8%AD%E6%96%87-2196F3?style=flat-square&logo=googletranslate&logoColor=white" />
  <img src="https://img.shields.io/badge/Automation-LangGraph%20Trigger-1A1A2E?style=flat-square&logo=python&logoColor=white" />
</p>

A fullstack AI health platform independently designed, developed, and deployed — from 0 to 1, solo delivery.

**4 AI Agent Modes**
- `Combination Agent` — Select ingredients + cooking action, AI estimates resulting dish & calories via structured JSON output
- `Cooking Agent` — Autonomous agent: receives customer orders, plans cooking steps, executes 80+ tool-defined actions, manages real-time inventory
- `Verification Agent` — Semantic matching between served dish and original order with confidence scoring
- `Support Agent` — Context-aware Q&A for user guidance and methodology explanation

**Platform Architecture**

```mermaid
flowchart TB
    subgraph Frontend["Frontend Layer"]
        A["Static Site\nHTML / CSS / JS\nCanvas Physics Animation"]
        B["React 19 + TypeScript\nAgent Workspace\n4-Mode Orchestrator"]
    end

    subgraph Backend["Serverless Backend · Cloudflare Functions"]
        C["Auth API\nEmail Verify / Google OAuth\nInvite-Code System"]
        D["Chat Completions Proxy\nModel Locking / Pro Gating\nCost Control"]
        E["Content API\nComments / FAQ Articles\nUser Profiles"]
        F["Middleware\nLocale Routing / CORS\nSession Validation"]
    end

    subgraph Data["Data Layer"]
        G["Cloudflare D1\nUsers / Articles / Profiles"]
        H["Cloudflare KV\nSessions / Cache / Invites"]
    end

    subgraph Auto["Automation Layer · Python"]
        I["LangGraph Trigger\nScheduled Article Ingestion\nMulti-Source Web Search"]
    end

    A <--> |iframe + postMessage| B
    Frontend --> Backend --> Data
    Auto --> E
```

**Key Technical Highlights**
- **Serverless-Native Architecture** — Edge-deployed fullstack application with globally distributed low-latency access
- **AI Agent Orchestration** — Multi-mode agent system with recursive function calling, structured output enforcement, and real-time state management
- **Multi-Layer Auth & Access Control** — Email verification, OAuth integration, invite-code gating, and subscription-based feature access
- **Canvas Physics Engine** — Custom real-time 2D physics simulation with pointer-tracking interaction
- **Bilingual Intelligent Routing** — Automatic locale detection and content switching across the entire platform
- **LangGraph Automation Pipeline** — Scheduled multi-source data aggregation with automated content ingestion

<p align="center">
  <a href="https://calculatorcaloriefree.com"><b>calculatorcaloriefree.com</b></a>
</p>

---

## AI Infra & Distributed Training

<p align="center">
  <img src="https://img.shields.io/badge/Scale-1000%2B%20GPUs-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/DeepSpeed-ZeRO--3-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-Distributed-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Precision-BF16%2FFP16-9B59B6?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Training-LoRA%20%2F%20SFT%20%2F%20DPO-E67E22?style=for-the-badge" />
</p>

```mermaid
flowchart LR
    subgraph Data["Data Pipeline"]
        A["Raw Corpus\n(TB-scale)"] --> B["ETL & Cleaning\nDeduplication"]
        B --> C["Tokenization\n& Sharding"]
    end

    subgraph Cluster["GPU Cluster · 1000+ Cards"]
        D["Job Scheduler\nResource Allocation\nSlurm / K8s"]
        E["DeepSpeed ZeRO-3\nPipeline & Tensor\nParallelism"]
        F["Mixed Precision\nGradient Accumulation\nActivation Checkpointing"]
        D --> E --> F
    end

    subgraph Strategy["Training Strategy"]
        G["SFT\nSupervised\nFine-Tuning"]
        H["LoRA / QLoRA\nParameter-Efficient\nFine-Tuning"]
        I["DPO / RLHF\nAlignment\nOptimization"]
        G --> H --> I
    end

    subgraph Serving["Model Serving"]
        J["FastAPI\nOllama"]
        K["OpenAI\nCompatible API"]
        L["Monitoring\nGPU Util & Throughput"]
        J --> K --> L
    end

    Data --> Cluster --> Strategy --> Serving
```

<p align="center">
  <i>End-to-end LLM training pipeline: from TB-scale data preprocessing to distributed training across 1000+ GPU cluster, through alignment optimization, to production model serving.</i>
</p>

---

## Top Projects

| Project | Description | Stars |
|:--|:--|:--|
| [prompt-optimizer-lite](https://github.com/Lab-Overflow/prompt-optimizer-lite) | Lightweight prompt optimization toolkit | [![GitHub Repo stars](https://img.shields.io/github/stars/Lab-Overflow/prompt-optimizer-lite?style=flat-square)](https://github.com/Lab-Overflow/prompt-optimizer-lite/stargazers) |

## Tech Focus

**AI Agent & Multi-Agent**
`LangChain` `LangGraph` `Dify` `MCP Protocol` `ReAct` `Function Calling` `Prompt Engineering` `Context Engineering` `Agentic Automation` `Multi-Agent Orchestration`

**RAG & Intelligent Query**
`Text2SQL` `NL2SQL` `NL2Data` `Vector Retrieval` `Hybrid Retrieval` `Query Rewrite` `Knowledge Base` `ETL Pipeline` `Structured Output` `JSON Schema`

**AI Infra & Model Engineering**
`PyTorch` `Transformers` `LoRA` `QLoRA` `SFT` `DPO` `DeepSpeed` `Distributed Training` `Mixed Precision` `Gradient Checkpointing` `Ollama` `OpenAI Compatible API` `Model Serving`

**Fullstack & DevOps**
`React` `TypeScript` `FastAPI` `Node.js` `Three.js` `WebGL` `MySQL` `Docker` `Kafka` `Nginx` `CI/CD` `GitHub Actions`
