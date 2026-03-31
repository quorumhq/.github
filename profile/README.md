## Quorum

**The accuracy layer for AI agent workflows.**

AI agent workflows fail because errors compound at every step. 85% per-step accuracy across 12 steps = 14% end-to-end success. Quorum intercepts errors at runtime — with verification, multi-model consensus, and self-healing — so your pipeline succeeds instead of silently failing.

### How it works

1. **Verify** — Schema checks, range validation, LLM-as-judge on every step output
2. **Consensus** — Run critical steps across multiple models, take the majority answer
3. **Self-heal** — When verification catches an error, retry with a different strategy automatically

### Get started

```bash
# Scan your codebase — see your compound accuracy number
pip install quorum-chaos
quorum-chaos scan ./my_agent/

# Fix it — change one environment variable
export OPENAI_BASE_URL=http://localhost:8741/v1
python my_agent.py  # your code, unchanged, now verified
```

### Products

| Product | What | Repo |
|---------|------|------|
| **Accuracy** | Rust runtime — verification, consensus, self-healing, pipeline orchestration | [quorum](https://github.com/quorumhq/quorum) |
| **Insights** | AI-powered product analytics. Connects to PostHog/Amplitude/any source. | [quorum-insights](https://github.com/quorumhq/quorum-insights) |
| **Actions** | Automated playbook engine. Monitors metrics, intervenes, measures. | [quorum-actions](https://github.com/quorumhq/quorum-actions) |

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
