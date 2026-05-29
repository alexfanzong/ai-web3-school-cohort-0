# Week 2 Note: AI x Web3 Project Breakdown

Status: ready to submit.

## Draft

This note breaks down two AI x Web3 projects:

- Giza / ARMA
- Virtuals Protocol

I chose them because they are not only using AI and tokens as a narrative. Both projects are trying to answer a more concrete question: **when AI agents start to perform economic actions, how should permissions, funds, settlement, and verifiable records be designed?**

## Object 1: Giza / ARMA

### What problem is it solving?

Giza / ARMA focuses on a real DeFi problem: yield opportunities are fragmented, market conditions change quickly, and most users cannot monitor or rebalance positions continuously.

Instead of asking users to manually compare yields across protocols such as Aave, Morpho, Compound, and Moonwell, ARMA aims to let an automated agent monitor stablecoin yield opportunities and rebalance within the user's authorized scope.

My understanding is that the core problem is: **DeFi has many opportunities, but users need a safer way to delegate continuous execution to an automated system.**

### What is the AI part?

The AI / agent part includes:

- Monitoring yield opportunities across multiple DeFi protocols.
- Evaluating APR, protocol rewards, ecosystem rewards, transaction costs, and rebalancing conditions.
- Deciding whether funds should be reallocated according to a strategy.
- Giving users an agent-style interface for managing DeFi yield more naturally.

In this case, AI does not have to mean a fully open-ended LLM. A more accurate description is that ARMA is an on-chain capital agent with an objective function: optimize stablecoin yield while managing execution cost and risk.

### What is the Web3 part?

The Web3 part includes:

- Users connect and activate the agent through a wallet.
- Assets and permissions are managed through a self-custodial smart account.
- Session keys give the automation flow limited permissions.
- The agent interacts with DeFi protocols on chains such as Base and Mode.
- Users keep control of their funds and should be able to revoke permissions or exit.

The most important design choice is the combination of smart accounts and session keys. It separates "the AI can take limited actions" from "the AI has unlimited control over user assets."

### Verifiable materials

- Giza documentation: https://docs.gizatech.xyz/
- ARMA overview: https://giza.mintlify.app/docs/overview
- ARMA agent components: https://giza.mintlify.app/docs/agent-components
- Giza GitHub organization: https://github.com/gizatechxyz
- ARMA app: https://arma.xyz/

### My judgment and questions

Giza / ARMA has a clear value proposition. It does not only say "AI agents will change finance." It chooses a concrete entry point: stablecoin yield optimization.

The main lesson for me is that AI x Web3 is not only about whether an agent can analyze information. The harder question is whether the agent's execution permissions can be productized safely.

Important questions:

- Can the agent receive only the minimum permissions needed for the task?
- Can the user revoke permissions at any time?
- What happens if market conditions change suddenly or the strategy fails?
- Does the user understand the risks behind an apparently simple "higher yield" interface?

My remaining question is how ARMA should prove performance in a trustworthy way. Showing a yield number is not enough. A stronger proof should include risk-adjusted returns, rebalancing history, failure cases, permission scope, drawdown, and whether users truly understand what session keys allow.

## Object 2: Virtuals Protocol

### What problem is it solving?

Virtuals Protocol focuses on a different problem: if AI agents become economic participants, they need ways to be discovered, hired, owned, incentivized, paid, and audited.

It is not only building one agent. It is trying to build an agent economy where agents can produce services, become tokenized, earn revenue, and participate in agent-to-agent or human-to-agent commerce.

My understanding is that the core problem is: **if agents can do useful work independently, they need composable infrastructure for coordination, ownership, incentives, and settlement.**

### What is the AI part?

The AI part includes:

- Autonomous agents that can produce services or products.
- Human-facing interface agents such as Butler, which translate user intent into tasks inside an agent supply chain.
- GAME and related agentic tooling that help builders create and deploy agents.
- Agent-to-agent discovery, coordination, and task execution.

This AI layer is more about application-level agents and coordination than about one specific model.

### What is the Web3 part?

The Web3 part includes:

- Agent tokenization, which lets an agent or AI-native business organize capital and incentives around a token.
- `$VIRTUAL` as a base liquidity pair and medium of exchange inside the ecosystem.
- Agent Commerce Protocol (ACP), which supports discovery, hiring, payment, and transaction records between agents.
- On-chain records for settlement, auditability, and accountability.

The key Web3 idea is that an agent is not only a software feature. It can become an on-chain economic object with ownership, revenue, incentives, and transaction history.

### Verifiable materials

- Virtuals Protocol whitepaper: https://whitepaper.virtuals.io/
- Virtuals Protocol FAQ: https://whitepaper.virtuals.io/info-hub/virtuals-protocol-faq
- Agent Commerce Protocol: https://whitepaper.virtuals.io/about-virtuals/agent-commerce-protocol-acp
- Virtuals app: https://app.virtuals.io/
- GAME documentation: https://docs.game.virtuals.io/

### My judgment and questions

Virtuals is interesting because it frames AI agents as economic actors, not only tools. This is important for AI x Web3 because Web3 is not mainly about making models smarter. Web3 is stronger at ownership, settlement, incentives, audit trails, and composability.

At the same time, I would be cautious. Agent tokenization can easily mix real proof-of-work with speculation. An agent having a token does not prove that it has sustainable revenue. On-chain transactions also do not automatically prove that the service quality is good.

When evaluating a project like this, I would not only look at attention, token price, or launchpad activity. I would ask:

- Does the agent have real users and real revenue?
- Does the revenue come from real services instead of short-term incentives?
- Can the agent's output be verified?
- Can transaction records be matched with specific tasks and deliverables?
- If the agent causes harm or financial loss, who is responsible?

My biggest question is accountability. AI agents can trade, publish content, recommend strategies, and execute tasks, but the responsibility boundary is still unclear when something goes wrong. For this type of protocol to work long term, agent identity, operator responsibility, user confirmation, dispute handling, and safety limits need to be designed more explicitly.

## Comparison

| Dimension | Giza / ARMA | Virtuals Protocol |
|---|---|---|
| Main problem | Automating DeFi yield management safely | Building an on-chain economy for AI agents |
| AI part | Yield-monitoring and execution agent | Autonomous agents, Butler, GAME, agent coordination |
| Web3 part | Smart accounts, session keys, DeFi protocols, user-controlled funds | Agent tokenization, ACP, $VIRTUAL, on-chain settlement |
| Proof type | Docs, app, GitHub, DeFi protocol interactions | Whitepaper, app, protocol docs, launch mechanisms, on-chain transaction records |
| Strongest insight | Agent permission design matters more than the AI wrapper | Agent economy needs verifiable work, not just tokenized attention |
| Main risk | Automation may hide DeFi and permission risk from users | Tokenization may outrun real agent utility and accountability |

## What I Learned

AI x Web3 projects should be judged by whether both sides are necessary.

In Giza / ARMA, AI is useful because continuous yield monitoring and execution are hard for humans to do manually. Web3 is necessary because the actions involve user assets, smart accounts, session keys, and DeFi protocols.

In Virtuals, AI is useful because agents are meant to provide services and coordinate tasks. Web3 is necessary because the protocol needs open ownership, incentive alignment, settlement, and audit records.

My practical evaluation rule:

- If AI only writes marketing copy, it is not a strong AI x Web3 project.
- If Web3 only adds a token without improving ownership, settlement, access control, or verification, it is not a strong AI x Web3 project.
- A stronger project should show proof-of-work through product usage, public docs, repos, demos, chain records, revenue, or concrete case studies.
- Any workflow touching funds, approvals, agent permissions, user identity, or governance should have explicit human confirmation and revocation paths.

## Public Proof

- Learning repo: https://github.com/alexfanzong/ai-web3-school-cohort-0
- Local note: `submissions/2026-05-28-ai-web3-project-breakdown.md`
