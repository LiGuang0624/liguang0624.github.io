#### MemTrace: Automatic Error Tracing and Attribution for LLM Memory Systems
*Core Contributor | Oct 2025 – Feb 2026 | ICLR 2026 (Under Review)* [[arXiv]](https://arxiv.org/abs/2605.28732) [[Code]](https://github.com/zjunlp/MemTrace)

- Built MemTrace, an error tracing and attribution framework for LLM memory systems, and constructed MemTraceBench, the first diagnostic benchmark with 160 real-world failure cases across four mainstream memory systems (Long-Context, RAG, Mem0, EverMemOS).
- Developed the smartcomment tracing toolkit, which transparently records variable- and operation-level information flow and dependencies as executable evolution graphs without rewriting underlying code.
- Proposed the MemTrace algorithm (hybrid retrieval initialization + priority queue) and MemTrace-OBS algorithm (global search) to locate decisive error sets (minimal causal cut sets) for cross-session, multi-stage fault attribution.
- Open-sourced MemTraceBench under MIT license; improved end-to-end downstream task performance by 7.62% via attribution-guided prompt optimization.

#### Fazhitong: Legal Consultation Assistant Based on ReAct Agent and Advanced RAG
*Independent Development | Oct 2024 – Jan 2025*

- Built an intelligent Q&A system for legal consultation based on ReAct Agent + advanced RAG, addressing poor recall in long legal texts and supporting personalized action recommendations based on user case history.
- Implemented BM25 + dense retrieval with BGE-Reranker reranking over a knowledge base of 100K+ legal articles, improving Top-3 retrieval hit rate to 92%.
- Developed a multi-agent collaboration framework with LangGraph, including a Critic Agent for hallucination detection and rewrite, and dynamic routing between legal article retrieval and document generation modes.
- Built a 100-question legal QA test set and evaluated with RAGAS, improving Faithfulness from 0.78 to 0.91.
- Deployed with FastAPI backend and Vue3 streaming chat frontend; encapsulated 5 tool functions with YAML-based decoupled configuration.
