# ICL Check-In Draft: 2026-05-25

Status: reviewed, ready to submit.

## Draft

今天听了 Toby 关于 Agent Memory 的分享，主题是“如何让 Agent 拥有持续上下文与长期一致性”。对我最有启发的一点是：Agent Memory 不是数据库。数据库关心的是存得准、查得快、不丢数据；但 agent memory 更关心的是选择性遗忘、按相关性召回、允许旧状态被新证据修正。用传统 CRUD 思维理解 memory，反而会低估它作为 AI 原生基础设施的复杂度。

第二个重要收获是 memory 不是单一组件，而是一层从 embedding、向量数据库、RAG、context engineering 到 memory engineering 的能力栈。前面几层解决“怎么存、怎么查”，真正困难的是最上层：谁来写入、什么时候召回、什么时候更新、什么时候忘记。

今天也重新梳理了两组概念：内容维度上的 semantic memory、episodic memory、procedural memory，以及时间维度上的 working memory 和 long-term memory。这两个维度是正交的，不能混在一起。对 Agent 来说，procedural memory 尤其重要，因为它记录的是 agent 学到的 workflow 和 how-to，未来可能成为 agent 自我改进的重要材料。

我自己的理解是：Memory 正在从 feature 变成 infrastructure。当一个能力开始影响 agent 的长期一致性、可追溯性和自我进化，它就不再只是“存一点上下文”，而需要被作为独立基础设施层设计。这个方向对 AI x Web3 也很重要，尤其是强监管、长周期、需要审计和责任边界的场景。

下一步我想继续思考：如果 agent memory 用在合规、跨境交易或 Agentic Commerce 中，哪些内容应该被长期记住，哪些应该过期，哪些需要人工审核后才能进入 durable memory。

## Public Proof

- Learning repo: https://github.com/alexfanzong/ai-web3-school-cohort-0
- Local note: `daily/2026-05-25.md`
