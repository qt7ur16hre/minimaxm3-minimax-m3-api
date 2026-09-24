# MiniMax M3 API (minimax-m3 / minimaxm3) — llm guide with published pricing

> **input $0.24; output $0.96** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-1d5d5c)** · **[Get an API key](https://go.apimart.ai/k-dfef7b)**

Everything here refers to **minimax-m3** — also written **minimaxm3** or **minimax m3**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $0.24 |
| `output` | $0.96 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $24 |
| 1,000 | $240 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"minimax-m3","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
