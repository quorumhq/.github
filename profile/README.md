## Quorum

**Three products. One suite. Make AI-powered products work, understand why, and act on it.**

### Products

| Product | What | For | Repo |
|---------|------|-----|------|
| **Accuracy** | Runtime that intercepts AI agent errors with verification, multi-model consensus, and self-healing. 85% per-step × 12 steps = 14% success. Quorum fixes that. | Engineering teams | [quorum](https://github.com/quorumhq/quorum) |
| **Insights** | AI-powered product analytics intelligence. Connects to PostHog, Amplitude, or any analytics source. Tells you *what's driving your metrics* — not just what happened. | Product teams | [quorum-insights](https://github.com/quorumhq/quorum-insights) |
| **Actions** | Automated playbook engine. Monitors your metrics, intervenes when things go wrong, measures the result. | Growth teams | [quorum-actions](https://github.com/quorumhq/quorum-actions) |

Each product works standalone. Together, they connect — AI quality becomes a first-class dimension in your analytics and automation.

### Get started

```bash
# Scan your agent codebase — see your compound accuracy number
pip install quorum-chaos
quorum-chaos scan ./my_agent/

# Fix it — change one environment variable
export OPENAI_BASE_URL=http://localhost:8741/v1
python my_agent.py  # your code, unchanged, now verified
```

### Ecosystem

| Repo | What |
|------|------|
| [open-agent-traces](https://github.com/quorumhq/open-agent-traces) | Open trace format spec for AI agent accuracy — community standard |
| [quorum-pi](https://github.com/quorumhq/quorum-pi) | Quorum extension for [pi](https://github.com/mariozechner/pi-coding-agent) coding agent |
| [quorum-vercel](https://github.com/quorumhq/quorum-vercel) | Middleware for Vercel AI SDK |
| [quorum-dify](https://github.com/quorumhq/quorum-dify) | Verification plugin for Dify |
| [n8n-nodes-quorum](https://github.com/quorumhq/n8n-nodes-quorum) | Verification node for n8n workflows |
| [quorum-coze](https://github.com/quorumhq/quorum-coze) | Plugin for ByteDance Coze |

### Links

- 🌐 [quorumhq.xyz](https://quorumhq.xyz)
- 📐 [The compound accuracy calculator](https://quorumhq.xyz/accuracy)
- 📖 [Documentation](https://quorumhq.xyz/docs)

Open core — MIT-licensed runtime, commercial cloud.
