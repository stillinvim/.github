# stillinvim

Upstream forks and patches by [@howtoexitvim](https://github.com/howtoexitvim). Kept in a separate org so my personal repository list stays clean.

## Patches

| Project | Summary | Links | Fork / Branch |
| :--- | :--- | :--- | :--- |
| [google-antigravity/antigravity-cli](https://github.com/google-antigravity/antigravity-cli) | Fix orphaned `agy --hub` processes left behind on VS Code window close (`subscriptions.dispose()` vs `deactivate()` race in `extension.js`). | [Issue #1390](https://github.com/google-antigravity/antigravity-cli/issues/1390), [#183 comment](https://github.com/google-antigravity/antigravity-cli/issues/183#issuecomment-6561864681) | [stillinvim/antigravity-cli](https://github.com/stillinvim/antigravity-cli) |
| [google-antigravity/antigravity-sdk-python](https://github.com/google-antigravity/antigravity-sdk-python) | Fix `localharness` subprocess and WebSocket leaks on `asyncio.CancelledError` and early stdio EOF in `LocalConnectionStrategy`. | [Issue #279](https://github.com/google-antigravity/antigravity-sdk-python/issues/279), [patch comment](https://github.com/google-antigravity/antigravity-sdk-python/issues/279#issuecomment-6561876940) | [fix/localharness-orphan-process-leak](https://github.com/stillinvim/antigravity-sdk-python/commit/44801ec) |
