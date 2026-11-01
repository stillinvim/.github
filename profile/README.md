<div align="center">

# `stillinvim` — Still in Vim

**Open-source systems, AI agent infrastructure, and upstream root-cause engineering by [@howtoexitvim](https://github.com/howtoexitvim).**

[![Website](https://img.shields.io/badge/Website-shuqihere.top-181717?style=flat-square)](https://www.shuqihere.top)
[![Maintainer](https://img.shields.io/badge/Maintainer-%40howtoexitvim-2ea44f?style=flat-square)](https://github.com/howtoexitvim)

</div>

---

### 🔍 Upstream Contributions & Root-Cause Analyses

This organization hosts upstream forks, patches, and deep-dive root-cause analyses across AI agent frameworks and developer toolchains:

| Target Project | Contribution & Technical Summary | Upstream Reference | Patch / Branch |
| :--- | :--- | :--- | :--- |
| **[`google-antigravity/antigravity-cli`](https://github.com/google-antigravity/antigravity-cli)** | **Orphaned `agy --hub` Daemon Memory Leak on VS Code Window Close**: Diagnosed race condition between synchronous `subscriptions.dispose()` and async `deactivate()`, 5s Extension Host exit timeout collision, and missing `SIGTERM` fallback leaking 110–200 MB per closed window. | [Issue #1390](https://github.com/google-antigravity/antigravity-cli/issues/1390) · [Issue #183 Comment](https://github.com/google-antigravity/antigravity-cli/issues/183#issuecomment-6561864681) | [`stillinvim/antigravity-cli`](https://github.com/stillinvim/antigravity-cli) |
| **[`google-antigravity/antigravity-sdk-python`](https://github.com/google-antigravity/antigravity-sdk-python)** | **`LocalConnectionStrategy` Subprocess & WebSocket Leak Fix**: Fixed `local_connection.py`, `interactions_connection.py`, and `litert_connection.py` bypassing `process.kill()` / `ws.close()` upon Python 3.8+ `asyncio.CancelledError` (`BaseException`) and early stdio EOF, with regression unit tests. | [Issue #279](https://github.com/google-antigravity/antigravity-sdk-python/issues/279) · [Patch Comment](https://github.com/google-antigravity/antigravity-sdk-python/issues/279#issuecomment-6561876940) | [`fix/localharness-orphan-process-leak` (`44801ec`)](https://github.com/stillinvim/antigravity-sdk-python/commit/44801ec) |
