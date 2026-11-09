# Hussein Gamal

**Senior Irrigation & Landscape Engineer · Cost Estimation · Riyadh, Saudi Arabia**

I'm a practising engineer who builds AI agents for my own estimation and design work. Most of that work comes back to one question:

> **How do I trust a number an LLM gives me?**

In cost estimation, a wrong quantity or price means lost money. So I build agents where a wrong number is **visible**, **measurable**, and **stoppable**.

---

## ⭐ Featured: [hussein-agent](https://github.com/husseingamalsa350-rgb/hussein-agent)

A verifiable, tool-using LLM agent for irrigation and landscape engineering: hydraulic design, quantity take-off, and cost estimation. This is the public copy of my private, daily-use system, with company data and the knowledge base removed.

| How it stays trustworthy | What it does |
|---|---|
| **Number-provenance verifier** | Every price or quantity in a reply must trace back to a source: the user's message, an attachment, retrieved memory, or a tool result. If a number has no source, the model is asked again to get it with a tool. If it still has none, the reply shows a ⚠ warning and the case is logged as an improvement ticket. The check is deterministic and needs no second model call. |
| **Evaluation harness** | A domain exam with reference answers and rubrics (300+ questions in the private version). It runs nightly and tracks pass rate, latency, and tokens across model and configuration changes. |
| **Human approval gate** | Any tool action that isn't read-only waits in an approval queue until I confirm it. |
| **Self-review loop** | Failures and unverified claims become tickets. New tools run in a separate process and are installed only after approval, and they can be rolled back. |
| **Context management** | Older turns get summarized while number lines are kept, retrieval is sized to the context that's left, and old tool outputs are trimmed. |

**Stack:** Python · Flask · Qwen3 via Ollama (local) · Gemini and Groq (hosted) · bge-m3 + BM25 hybrid RAG · MCP server · Telegram · WhatsApp · Excel add-in · 31 domain tool modules · 60 test modules

---

## Also running in the private version

- **24/7 cloud knowledge shift with Claude.** A scheduled GitHub Actions pipeline. Every run, Claude picks the next topic from a queue, writes a knowledge file, reviews it, and commits it to the agent's knowledge base. I add a whole course and it gets worked through lesson by lesson. A 15-lesson course on cost estimation and tendering was finished in one day. Built-in rules: no real prices, uncertain figures are marked *approximate*, and every file ends with a "common mistakes" section.
- **Civil 3D grading automation.** Grading sheets with FPL/SOIL levels on islands, existing-ground fallback for stations outside the surface, slope arrows aligned to curbs, and level-label placement, all covered by tests.

---

## Domain
`Irrigation hydraulics` · `Pump stations & smart controllers` · `Landscape & softscape` · `Quantity surveying` · `Cost estimation & tendering` · `Civil 3D`

مهندس ري ولاندسكيب وتسعير في الرياض، وببني وكلاء ذكاء اصطناعي كل رقم بيقولوه لازم يكون له مصدر.
