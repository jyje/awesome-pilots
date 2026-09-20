<div align="center">

# jyje/awesome-pilots

🧪 jyje의 pilot 프로젝트를 카테고리별로 정리한 큐레이션 목록

[English](README.md) · [한국어](README-ko.md)

---

**Found this useful? Please give it a ⭐ — it helps others find it.**

</div>

## Overview

[jyje](https://github.com/jyje)의 `pilot-` 접두사 프로젝트와 그 출발점이 되는 템플릿을 카테고리별로 정리한 목록입니다. 각 레포는 특정 기술이나 아이디어를 검증하기 위한 최소 단위 실험(pilot)입니다.

## 🤖 Agent & Orchestration

LangGraph / LangChain DeepAgents 기반 에이전트 아키텍처와 MCP(Model Context Protocol) 검증.

| Repo | 설명 | 스택 |
|---|---|---|
| [pilot-upstage-solar-open2](https://github.com/jyje/pilot-upstage-solar-open2) | Upstage Solar Open 2(250B MoE) 모델 위에서 Claude Code, Hermes Agent, Claude Agent SDK, LangChain DeepAgents, OpenWiki, Grok Build 등 여러 에이전트 하네스를 동일 조건으로 비교 검증 | Python 3.13, Solar Open2 |
| [pilot-agent-factory](https://github.com/jyje/pilot-agent-factory) | LangGraph 서브에이전트를 런타임에 로드 가능한 표준 플러그인 패키지로 만드는 패턴 (entry points / drop-in 두 방식) | LangGraph, Python 3.14 |
| [pilot-deepagents-rubrics](https://github.com/jyje/pilot-deepagents-rubrics) | DeepAgents의 `RubricMiddleware`(기준을 만족할 때까지 재시도하는 미들웨어)를 Anthropic Claude로 end-to-end 검증 | LangChain DeepAgents, Claude |
| [pilot-deepagents-dynamic-subagents](https://github.com/jyje/pilot-deepagents-dynamic-subagents) | DeepAgents의 Dynamic Subagents 위임 기능이 NVIDIA NIM 백엔드에서도 동작하는지 검증 | DeepAgents, NVIDIA NIM |
| [pilot-langchain-remotegraph](https://github.com/jyje/pilot-langchain-remotegraph) | LangGraph `RemoteGraph`가 self-hosted Agent Protocol 호환 백엔드(aegra, open-langgraph-platform 등) 3종과 실제로 상호운용되는지 검증하는 CLI | LangGraph, Agent Protocol |
| [pilot-langgraph-mcp-cli](https://github.com/jyje/pilot-langgraph-mcp-cli) | MCP 도구 연동을 지원하는 LangGraph 기반 챗봇 CLI | LangGraph, OpenAI API, MCP |
| [pilot-deepagents](https://github.com/jyje/pilot-deepagents) | LangChain DeepAgents 공식 문서를 따라가는 기본 예제 (OpenAI 호환 API) | LangChain DeepAgents |
| [pilot-fastmcp](https://github.com/jyje/pilot-fastmcp) | FastMCP 파일럿 프로젝트 | FastMCP |
| [pilot-typesafeai-jev](https://github.com/jyje/pilot-typesafeai-jev) | 텍스트 대신 타입이 있는 판단을 돌려주는 TypeSafe AI의 Jev를 LangGraph와 Deep Agents 안에서 라우터, 가드레일, 검증 도구로 활용. 채팅 모델은 ChatGPT 구독, NVIDIA NIM, LM Studio 중에서 고를 수 있음 | LangGraph, Deep Agents, TypeSafe AI Jev |

## 📚 RAG & Vector Search

RAG 파이프라인과 벡터 검색/시각화 실험.

| Repo | 설명 | 스택 |
|---|---|---|
| [pilot-onpremise-rag](https://github.com/jyje/pilot-onpremise-rag) (`pirag`) | 온프레미스 환경에서 동작하는 LLM+RAG CLI. PyPI로 패키지 배포까지 진행 | LangChain, Milvus, MinIO, Typer |
| [pilot-langchain-pgvector](https://github.com/jyje/pilot-langchain-pgvector) | pgVector + LangChain으로 문서 저장 및 유사도 검색을 구현한 예제 | PostgreSQL/pgVector, LangChain, Docker Compose |
| [pilot-vector-tsne](https://github.com/jyje/pilot-vector-tsne) | Milvus에 저장된 고차원 벡터를 t-SNE로 시각화하는 실험 | t-SNE, Milvus |
| [pilot-chainlit-rag](https://github.com/jyje/pilot-chainlit-rag) | Chainlit 기반 RAG 파일럿 | Chainlit |

## 🧰 템플릿

새 pilot을 시작하기 위한 출발점입니다.

| Repo | 설명 | 스택 |
|---|---|---|
| [template-pilot-ai-python](https://github.com/jyje/template-pilot-ai-python) | Python AI pilot용 GitHub 템플릿. uv 앱, ChatGPT 구독과 NVIDIA NIM 공급자, 에이전트 스킬, 4개 언어 문서, CI, 릴리스 워크플로 포함 | Python 3.13, uv, LangGraph |

## ☁️ Infra & DevOps

배포 인프라, 마이크로 프론트엔드, MLOps 파이프라인 검증.

| Repo | 설명 | 스택 |
|---|---|---|
| [pilot-module-federation](https://github.com/jyje/pilot-module-federation) | Vue 3와 Next.js를 HTTP Module Federation으로 비교하는 AI 플랫폼 셸. 팀별 마이크로 프론트엔드가 독립 배포되는 구조를 검증 | Vue 3, Next.js, Module Federation, Fastify |
| [pilot-mlops-cicd](https://github.com/jyje/pilot-mlops-cicd) | 모델 학습부터 서빙까지 클라우드 네이티브 환경의 MLOps 파이프라인 레퍼런스 구현 | NVIDIA Triton, Kubernetes, GitHub Actions |
| [pilot-gitops-argocd](https://github.com/jyje/pilot-gitops-argocd) | GitOps/ArgoCD 파일럿 | ArgoCD |

## 🧪 LLM 기초 & 모델 실험

특정 런타임/프레임워크 위에서 LLM을 최소 구성으로 돌려보는 실험, 그리고 그 밖의 툴링 파일럿.

| Repo | 설명 | 스택 |
|---|---|---|
| [pilot-openai-llm](https://github.com/jyje/pilot-openai-llm) | OpenAI API 기초 실험 노트북 | Jupyter Notebook, OpenAI API |
| [pilot-ollama](https://github.com/jyje/pilot-ollama) | Ollama 로컬 LLM 파일럿 | Ollama |
| [pilot-pytorch-mps](https://github.com/jyje/pilot-pytorch-mps) | Apple Silicon(MPS) / CUDA / CPU 각 환경에서 PyTorch 학습이 동작하는지 검증하는 최소 예제 | PyTorch |
| [Pilot.NET.LLM](https://github.com/jyje/Pilot.NET.LLM) | .NET 9 + Ollama(gemma2, exaone3.5)로 만든 간단한 LLM 유스케이스 | C#/.NET 9, Ollama |
| [pilot-slidev](https://github.com/jyje/pilot-slidev) | Slidev 기반 프레젠테이션 툴링 파일럿 (LLM과는 무관) | Slidev, pnpm |

---

> 각 레포의 README(영문 우선)를 기준으로 요약했습니다. README가 비어 있거나 제목만 있는 레포(`pilot-fastmcp`, `pilot-gitops-argocd`, `pilot-ollama`, `pilot-openai-llm`, `pilot-chainlit-rag`)는 GitHub description으로 대체 요약했습니다.
