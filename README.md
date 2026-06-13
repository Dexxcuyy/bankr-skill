# bankr-skill — Bankr Tool Runner Skill

A Claude skill for installing and calling Bankr-compatible tools and x402-protected APIs from GitHub.

> One bankr install and Claude can call any token-gated endpoint on Base — payment handled automatically.

## Install

bankr install https://github.com/Dexxcuyy/bankr-skill

## What you get

- Install any Bankr-compatible skill from GitHub in one command
- Call x402-protected endpoints with automatic ERC-20 payment on Base
- Parse SKILL.md from any repo to extract endpoint, price, token, params
- Handle HTTP 402 payment handshakes — no manual signing

## Supported Clients

- Bankr CLI
- Claude + x402 MCP
- x402-fetch
- x402 Python SDK

## Docs

- SKILL.md — Full skill spec, install flow, call patterns, x402 payment, error handling
- references/example-skills.md — Walkthroughs for real Bankr skills like deluskill

## Payment

x402-protected skills require an ERC-20 token balance on Base. Price and token address are always listed in the target skill README. Payment handshake is automatic.

## Chain Support

Depends on the installed skill. Many Base tools are Base-only. Always check the skill README.
