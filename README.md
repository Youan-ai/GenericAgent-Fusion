# GenericAgent-Fusion

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://python.org)

A generic agent fusion framework that combines multiple AI agent capabilities into a unified system. Designed for extensibility and modular composition.

通用智能体融合框架，将多种AI智能体能力融合为统一系统。设计注重可扩展性和模块化组合。

## Quick Start

```bash
pip install genericagent-fusion
from fusion import AgentFusion
agent = AgentFusion()
```

## Core API

- `AgentFusion()` - Create a fused agent with multiple capabilities
- `.register(agent_type, config)` - Register a new agent type
- `.dispatch(task)` - Dispatch tasks to the appropriate agent(s)
- `.aggregate(results)` - Aggregate results from multiple agents

## Features

- 🔀 **Multi-Agent Fusion** - Combine diverse AI agents seamlessly
- 🧩 **Plugin Architecture** - Easy to extend with custom agents
- ⚡ **Smart Routing** - Automatic task dispatch to best-suited agent
- 🔄 **Result Aggregation** - Intelligent merging of agent outputs

## License

Apache 2.0
