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

### Repos

| Repo | What |
|------|------|
| [agent-chaos](https://github.com/quorumhq/agent-chaos) | Scan agent codebases for accuracy anti-patterns |
| *quorum-core* | Rust runtime — verification, consensus, self-healing *(coming soon)* |
| *quorum-proxy* | OpenAI-compatible verification proxy *(coming soon)* |
| *quorum-python* | Python SDK + framework integrations *(coming soon)* |

### Links

- 🌐 [quorum.dev](https://quorum.dev)
- 📐 [The compound accuracy calculator](https://quorum.dev/accuracy)
- 📖 [Documentation](https://quorum.dev/docs)

Open core — MIT-licensed runtime, commercial cloud. Built by the team behind [Avail](https://availproject.org).
