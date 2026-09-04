# Hi, I'm Night 👋

**AI Engineer — LLM applications, RAG pipelines, and agentic systems.**

Civil engineer turned AI engineer. I build systems where model output has to hold up under
scrutiny: document extraction that feeds payroll, agents that pause for human approval before
acting, and serverless AI applications backed by automated Infrastructure-as-Code delivery.

Most of my production work lives in a private client repository. What's here is the public
half — the projects where I was working out how agents, tools, cloud infrastructure, and CI/CD pipelines actually fit together.

📫 **atichat.cs@gmail.com** · 📍 Bangkok, Thailand

---

## Tech Stack

**Frontend & Full Stack**

![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

**LLM & Agents**

![AWS Bedrock](https://img.shields.io/badge/AWS_Bedrock-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white)
![CrewAI](https://img.shields.io/badge/CrewAI-FF5A50?style=for-the-badge&logoColor=white)
![OpenAI Agents SDK](https://img.shields.io/badge/OpenAI_Agents_SDK-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=claude&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6566F1?style=for-the-badge&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Cloud Infrastructure & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Langfuse](https://img.shields.io/badge/Langfuse-000000?style=for-the-badge&logo=langfuse&logoColor=white)

**Backend & Data**

![Python](https://img.shields.io/badge/Python_3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B4A?style=for-the-badge&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)

---

## Projects

### 🤖 [digital-twin](https://github.com/NakitaDev/digital-twin)

![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![AWS Bedrock](https://img.shields.io/badge/AWS_Bedrock-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

An interactive, production-grade AI Digital Twin conversational companion representing me to website visitors and potential employers. Built with Next.js 16 and FastAPI, running on fully serverless AWS infrastructure (CloudFront, S3 static hosting, API Gateway HTTP API, Lambda via Mangum).

Features dual-LLM resilience with AWS Bedrock as primary and OpenRouter as automated fallback, stateful session memory backed by Amazon S3, and dark-mode first UI. Provisioned entirely via Terraform Infrastructure-as-Code with remote S3/DynamoDB state locking and automated multi-environment CI/CD via GitHub Actions using keyless AWS OIDC authentication.

### 🔍 [deep-research-agent](https://github.com/NakitaDev/deep-research-agent)

![OpenAI Agents SDK](https://img.shields.io/badge/OpenAI_Agents_SDK-412991?style=flat-square&logo=openai&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6566F1?style=flat-square&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=flat-square&logo=gradio&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

A multi-agent research pipeline on the OpenAI Agents SDK: a planner turns a question into
search terms with reasoning, searches run in parallel, a writer synthesizes them into a
long-form report, and a final agent delivers it by email or push notification.

The interesting part is that it runs on OpenRouter rather than OpenAI. That meant switching
the SDK to Chat Completions mode and replacing the hosted web-search tool with a direct
Serper call, since OpenRouter supports neither — working out which parts of an agent
framework are provider-agnostic and which are quietly coupled to one vendor.

### 🤖 [langchain-sidekick](https://github.com/NakitaDev/langchain-sidekick)

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=flat-square&logo=gradio&logoColor=white)

A personal assistant agent built on LangChain and LangGraph — a worker agent wrapped in a
homemade evaluator loop that self-checks its answers against user-defined success criteria
before replying. It plans work through a visible todo list, drives a real browser and a
sandboxed filesystem through MCP servers, and pauses for human approval before sensitive
actions.

### 🏗️ [engineering-team](https://github.com/NakitaDev/engineering-team)

![CrewAI](https://img.shields.io/badge/CrewAI-FF5A50?style=flat-square&logoColor=white)
![MCP](https://img.shields.io/badge/Context7_MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

A CrewAI crew that turns plain-English requirements into a working, tested Python application.
Four agents run in sequence — lead, backend, frontend, test — each handing off to the next.
Generated code executes inside an ephemeral Docker container rather than on the host, and the
sandbox is wiped and rebuilt on every run, so the agents only ever have the standard library
plus what I've explicitly installed.

### 🗡️ [hollow-lore-master](https://github.com/NakitaDev/hollow-lore-master)

![LangChain](https://img.shields.io/badge/LangChain%20LCEL-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B4A?style=flat-square&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=claude&logoColor=white)
![Hugging Face](https://img.shields.io/badge/HF_Spaces-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

A retrieval-augmented Q&A chatbot answering open-ended lore questions about Hollow Knight,
grounded in a scraped wiki knowledge base. Covers the full pipeline — scraping, recursive
chunking, embedding generation, and persistence to a vector store (ChromaDB locally, Pinecone
for hosted indexes) — with a history-aware retrieval
chain that reformulates follow-up questions against prior conversation context instead of
treating them as isolated queries.

---

*Open to AI Engineer roles and freelance work in Thailand.*
