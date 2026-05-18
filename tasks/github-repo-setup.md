# Task: GitHub Learning Repo Setup

- Source: Learning Agent startup prompt.
- Status: pending user confirmation.

## Recommended Defaults

- Repo name: `ai-web3-school-cohort-0`
- Visibility: public
- Local path: `/Users/venger/Desktop/Web3/AI×Web3 School`
- Description: `Personal learning journal and proof-of-work for AI x Web3 School.`

## Current State

- Local files are initialized.
- Local Git repo is initialized.
- GitHub CLI command `gh` is not installed in this environment.
- No remote repo has been created yet.
- No commit has been made yet.

## Safe Setup Steps

1. Install GitHub CLI from https://cli.github.com/ if you want to use the command-line flow.
2. Run `gh auth login` and complete browser login.
3. Run `gh auth status` to confirm login.
4. Confirm repo name, public/private visibility, and local path before creating the remote repo.

## Commands After Confirmation

```bash
gh repo create ai-web3-school-cohort-0 --public --description "Personal learning journal and proof-of-work for AI x Web3 School" --source . --remote origin --push
```

Do not send tokens, passwords, verification codes, private keys, seed phrases, or API keys to the agent.
