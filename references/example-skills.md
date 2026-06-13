# Example Bankr Skills

## deluskill — Delu Oracle

Repo: https://github.com/deluonchain/deluskill

Install:
bankr install https://github.com/deluonchain/deluskill

Endpoint:
GET https://<host>/delu-oracle/analyze/{ca}

Pricing:
- 100,000 DELU per call (x402, ERC-20 on Base)
- Token: 0x7b0ee9dcb5c1d4d7cd630c6529599951936512ba3
- Optional: ?social=true (+$0.45 USDC)
- Optional: ?verbose=true (raw data)

Response fields:
- action: ENTER / WATCH / AVOID
- conviction: 0-100
- direction: long / short
- entry_low / entry_high: entry zone
- stop: stop loss level
- size_pct: position size hint
- read: one-line summary
- verdict: strong_buy / buy / hold / avoid / drop
- score: 0-100 fused cognition score
- signals: momentum, flow, structure, volatility, liquidity

Chain: Base only
