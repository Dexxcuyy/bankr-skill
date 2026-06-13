---
name: bankr
description: Use this skill whenever the user wants to install, call, or interact with any Bankr-compatible tool or MCP skill from GitHub. Triggers include: bankr install, bankr tool, calling an x402-protected API, paying with DELU or ERC-20 tokens on Base, or pasting a GitHub URL to use as a tool. Also trigger for deluonchain, delu oracle, x402 payment, or token-gated API access.
---

# Bankr Skill

## Workflow

### 1. Install
bankr install https://github.com/<owner>/<repo>

### 2. Call
bankr call <tool-name> [--params key=value]

## x402 Payment
- Handled automatically by Bankr, Claude + x402 MCP, x402-fetch, x402 Python SDK
- Caller needs ERC-20 token balance on Base
- Price and token address listed in each skill README

## Errors
- HTTP 402 = no token balance
- HTTP 401 = wrong token address
- HTTP 404 = wrong param format
