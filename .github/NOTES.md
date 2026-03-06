# 🧠 Copilot Memory — NOTES.md

## Kod wywołania: `@sync`
Użyj `@sync` żeby przypomnieć mi kontekst sesji.

---

## 📌 Status projektu (2026-03-06)

### Co robimy?
Konfigurujemy MCP serwery dla GitHub Copilot w repo `marekdkropiewnicki-dotcom/cli`.

### Urządzenie
- 📱 iPhone 16 — tylko iOS

---

### ✅ Co już zrobione?

**Serwery MCP (`mcp.json`):**
- `github` — SSE `https://mcp.github.com/mcp`
- `brave-search` — SSE via Smithery
- `huggingface` — SSE `https://hf.co/mcp/sse`
- `context7` — stdio `@upstash/context7-mcp`
- `telegram` — stdio `mcp-telegram`
- `discord` — stdio `@scarecr0w12/discord-mcp`

**Secrets:**
- `SMITHERY_API_KEY`
- `HUGGINGFACE_API_KEY`
- `DISCORD_BOT_TOKEN`
- `TELEGRAM_API_ID`
- `TELEGRAM_API_HASH`
- `BRAVE_API_KEY`

**Inne:**
- Wszystkie klucze przeniesione do secrets (brak plain text)
- Secret scanning zaakceptowany ("It's used in tests")
- `NOTES.md` — pamięć Copilota działa
- Sync zweryfikowany (2026-03-06)

---

### 🟢 Stan projektu
Wszystkie 6 serwerów MCP skonfigurowanych i gotowych do użycia.

---

### ⚠️ Znany problem
iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji.
**Rozwiązanie:** `@sync` + NOTES.md

---

### 📖 Co to jest context7?
**Context7** daje Copilotowi dostęp do **aktualnej dokumentacji** bibliotek i frameworków na żywo — zamiast przestarzałych danych treningowych.

---

## 🔑 Ważne informacje
- Repo: `marekdkropiewnicki-dotcom/cli`
- Branch: `trunk`
- Właściciel: `marekdkropiewnicki-dotcom`
- Sync: `@sync`

---

## 📋 Konfiguracja mcp.json

| Serwer | Typ | Endpoint / Package | Secrets |
|---|---|---|---|
| `github` | `sse` | `https://mcp.github.com/mcp` | — |
| `brave-search` | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` |
| `huggingface` | `sse` | `https://hf.co/mcp/sse` | `HUGGINGFACE_API_KEY` |
| `context7` | `stdio` | `@upstash/context7-mcp` | — |
| `telegram` | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID`, `TELEGRAM_API_HASH` |
| `discord` | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` |