# AI x Web3 Information Flow

Status: ready to submit.

## Source Boundary

I used the course recommendation screenshots and visible X profile/post information as the starting point. I did not include private keys, wallet information, API keys, account credentials, or private course materials.

## Follow List

| Category | Account | X handle | Why I chose it | What I want to observe |
|---|---|---|---|---|
| Course ecosystem | AIxWeb3 School | [@aiweb3school](https://x.com/aiweb3school) | Official course account for bootcamp, hackathon, handbook, and assignment updates. | Course themes, selected projects, builder examples, and how the program frames AI agents, wallets, payments, privacy, and secure execution. |
| Course ecosystem | ETHPanda | [@ETHPanda_Org](https://x.com/ETHPanda_Org) | Chinese-speaking Ethereum builder community and course co-initiator. | Ethereum public-goods activity, Chinese builder opportunities, and how local communities translate Ethereum ideas into builder workflows. |
| Course ecosystem | LXDAO | [@LXDAO_Official](https://x.com/LXDAO_Official) | R&D-driven DAO focused on open-source projects and public goods. | Public-goods funding, builder coordination, open-source sustainability, and AI x Web3 community activities. |
| Course ecosystem | Web3 Career Build | [@web3careerbuild](https://x.com/web3careerbuild) | WCB platform account connected to course tasks and proof-of-work. | Learning tasks, public submissions, internship-style opportunities, and how builders present work publicly. |
| AI / Agent | Z.ai / GLM | [@Zai_org](https://x.com/Zai_org) | Course sponsor and an important AI model/tooling account. | GLM model updates, agentic coding, long-context inference, model/API capabilities, and how AI tooling becomes usable for builders. |
| Wallet / custody / payment | Cobo | [@Cobo_Global](https://x.com/Cobo_Global) | Course sponsor with strong relevance to institutional wallets, MPC, custody, and agentic wallet design. | Wallet security, delegated execution, payment infrastructure, and where human confirmation should remain mandatory. |
| Security | GoPlus Security | [@GoPlusSecurity](https://x.com/GoPlusSecurity) | Relevant to AI security and on-chain risk detection before execution. | Address, contract, approval, signature, and transaction risk checks that could become guardrails for AI agents. |
| AI security / trusted execution | Phala Network | [@PhalaNetwork](https://x.com/PhalaNetwork) | Relevant to TEE, verifiable execution, model hosting, and agent security. | How trusted execution can protect AI agents, model outputs, private data, and delegated workflows. |
| Smart wallet / agent wallet | ELYTRO | [@elytro_eth](https://x.com/elytro_eth) | Account-abstraction and smart-wallet direction closely related to agent wallet design. | Session keys, social recovery, spending limits, permission scopes, and the line between automation and user control. |
| Cross-chain / intent | LI.FI | [@lifiprotocol](https://x.com/lifiprotocol) | Infrastructure for swaps, bridging, and on-chain actions; useful for intent and cross-chain execution. | How intents, routing, stablecoin payments, RWAs, and compliant on-chain liquidity are productized. |
| Privacy | Web3Privacy / W3PN | [@web3privacy](https://x.com/web3privacy) | Privacy research community connected to the course's privacy session. | Privacy culture, anti-surveillance application design, and permission boundaries for AI agents. |
| Chinese builder | Bruce Xu | [@brucexu_eth](https://x.com/brucexu_eth) | Connected to ETHPanda, LXDAO, LI.FI, and AI x ETH builder education. | Chinese Ethereum builder discourse, AI x ETH ideas, public-goods work, and ecosystem opportunities. |
| Ethereum / Web3 expert | Vitalik Buterin | [@VitalikButerin](https://x.com/VitalikButerin) | Core Ethereum thinker for long-term protocol, privacy, governance, and public-goods direction. | Ethereum's long-term social and technical roadmap: privacy, governance, local-first AI, decentralization, and credible neutrality. |
| Ethereum builder path | Austin Griffith | [@austingriffith](https://x.com/austingriffith) | Practical Ethereum builder educator and tooling advocate. | How humans and AI agents can learn Ethereum development, and what tooling makes on-chain building easier. |
| AI x Governance | DeepFunding | [@DeepFunding](https://x.com/DeepFunding) | Recommended partner account for AI x governance and public-goods funding. | Reputation, contribution evaluation, decentralized collaboration, and how AI can help allocate resources. |

## Why This Feed Is Useful

I do not want an information flow that is only about market attention. I want a feed that helps me observe the real operating layer of AI x Web3:

- Who authorizes an AI agent to act?
- Who pays when an agent triggers an on-chain action?
- What permission scope is safe enough for automation?
- How can wallets, smart accounts, session keys, and spending limits protect users?
- Which parts of AI x Web3 are real infrastructure, and which parts are only narrative?
- How can privacy, security, auditability, and user consent be designed before execution?

This connects directly to my learning direction: **Programmable Compliance**. Compliance should be embedded into product and protocol design before a high-risk action happens, instead of becoming an after-the-fact legal remedy.

## Content Notes

### 1. AIxWeb3 School: AI agents need authorization, payment, and responsibility boundaries

The AIxWeb3 School pinned post frames the course around a practical question: when an AI agent can act on behalf of a user, who authorizes it, who pays, and who is responsible when something goes wrong?

The technical/product trend behind this is that AI agents are moving from "chat and recommendation" into tool use, data access, wallet actions, payment, and on-chain execution. This makes Web3 relevant because Web3 has native concepts for wallets, signatures, smart contracts, permissions, settlement, and verifiable records.

Relation to Week 1: Week 1 emphasized that Web3 builders in the AI era need stronger architecture and security thinking. This post gives the reason: the important problem is not only whether an AI can generate an answer, but whether it can safely perform an action.

My open question: what is the minimum product pattern for user consent when an AI agent needs repeated permissions instead of one-time confirmation?

### 2. LXDAO: agent capability makes authorization and responsibility a product problem

LXDAO's visible pinned discussion repeats the same core boundary: if an AI agent can place an order, transfer funds, or send an email, authorization, payment, and responsibility cannot be handled by intuition.

The product trend is that permission design becomes part of the user experience. A builder cannot hide behind a vague "the user approved it" flow. The product should show what the agent can do, under what limits, how the user can revoke access, and what requires human confirmation.

Relation to Week 1: this matches the idea that architecture capability matters more in the AI era. The architecture is not only backend/frontend; it includes trust boundaries, signing boundaries, execution boundaries, and accountability records.

My open question: how should products communicate permission scope to normal users without overwhelming them with wallet/security details?

### 3. LI.FI: intents are becoming infrastructure for payments, RWAs, and compliant liquidity

LI.FI's pinned content introduces LI.FI Intents as infrastructure for apps, wallets, and financial products to support stablecoin payments, real-world assets, and compliant on-chain liquidity.

The trend is that users may not want to manually choose a bridge, route, chain, or DEX. They may express an intent, and infrastructure will find a route. This is powerful for agentic execution because agents also need routing layers to complete financial actions.

Relation to Week 1: this helps connect Web3 basics to AI x Web3. Wallets and chains are not isolated concepts; they become the execution layer for future AI-assisted financial products.

My open question: when an intent solver chooses a route, how can the user or agent verify that the route is safe, compliant, and not only cheap or fast?

### 4. Z.ai / GLM: agentic coding and long-context inference make AI tools more practical for builders

Z.ai's visible content discusses model infrastructure, long-context inference, and GLM-5.1 being used for agentic coding and repo repair benchmarks.

The trend is that AI tools are becoming more capable at working across larger codebases and longer tasks. For Web3 builders, this can reduce the barrier to building prototypes, auditing code, reading docs, and creating learning artifacts.

Relation to Week 1: Week 1 encouraged using AI as a learning and building assistant, but not blindly delegating judgment. Stronger AI coding tools are useful only if the human still understands the risk boundary.

My open question: how should a non-traditional developer verify AI-generated Web3 code before it touches wallets, signatures, or deployed contracts?

### 5. Vitalik: privacy and local AI are still core infrastructure questions

Vitalik's visible recent posts touched on privacy infrastructure for voting/collaboration and also local LLM hardware constraints. These are not only abstract research topics. They matter for AI x Web3 because agents may handle private data, user preferences, governance choices, and financial actions.

The trend is that AI x Web3 needs both decentralization and privacy. If every useful agent requires centralized data access, the system may become convenient but fragile. If local or privacy-preserving AI becomes more practical, users may keep more control over sensitive information.

Relation to Week 1: this expands the "Web3 architecture" frame beyond contracts and tokens. Architecture also includes where data is processed, who can observe user intent, and whether the system can protect collective decision-making.

My open question: which privacy guarantees are realistic for near-term AI agent products, and which are still research-level?

## My Observation Framework

When I follow these accounts, I will sort useful information into five questions:

| Question | Why it matters |
|---|---|
| What action can the agent perform? | Separates content generation from real execution. |
| What permission does the user grant? | Shows whether the product has clear security boundaries. |
| What happens before signing or payment? | Identifies where programmable compliance can intervene. |
| What record is created after execution? | Determines whether the action can be audited or disputed. |
| What remains unclear or risky? | Prevents me from treating every AI x Web3 narrative as real infrastructure. |

## Final Takeaway

My information flow should help me watch the shift from AI as an assistant to AI as an economic actor. The key learning object is not "more accounts" but better judgment: which projects make agent execution safer, more verifiable, more private, and more accountable.

For my own direction, the most important line is:

**AI x Web3 becomes serious when agents can act, wallets can limit action, infrastructure can verify action, and compliance can be designed before action.**
