## 为什么选择长文本：

1 LC 与 RAG 之争作为 motivation 的出发点

2 追热点，新 benchmark 和 paper 层出不穷。

3 LC benchmark 中的 Open－Ended task 任务十分合适，目前 close－ended 的工作已经很多了，但 open 相关的工作比较少，有创新的空间。

4 通过一些外置手段做推理已经比较普遍，比如 CoT、think on graph、interactive promoting 等等；

而利用 KG+一些传统的 NLP 手段算是微软的 GrpahRAG 做的一个新方向（他用到了 community detection 算法）。

o1 可以说是揭开了 post-training 的大幕，现在有很多研究都在尝试通过开源的模型和方法复现 o1 的推理能力。那我更倾向于做一些 post-training 的其他工作。

---

## 科研敏感性：

1 科学问题的发现与概念的定义

retrieve－then-match 是借鉴了 generate－then－ground 的一篇工作。他把常用的 RAG 解决方案概括为“retrieve-then-read“
（ retrieve potential documents from an external corpus to read an answer.）

2 Pipeline 的包装？

选用多智能体 RL 是出于对热点的借鉴，比如 GPTo1，RL+LLM 的工作在 ACL、ICML 也有一些。

多智能体很热，比如 neo4j 说 Agent is the next era，各种关于 agent 的应用和概念也层出不穷。但很多情况下都混淆了 Agent 的概念，尤其是 RL-based 和 LLM-based。我想交叉中做出一点新东西，批判 agent 热潮，抬高自己。也许能引起审稿人的关注。

【Exploring Large Language Model based Intelligent Agents: Definitions, Methods, and Prospects】

如果重点做多智能体的话，可能在代码实现阶段有较大的困难。
