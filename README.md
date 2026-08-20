# Hi, I'm Night 👋

**AI Engineer — LLM applications, RAG pipelines, and agentic systems.**

Civil engineer turned AI engineer. I build systems where model output has to hold up under
scrutiny: document extraction that feeds payroll, agents that pause for human approval before
acting, retrieval chains that stay grounded in a real knowledge base.

Most of my production work lives in a private client repository. What's here is the public
half — the projects where I was working out how agents, tools, and retrieval actually fit
together.

📫 **atichat.cs@gmail.com** · 📍 Bangkok, Thailand

---

## What I'm working on

🔭 Shipped a staff-operations platform for a Thai restaurant chain — solo build, six weeks,
covering attendance, scheduling, payroll, inventory, and HR. Its AI layer turns supplier
invoice photos, delivery-platform CSVs, and purchase PDFs into typed database rows using
schema-constrained structured output. Because that data feeds payroll, the model never writes
to the database: it parses only and returns a preview a human reviews, while a separate
permission-fenced procedure performs the write.

🌱 Currently going deeper on multi-agent orchestration, evaluation, and MCP integrations.

---

## Tech Stack

**LLM & Agents**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white)
![CrewAI](https://img.shields.io/badge/CrewAI-FF5A50?style=for-the-badge&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=claude&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Data & Storage**

![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B4A?style=for-the-badge&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

**Languages & Tooling**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=for-the-badge&logo=gradio&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

## Projects

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

### 👤 [twin](https://github.com/NakitaDev/twin)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![No Framework](https://img.shields.io/badge/no_framework-by_design-6B7280?style=flat-square)

A digital-twin chatbot built deliberately without an agent framework — raw HTTP requests and
hand-rolled tool handling. I built it this way on purpose: it's easier to reason about what an
agent framework is doing for you once you've written the loop yourself.

---

*Open to AI Engineer roles and freelance work in Thailand.*
