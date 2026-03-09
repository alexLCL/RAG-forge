# RAGForge - Production-Grade Retrieval-Augmented Generation System

**A scalable, traceable, enterprise-ready RAG knowledge base Q&A engine with high accuracy and extensibility.**
<image alt="Architecture-en" src="./images/RAG-forge.png" ></image>
<details>
<summary>中文版（简体中文） - Chinese (Simplified)</summary>

# RAGForge - 生产级检索增强生成知识库问答系统

**一个可扩展、可溯源、高准确率的企业级 RAG 智能问答引擎。**

RAGForge 基于先进检索增强生成（RAG）技术，提供可靠的生产级知识库问答，支持复杂文档理解、精准检索、 grounded 生成和全程溯源。适用于企业知识管理、智能客服、合规问答、内部协作等场景。

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-powered-009688?logo=fastapi)](https://fastapi.tiangolo.com/)
[![LangChain](https://img.shields.io/badge/LangChain-powered-FF6B6B?logo=langchain)](https://www.langchain.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<image alt="Architecture-zh" src="./images/architecture-zh.jpeg" ></image>

## 🎯 项目定位

RAGForge 面向团队和企业，提供**高准确率、全程可溯源、可大规模扩展**的知识库智能问答系统。融合业界领先 RAG 架构与生产级工程实践，适合知识管理、智能客服、合规/法律/金融问答等业务场景。

## 🏗 架构概览

- **前端** — Pure-Admin-Thin Vue：文档上传、交互问答、来源溯源展示。
- **后端 API** — FastAPI：高性能异步接口，支持多用户角色权限控制。
- **文档处理** — LlamaIndex：智能语义分块、表格/代码块识别。
- **向量存储** — Chroma：本地持久化、增量索引、批量 embedding、快速更新。
- **检索与生成** — LangChain 编排：混合检索、Query Rewrite、Rerank、重排序。
- **安全运维** — API 限流、XSS/SQL 防护、IP 黑名单、企业日志审计，全参数 .env 配置。
<image alt="QA" src="./images/QA.png" ></image>

<image alt="user-manage" src="./images/user-manage.png" ></image>

<image alt="documents-manage" src="./images/documents-manage.png" ></image>

<image alt="upload-document" src="./images/upload-document.png" ></image>

<image alt="rbac-permission" src="./images/rbac.png" ></image>

## ✨ 功能亮点

- **智能语义分块** — 自动识别表格/代码块，适配复杂文档。
- **Query Rewrite** — 查询改写，提升召回与相关性。
## ✨ 功能亮点

- **智能语义分块** — 自动识别表格/代码块，适配复杂文档。
- **Query Rewrite** — 查询改写，提升召回与相关性。
- **Rerank 重排序** — 优先展示最相关 chunk。
- **混合检索** — 语义向量 + 关键词覆盖更全面。
- **增量索引更新** — 文档增删无需全量重建。
- **全程溯源** — 答案带文件、页码、chunk 来源。
- **多用户 RBAC** — 企业级权限协作。
- **生产安全** — 限流、输入防护、IP 黑名单。
- **企业日志** — JSON 结构化 + 轮转，便于审计。
- **RAGAS 评测** — 与生产环境一致，结果真实。
- **灵活配置** — 多模型、多场景快速切换。

## 💡 解决的行业痛点

- 传统检索准确率低、答案无出处 → 难以信任。
- 文档更新慢 → 全量重建索引影响业务。
- 复杂查询召回差 → 答案相关性不足。
- 多用户/合规场景安全需求无法满足。
- 评测与生产不一致 → 决策风险高。

## 🔧 高可扩展性

- **模型相关关** — 轻松切换 LLM/Embedding。
- **配置驱动** — 分块/检索/生成参数 .env 一键调。
- **模块化设计** — 便于二次开发与集成。
- **前后端分离** — 支持多端接入/定制。

## 🚀 应用场景

- 企业知识库与智能问答。
- 客服自动化与业务流程优化。
- 合规、法律、金融高溯源场景。
- 内部文档检索与团队协作。

## 🤝 合作与定制开发

需要定制 RAG 系统、技术咨询、部署指导或完整项目合作？  
欢迎通过以下方式联系：

- **GitHub Issues** 或 Discussions
- **Upwork** → [contact](upwork.com/freelancers/~018e1ea2502904a819)
- **LinkedIn** → [contact](www.linkedin.com/in/changliang-liu-05b974111
)

如果这个展示对你有帮助，欢迎 Star ⭐
</details>

RAGForge delivers reliable, production-grade intelligent question-answering powered by advanced Retrieval-Augmented Generation (RAG). It supports complex document understanding, precise retrieval, grounded generation, and full traceability — ideal for enterprise knowledge management, smart customer service, compliance Q&A, and internal collaboration.

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-powered-009688?logo=fastapi)](https://fastapi.tiangolo.com/)
[![LangChain](https://img.shields.io/badge/LangChain-powered-FF6B6B?logo=langchain)](https://www.langchain.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🎯 Project Positioning

RAGForge is designed for teams and enterprises needing **high-accuracy, fully traceable, and scalable** knowledge base Q&A. It combines state-of-the-art RAG techniques with production engineering best practices — perfect for knowledge management, intelligent customer support, regulatory/compliance Q&A, and secure internal search.

## 🏗 Architecture Overview

- **Frontend** — Pure-Admin-Thin Vue: Clean UI for document upload, interactive Q&A, source tracing display.
- **Backend API** — FastAPI: High-performance, async-ready endpoints with multi-user role-based access control.
- **Document Processing** — LlamaIndex: Intelligent semantic chunking, table/code block recognition for complex docs.
- **Vector Store** — Chroma: Persistent local storage, incremental indexing, batch embedding, fast updates.
- **Retrieval & Generation** — LangChain orchestration: Hybrid search (vector + keyword), Query Rewrite, Rerank, grounded answers.
- **Security & Ops** — Rate limiting, XSS/SQL injection protection, IP blacklist, enterprise logging & auditing, all configurable via `.env`.

## ✨ Key Features & Highlights

- **Intelligent Semantic Chunking** — Auto-detects tables, code blocks; adapts to complex document structures.
- **Query Rewrite** — Automatically refines user queries for better recall and relevance.
- **Rerank** — Re-orders retrieved chunks to prioritize most relevant content.
- **Hybrid Retrieval** — Combines semantic vectors + keyword search for comprehensive coverage.
- **Incremental Indexing & Updates** — Add/delete documents without full re-indexing.
- **Full-Chain Traceability** — Every answer includes source file, page, chunk — transparent and auditable.
- **Multi-User RBAC** — Role-based permissions for enterprise collaboration.
- **Production Security** — API rate limiting, input sanitization, IP blocking.
- **Enterprise Logging** — Structured JSON logs with rotation for ops and compliance.
- **RAGAS Evaluation** — Production-consistent metrics for reliable benchmarking.
- **Flexible Configuration** — Switch LLMs/embeddings, adjust chunking/retrieval params via `.env`.
<image alt="QA" src="./images/QA.png" ></image>

<image alt="user-manage" src="./images/user-manage.png" ></image>

<image alt="documents-manage" src="./images/documents-manage.png" ></image>

<image alt="upload-document" src="./images/upload-document.png" ></image>

<image alt="rbac-permission" src="./images/rbac.png" ></image>
## 💡 Industry Pain Points Solved

- Low accuracy & no source citation → untrustworthy answers.
- Slow updates → full re-indexing disrupts business.
- Poor recall on complex queries → irrelevant or incomplete responses.
- Security/compliance gaps → unsuitable for regulated industries.
- Evaluation mismatch → lab results ≠ production reality.

## 🔧 High Extensibility

- **Model Agnostic** — Plug in any LLM/Embedding (OpenAI, local, fine-tuned).
- **Config-Driven** — All core params (chunk size, retrieval k, rerank threshold) adjustable in `.env`.
- **Modular Design** — Easy to extend retrieval, generation, or UI components.
- **Frontend-Backend Separation** — Supports multi-client integration (web, mobile, API).

## 🚀 Application Scenarios

- Enterprise knowledge bases & internal smart search.
- Automated customer support & business process Q&A.
- Compliance, legal, finance — high-traceability scenarios.
- Team collaboration & document discovery.

## 🤝 Collaboration & Custom Development

Need a tailored RAG system, technical consulting, deployment help, or full project integration?  
Reach out via:

- **GitHub Issues** 或 Discussions
- **Upwork** → [contact](upwork.com/freelancers/~018e1ea2502904a819)
- **LinkedIn** → [contact](www.linkedin.com/in/changliang-liu-05b974111
)


Star ⭐ if this resonates — happy to discuss ideas!

