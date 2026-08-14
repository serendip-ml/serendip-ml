# Production AI agent infrastructure

**AI is systems engineering.** The hardest part of production AI agents is the infrastructure around the models: off-LLM guarantees, verification loops, response guards, per-role model routing.

---

**Live products:**
- 📰 [news.llm-works.ai](https://news.llm-works.ai): AI news aggregation across 70+ sources with theme clustering, daily digests, and persona-based presentation
- 🔬 [xray.llm-works.ai](https://xray.llm-works.ai): Decision-grade deep research with calibrated verdicts through adversarial + hypothesis + grader verification loops, plan-as-protagonist architecture, knowledge-graph synthesis

---

## Open substrate stack

| Package | What it does |
|---------|--------------|
| [llm-gent](https://github.com/llm-works/llm-gent) | Trait-based agent framework with production HTTP runtime |
| [llm-saia](https://github.com/llm-works/llm-saia) | Verb-vocabulary LLM interaction (ask · verify · critique · refine · ...) |
| [llm-kelt](https://github.com/llm-works/llm-kelt) | Persistent memory + embeddings + LoRA/DPO adapter training (Postgres+pgvector) |
| [llm-infer](https://github.com/llm-works/llm-infer) | Unified inference (vLLM · Ollama · native torch), multi-provider client |
| [appinfra](https://github.com/llm-works/appinfra) | Production Python infrastructure (logging · DB · lifecycle) |

~500K lines across all packages. ~1:1 test-to-code ratio. Local Qwen3.5-27B on RTX PRO 6000.

---

→ 📝 [Blog](https://llm-works.ai/blog/)  ·  🌐 [llm-works.ai](https://llm-works.ai)  ·  🏭 [github.com/llm-works](https://github.com/llm-works)
