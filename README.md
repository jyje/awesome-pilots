<div align="center">

# jyje/awesome-pilots

🧪 A curated, categorized index of jyje's pilot projects

[English](README.md) · [한국어](README-ko.md)

---

**Found this useful? Please give it a ⭐ — it helps others find it.**

</div>

## Overview

A categorized index of [jyje](https://github.com/jyje)'s `pilot-` prefixed repositories. Each repo is a small, focused experiment validating one specific technology or idea.

## 🤖 Agent & Orchestration

Agent architectures built on LangGraph / LangChain DeepAgents, and MCP (Model Context Protocol) validation.

| Repo | Description | Stack |
|---|---|---|
| [pilot-upstage-solar-open2](https://github.com/jyje/pilot-upstage-solar-open2) | Compares multiple agent harnesses — Claude Code, Hermes Agent, Claude Agent SDK, LangChain DeepAgents, OpenWiki, Grok Build — all running on Upstage Solar Open 2 (250B MoE) under the same conditions | Python 3.13, Solar Open2 |
| [pilot-agent-factory](https://github.com/jyje/pilot-agent-factory) | A pattern for packaging LangGraph sub-agents as standardized, runtime-loadable plugins (entry points and drop-in modes) | LangGraph, Python 3.14 |
| [pilot-deepagents-rubrics](https://github.com/jyje/pilot-deepagents-rubrics) | End-to-end validation of DeepAgents' `RubricMiddleware` (retries until output meets criteria) using Anthropic Claude | LangChain DeepAgents, Claude |
| [pilot-deepagents-dynamic-subagents](https://github.com/jyje/pilot-deepagents-dynamic-subagents) | Verifies that DeepAgents' Dynamic Subagents delegation works with an NVIDIA NIM backend | DeepAgents, NVIDIA NIM |
| [pilot-langchain-remotegraph](https://github.com/jyje/pilot-langchain-remotegraph) | A CLI that checks whether LangGraph's `RemoteGraph` truly interoperates with three self-hosted, Agent-Protocol-compatible backends (aegra, open-langgraph-platform, etc.) | LangGraph, Agent Protocol |
| [pilot-langgraph-mcp-cli](https://github.com/jyje/pilot-langgraph-mcp-cli) | A LangGraph-based chatbot CLI with MCP (Model Context Protocol) tool support | LangGraph, OpenAI API, MCP |
| [pilot-deepagents](https://github.com/jyje/pilot-deepagents) | A basic example following the official LangChain DeepAgents docs (OpenAI-compatible API) | LangChain DeepAgents |
| [pilot-fastmcp](https://github.com/jyje/pilot-fastmcp) | A pilot project for FastMCP | FastMCP |

## 📚 RAG & Vector Search

RAG pipelines and vector search / visualization experiments.

| Repo | Description | Stack |
|---|---|---|
| [pilot-onpremise-rag](https://github.com/jyje/pilot-onpremise-rag) (`pirag`) | An LLM+RAG CLI designed to run in on-premise environments, published as a PyPI package | LangChain, Milvus, MinIO, Typer |
| [pilot-langchain-pgvector](https://github.com/jyje/pilot-langchain-pgvector) | An example of storing documents and running similarity search with pgVector + LangChain | PostgreSQL/pgVector, LangChain, Docker Compose |
| [pilot-vector-tsne](https://github.com/jyje/pilot-vector-tsne) | Visualizes high-dimensional vectors stored in Milvus using t-SNE | t-SNE, Milvus |
| [pilot-chainlit-rag](https://github.com/jyje/pilot-chainlit-rag) | A Chainlit-based RAG pilot | Chainlit |

## ☁️ Infra & DevOps

Deployment infrastructure, micro-frontends, and MLOps pipeline validation.

| Repo | Description | Stack |
|---|---|---|
| [pilot-module-federation](https://github.com/jyje/pilot-module-federation) | An AI platform shell comparing Vue 3 and Next.js over HTTP Module Federation, validating independently deployable, team-owned micro frontends | Vue 3, Next.js, Module Federation, Fastify |
| [pilot-mlops-cicd](https://github.com/jyje/pilot-mlops-cicd) | A reference implementation of a cloud-native MLOps pipeline, from model training to serving | NVIDIA Triton, Kubernetes, GitHub Actions |
| [pilot-gitops-argocd](https://github.com/jyje/pilot-gitops-argocd) | A GitOps / ArgoCD pilot | ArgoCD |

## 🧪 LLM Basics & Model Experiments

Minimal setups for running LLMs on a specific runtime or framework, plus miscellaneous tooling pilots.

| Repo | Description | Stack |
|---|---|---|
| [pilot-openai-llm](https://github.com/jyje/pilot-openai-llm) | Basic OpenAI API experiments in a notebook | Jupyter Notebook, OpenAI API |
| [pilot-ollama](https://github.com/jyje/pilot-ollama) | A local LLM pilot using Ollama | Ollama |
| [pilot-pytorch-mps](https://github.com/jyje/pilot-pytorch-mps) | A minimal example verifying PyTorch training on Apple Silicon (MPS), CUDA, and CPU | PyTorch |
| [Pilot.NET.LLM](https://github.com/jyje/Pilot.NET.LLM) | A simple LLM use case built with .NET 9 + Ollama (gemma2, exaone3.5) | C#/.NET 9, Ollama |
| [pilot-slidev](https://github.com/jyje/pilot-slidev) | A Slidev-based presentation tooling pilot (unrelated to LLMs) | Slidev, pnpm |

---

> Summaries are based on each repo's README (English version preferred). Repos with an empty or title-only README (`pilot-fastmcp`, `pilot-gitops-argocd`, `pilot-ollama`, `pilot-openai-llm`, `pilot-chainlit-rag`) were summarized from their GitHub description instead.
