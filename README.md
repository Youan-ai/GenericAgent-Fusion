# 🤖 GenericAgent — Self-Evolving Agent Framework

> **Tasks complete → Skills crystallize automatically. Every execution makes you smarter.**

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.9%2B-brightgreen)](https://python.org)

GenericAgent is a **self-evolving agent loop** (~100 lines of stable kernel) that automatically crystallizes completed tasks into reusable skills. Every task execution leaves behind a skill — making the agent progressively more capable without manual intervention.

---

## ✨ Features

- **Auto-Crystallization** — Task done → skill generated. Zero manual effort.
- **9 Atomic Tools** — code_run, file_read/write/patch, web_scan, ask_user, checkpoint, long_term_update
- **L0-L4 Hierarchical Memory** — Context → Working → Short → Long → Meta, with auto-promotion
- **FTS5 + Semantic Search** — Hybrid retrieval (0.7 semantic + 0.3 success-weight)
- **GEP Gene Encoding** — Each skill is a gene capsule with mutation history and evolution trace

## 📦 Installation

```bash
git clone https://github.com/Youan-ai/GenericAgent-Fusion.git
cd GenericAgent-Fusion
```

## 🚀 Quick Start

```python
from generic_agent import GenericAgent

agent = GenericAgent()

# Agent automatically:
# 1. Receives task → 2. Searches existing skills → 3. Executes → 4. Crystallizes new skill
result = agent.run("Write a Python script to sort files by date")
# A new skill is now available for future tasks!
print(f"Crystallized: {result.skills_created}")
```

## 🏗️ Architecture

```
┌─────────────────────────────────────────────┐
│              GenericAgent Loop                │
├──────────────┬──────────────────────────────┤
│ Execution    │ Crystallization               │
├──────────────┼──────────────────────────────┤
│ receive task │ analyze execution path        │
│ search skills│ extract SOP/pattern           │
│ run tools    │ encode as Gene capsule        │
│ collect      │ store in skill bank           │
│ results      │ update AGENTS.md refs         │
└──────────────┴──────────────────────────────┘
```

## 📚 Memory Hierarchy (L0-L4)

| Level | Name | Capacity | Persistence |
|-------|------|----------|-------------|
| L0 | Context Window | ~session | Session |
| L1 | Working Memory | ~50 items | Task duration |
| L2 | Short-term | ~500 items | Day |
| L3 | Long-term | ~5000 items | Weeks |
| L4 | Meta-memory | Core skills | Permanent |

## 🤝 Contributing

Open issues and PRs welcome!

## 📄 License

Apache 2.0 — see [LICENSE](LICENSE).
