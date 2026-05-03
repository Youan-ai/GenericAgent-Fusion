# GenericAgent-Fusion

Self-evolving agent framework with L0-L4 layered memory architecture. Automatically crystallizes task execution paths into reusable skills.

## Features
- L0-L4 hierarchical memory (context → metacognition)
- GEP-inspired gene encoding for skills
- Density maximization protocol (<summary> protocol)
- 9 atomic tools: code_run, file_read/write/patch, web_scan/js, ask_user, checkpoint, long_term_update

## Architecture
```
Task Input → Agent Loop → Tool Execution → Skill Crystallization → Skill Vault
     ↑                                                              ↓
     └────────────────── Reuse on similar tasks ────────────────────┘
```
