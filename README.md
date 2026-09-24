# HappyHorse 1.1 API (happyhorse-1.1 / happyhorse1.1) — api guide with published pricing

> **720P $0.13; default $0.172; 1080P $0.172** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-97c0b1)** · **[Get an API key](https://go.apimart.ai/k-d6fcc6)**

Everything here refers to **happyhorse-1.1** — also written **happyhorse1.1** or **happyhorse 1.1**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `720P` | $0.13 |
| `default` | $0.172 |
| `1080P` | $0.172 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $13 |
| 1,000 | $130 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/videos/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"happyhorse-1.1","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
