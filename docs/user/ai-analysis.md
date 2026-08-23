# AI Analysis

AI is off by default. Chronlyt currently implements an OpenAI-compatible adapter with configurable HTTPS base URL, model and API key; other providers require dedicated adapters.

Enable AI and behavioural data sharing, choose the period/categories/detail level, preview the exact payload, then use the one-time consent action. The key is retrieved from the OS credential store and never stored in SQLite, localStorage, logs, exports or backups. Provider failures do not affect core features.
