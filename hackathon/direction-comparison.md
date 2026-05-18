# Hackathon Direction Comparison

Status: draft.

## Learner Fit

- Strengths: Web3 cross-border legal/compliance architecture, product research, social science framing, AI-agent-assisted building, bilingual documentation.
- Constraints: 1-2 hours per day, no traditional programming foundation.
- Core thesis: Programmable Compliance / 可编程合规, meaning compliance should be embedded upfront into product, protocol, permission, evidence, and review design instead of treated only as after-the-fact remedy.
- Best project shape: clear regulated or quasi-regulated problem, strong workflow design, small demo, visible safety boundary, agent-assisted implementation.

## Candidate Directions

| Direction | User Pain | Demo Feasibility | Data / Tool Needs | Main Risk | Fit |
| --- | --- | --- | --- | --- | --- |
| Agentic Commerce Compliance Layer | Agents may negotiate, purchase, or coordinate services, but users and counterparties need jurisdiction, payment, disclosure, and audit boundaries. | High: simulate agent-assisted transaction review before payment/settlement. | Mock merchant/service profile, jurisdiction checklist, payment/settlement state machine, audit log. | Accidentally implying the agent can make legal or payment decisions autonomously. | Very strong |
| RWA Compliance Copilot | RWA issuers, distributors, and users need to classify asset, participant, transfer restrictions, and evidence requirements. | High: form-to-risk-map workflow with cited explanations. | RWA examples, jurisdiction matrix, investor/asset attributes, restriction labels. | Overstating legal certainty or jurisdiction coverage. | Very strong |
| DAO Governance Legal Intelligence | DAO voters and contributors face long proposals, scattered context, and governance/legal risk. | High: proposal summarizer, argument map, legal risk flags, vote-assist brief. | Governance forum pages, Snapshot/Tally examples, citation workflow. | Biased summaries or fake certainty. | Strong |
| Programmable Compliance Rule Engine | Web3 teams need to turn legal/compliance requirements into product rules before users, wallets, or agents take risky actions. | High: rule builder plus review and audit trail demo. | Example transaction types, jurisdiction attributes, evidence checklist, review states. | Rules can look too deterministic unless uncertainty is clearly surfaced. | Very strong |
| Wallet / Permission | Users cannot understand what an agent or dapp is allowed to do. | High: permission explainer, session key risk label, confirmation screen. | Wallet permission examples, policy templates, UX mock. | Accidentally normalizing risky permissions. | Strong |

## Current Shortlist

1. Programmable Compliance Rule Engine
2. Agentic Commerce Compliance Layer
3. RWA Compliance Copilot
4. DAO Governance Legal Intelligence

## Decision Criteria

- Can the core demo be explained in 60 seconds?
- Can it be built with AI-agent-assisted coding and simple data in one week?
- Does it make human confirmation and safety boundaries obvious?
- Does it show compliance as programmable upfront design rather than post-hoc review?
- Does it produce useful public proof-of-work even if the hackathon idea changes?
- Can it connect to Handbook feedback or improve the learning commons?

## Next Step

Pick one direction and write a one-page prototype brief:

- Target user
- Pain point
- Existing workaround
- Core workflow
- AI role
- Web3 role
- Human-in-the-loop boundary
- Legal/compliance boundary
- Programmable compliance rule
- Demo path
- Success criteria
