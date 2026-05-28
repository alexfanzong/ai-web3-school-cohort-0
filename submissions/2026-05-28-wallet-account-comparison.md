# Week 2 Note: EOA, Smart Account, and Multisig Account

Status: ready to submit.

## Draft

这份笔记比较三类常见 Web3 账户：EOA、智能账户和多签账户。

我理解它们的核心区别不只是地址形式，而是：**谁控制账户、谁可以发起交易、谁可以批准交易，以及风险最终落在什么地方。**

## Comparison Table

| Dimension | EOA | Smart Account | Multisig Account |
|---|---|---|---|
| Who holds control | A single private key or seed phrase controls the account. | Control is defined by account contract logic. The controller can be one signer, multiple signers, devices, guardians, session keys, or policy modules. | A group of signers controls the account together through a threshold rule, such as 2-of-3 or 3-of-5. |
| Who can initiate a transaction | The private key holder can directly send transactions. | Any signer, app, session key, relayer, or automation flow allowed by the account policy may initiate or prepare actions. | Usually one signer can create a transaction proposal, but execution requires enough confirmations. |
| Who can approve execution | The same private key approves and executes. | Approval depends on policy: owner signature, guardian approval, spending limit rule, session key scope, or another contract-defined condition. | A required number of signers must approve before the transaction can be executed. |
| Multi-person confirmation | Not supported natively. | Supported if the smart account is designed with multi-owner or guardian rules. | Supported by default as the main design purpose. |
| Recovery, limits, or automation | Very limited. If the private key is lost, the account is usually lost. | Can support social recovery, daily limits, allowlists, session keys, gas sponsorship, automated payments, and policy-based execution. | Can support threshold changes, modules, spending limits, role separation, and operational workflows, depending on the multisig product. |
| Typical use cases | Personal wallet, test account, small-value on-chain interactions, simple dApp use. | Consumer wallet, app-specific wallet, AI-agent wallet, game account, subscription payment, enterprise policy wallet. | DAO treasury, project treasury, protocol admin account, company asset custody, grant or budget management. |
| Main risk points | Private key compromise, seed phrase loss, phishing signatures, unlimited token approvals, no built-in recovery. | Contract bugs, unsafe account modules, excessive automation permissions, weak recovery design, unclear session key scope. | Signer collusion, signer loss, poor threshold design, slow response in emergencies, all signers using weak operational security. |

## Security Boundary by Account Type

### EOA

An EOA is the simplest model: one private key controls everything.

The security boundary is the private key. If the private key or seed phrase is leaked, the attacker can transfer funds, approve tokens, sign messages, and interact with contracts as the account owner.

EOA is suitable for personal learning, small-value usage, and simple wallet interactions. It is not ideal for large treasuries, protocol admin rights, or any workflow that needs shared approval or recovery.

Example use case:

- A learner uses MetaMask to connect to a testnet dApp and send a small test transaction.

Main risk:

- A phishing site tricks the user into signing a malicious approval, or the seed phrase is exposed.

### Smart Account

A smart account uses contract logic to define account permissions.

The security boundary is no longer only one private key. It includes the account contract, enabled modules, recovery rules, spending limits, session keys, automation policies, and the services allowed to help execute transactions.

Smart accounts are useful when the user needs better experience or finer permission control. For example, an app may allow a session key to perform only game actions for one hour, while transfers above a limit still require manual confirmation.

Example use case:

- An AI-agent wallet can prepare transactions, use a limited session key for low-risk actions, and pause for human review before signing high-risk operations.

Main risk:

- A poorly designed module or over-broad session key may allow more actions than the user intended.

### Multisig Account

A multisig account separates control across multiple signers.

The security boundary is the approval threshold and signer management process. A single compromised signer should not be enough to drain the account, but the account is only as safe as the signer distribution, threshold design, and review process.

Multisig accounts are suitable for shared funds and high-impact permissions because they make unilateral action harder. They are less convenient for fast personal use because execution usually requires coordination.

Example use case:

- A DAO treasury uses a 3-of-5 multisig so that budget payments require several independent approvals.

Main risk:

- If enough signers collude, lose keys, or approve transactions without review, the multisig protection can fail.

## Actions That Must Require Human Confirmation

For a safe wallet or agent workflow, the following actions should require explicit human confirmation before execution:

| Action | Why manual confirmation is required |
|---|---|
| Sending real funds | Direct financial loss is possible if the recipient, amount, chain, or token is wrong. |
| Approving token spending | Token approvals can allow a contract to move assets later, especially if the approval is unlimited. |
| Signing messages with legal, identity, or financial meaning | Some signatures can authorize login, delegation, claims, or off-chain agreements. |
| Granting or changing session key permissions | A session key can quietly expand what an app or agent can do without asking again. |
| Enabling smart account modules or plugins | A malicious or buggy module can change the account's effective security model. |
| Changing guardians, recovery methods, or owners | Recovery and ownership changes can permanently shift control of the account. |
| Changing multisig threshold or signer list | A lower threshold or compromised signer set can weaken treasury security. |
| Executing DAO treasury, protocol admin, upgrade, or emergency actions | These actions can affect shared funds, users, contracts, or governance outcomes. |
| Interacting with unknown contracts | Unknown contracts may contain malicious logic, hidden permissions, or misleading transaction data. |
| Allowing automation above a small preset limit | Automation can be useful, but it should not silently move large funds or grant broad permissions. |

## Practical Rule

My practical rule is:

- Read-only actions can be automated.
- Drafting or simulating transactions can be automated.
- Low-value actions may use limited policies or session keys.
- Anything involving funds, approvals, ownership, recovery, governance, contract upgrades, or broad automation must require human confirmation.

## Summary

EOA is simple but has a single-key failure point.

Smart account is flexible and programmable, but its security depends on contract logic and policy design.

Multisig account is better for shared control and treasury safety, but it depends on signer discipline and threshold design.

For AI x Web3 workflows, the most important boundary is this: **AI can help explain, prepare, simulate, and classify actions, but signing, approval, fund movement, ownership change, and high-impact execution should remain human-confirmed.**

## Public Proof

- Learning repo: https://github.com/alexfanzong/ai-web3-school-cohort-0
- Local note: `submissions/2026-05-28-wallet-account-comparison.md`
