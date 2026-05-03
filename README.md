# GenericAgent-Fusion

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://python.org)
[![GitHub stars](https://img.shields.io/github/stars/youan-ai/GenericAgent-Fusion)](https://github.com/youan-ai/GenericAgent-Fusion)

A self-evolving agent framework with skill crystallization. Combines multiple AI agent capabilities into a unified, extensible system with automatic skill extraction and knowledge transfer between agents.

自进化智能体融合框架，具有技能结晶能力。将多种AI智能体能力融合为统一可扩展系统，支持自动技能提取和跨智能体知识迁移。

## Quick Start

```bash
pip install genericagent-fusion
```

```python
from fusion import AgentFusion
agent = AgentFusion()
agent.register("assistant", AssistantAgent())
result = agent.dispatch("Hello!")
```

## Core API

| Method | Description |
|--------|-------------|
| `AgentFusion()` | Create a fused agent with multiple capabilities |
| `agent.register(name, agent_instance)` | Register a new agent type into the fusion system |
| `agent.dispatch(task)` | Automatically route task to the best-suited agent |
| `agent.crystallize()` | Extract and crystallize reusable skills from interactions |

## Features

- 🔀 **Multi-Agent Fusion** - Seamlessly combine diverse AI agents
- 💎 **Skill Crystallization** - Auto-extract reusable skills from agent interactions
- 🧩 **Plugin Architecture** - Easy to extend with custom agent implementations
- 🔄 **Knowledge Transfer** - Cross-agent learning and capability sharing

## License

Apache 2.0. See [LICENSE](LICENSE) for details.
