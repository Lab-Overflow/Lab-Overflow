## Abstract

<!-- Streak Stats -->
<p align="center">
  <img src="https://streak-stats.demolab.com/?user=Lab-Overflow&theme=github-dark&hide_border=true" alt="GitHub Streak" width="100%" />
</p>

<!-- Activity Graph -->
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Lab-Overflow&theme=github-compact" width="100%" />
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
  <img src="https://img.shields.io/badge/Frontend-React%20%2B%20Three.js%20%2B%20WebGL-61DAFB?style=flat-square&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/Backend-FastAPI%20%2B%20Node.js-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/AI%20Agent-GPT%20%2B%20MCP%20Tool%20Use-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/3D-Three.js%20%2B%20WebGL-000000?style=flat-square&logo=threedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-MySQL%20%2B%20Persistent%20Storage-4479A1?style=flat-square&logo=mysql&logoColor=white" />
</p>

A fullstack AI health platform built from scratch — independently designed, developed, and deployed.

- **AI Agent Integration** — Built-in AI assistant powered by LLM with MCP tool-use capabilities, enabling natural language interaction with platform features
- **Web3D Interactive UI** — Three.js + WebGL rendering for immersive 3D visual experiences in the browser
- **Full User System** — Email verification, account management, and community comment system with database persistence
- **End-to-End Delivery** — From UI design, backend API, database architecture to production deployment — solo fullstack delivery

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
| [prompt-optimizer-lite](https://github.com/Lab-Overflow/prompt-optimizer-lite) | Lightweight prompt optimization toolkit | `262 ⭐` |

## Tech Focus

**AI Agent & Multi-Agent**
`LangChain` `LangGraph` `Dify` `MCP Protocol` `ReAct` `Function Calling` `Prompt Engineering` `Context Engineering` `Agentic Automation` `Multi-Agent Orchestration`

**RAG & Intelligent Query**
`Text2SQL` `NL2SQL` `NL2Data` `Vector Retrieval` `Hybrid Retrieval` `Query Rewrite` `Knowledge Base` `ETL Pipeline` `Structured Output` `JSON Schema`

**AI Infra & Model Engineering**
`PyTorch` `Transformers` `LoRA` `QLoRA` `SFT` `DPO` `DeepSpeed` `Distributed Training` `Mixed Precision` `Gradient Checkpointing` `Ollama` `OpenAI Compatible API` `Model Serving`

**Fullstack & DevOps**
`React` `TypeScript` `FastAPI` `Node.js` `Three.js` `WebGL` `MySQL` `Docker` `Kafka` `Nginx` `CI/CD` `GitHub Actions`
