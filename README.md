# GenericAgent Fusion

> 自进化Agent引擎 — 任务完成自动结晶为可复用技能

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

基于 [GenericAgent](https://github.com/lsdefine/generic-agent) (8.8K★) 核心设计理念，
融合GEP基因编码、FTS5语义搜索、成功次数加权检索等增强。

## 核心架构

### L0-L4 分层记忆
```
L0: 上下文窗口 (当前会话)
L1: 工作记忆 (当前任务)
L2: 短期记忆 (当前session)
L3: 长期记忆 (跨session)
L4: 元记忆 (技能+模式)
```

### 9个原子工具
- code_run — 代码执行
- file_read — 文件读取
- file_write — 文件写入
- file_patch — 精准代码修改
- web_scan/js — 网页抓取
- ask_user — 用户交互
- checkpoint — 检查点管理
- long_term_update — 长期记忆更新

### GEP基因编码
任务结晶后的技能被编码为Gene胶囊：
- 技能ID + 变异历史
- 进化轨迹追踪
- 成功率加权检索

### 双重搜索策略
- 关键词匹配 (FTS5)
- 向量语义搜索 (hash嵌入 + 余弦相似度)
- 0.7语义 + 0.3成功率的加权排序

## 安装

```bash
git clone https://github.com/Youan-ai/GenericAgent-Fusion.git
cd GenericAgent-Fusion
pip install -e .
```

## 快速开始

```python
from generic_agent import Agent, Memory

# 创建Agent
agent = Agent()

# 执行任务 — 完成后自动结晶为技能
result = agent.run("计算斐波那契数列第20项")

# 下次类似任务可以直接复用结晶技能
```

## 关联项目

- [LightAgent-Enhanced](https://github.com/Youan-ai/LightAgent-Enhanced) — 零依赖轻量Agent框架
- [佑安AI](https://github.com/youan-ai) — 12引擎驱动的自进化AI助手

## 许可证

MIT License

---

*隶属于 [佑安](https://github.com/youan-ai) AI助手体系 — 从代码中自我进化，利滚利式成长*
