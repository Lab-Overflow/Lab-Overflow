## Abstract

<!-- Trophy Wall -->
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Lab-Overflow&theme=darkhub&title=-Reviews&v=2" alt="Lab-Overflow's Trophies" width="100%" />
</p>

<!-- Streak Stats -->
<p align="center">
  <img src="https://streak-stats.demolab.com/?user=Lab-Overflow&theme=github-dark&hide_border=true" alt="GitHub Streak" width="100%" />
</p>

<!-- GitHub Stats -->
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Lab-Overflow&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&theme=github_dark" alt="Github Stats" width="100%" />
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
