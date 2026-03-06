# 🧠 Copilot Memory — NOTES.md

## Kod wywołania: `@sync`
Użyj `@sync` żeby przypomnieć mi kontekst sesji.

---

## 📌 Status projektu (2026-03-06)

### Co robimy?
Konfigurujemy MCP serwery dla GitHub Copilot w repo `marekdkropiewnicki-dotcom/cli`.

### Urządzenie
- 📱 iPhone 16 — tylko iOS (brak dostępu do PC)

### Co już zrobione?
- ✅ `.github/mcp.json` — skonfigurowany z serwerami:
  - **github** — zdalny SSE endpoint `https://mcp.github.com/mcp` ✅ (działa na iOS!)
  - **context7** (`@upstash/context7-mcp`) — stdio (wymaga PC)
  - **brave-search** — zdalny SSE via Smithery ✅ (działa na iOS!)
  - **telegram** — klucze jako secrets (wymaga PC)
  - **discord** — token jako secrets (wymaga PC)
- ✅ Secret `DISCORD_BOT_TOKEN` dodany do repo secrets
- ✅ Secret `BRAVE_API_KEY` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_ID` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_HASH` dodany do repo secrets
- ✅ Secret `SMITHERY_API_KEY` dodany do repo secrets
- ✅ Secret scanning — zaakceptowany (wybrano "It's used in tests")
- ✅ `.github/NOTES.md` — pamięć Copilota działa
- ✅ Wszystkie klucze przeniesione do secrets (brak plain text)
- ✅ Serwer `github` zaktualizowany na zdalny SSE endpoint
- ✅ Serwer `brave-search` zaktualizowany na zdalny SSE via Smithery
- ✅ Projekt częściowo na iOS — 2 serwery SSE działają!

### Problem
- ⚠️ iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji
- ✅ Rozwiązanie: `@sync` + NOTES.md

### 🔲 Jeszcze do zrobienia
- 🔲 Przetestować działanie serwerów `github` i `brave-search` (SSE) na iOS
- 🔲 Serwery `context7`, `telegram`, `discord` wymagają PC + VS Code

---

## 🔑 Ważne informacje
- Repo: `marekdkropiewnicki-dotcom/cli`
- Branch: `trunk`
- Właściciel: `marekdkropiewnicki-dotcom`
- Kod wywołania pamięci: `@sync`

---

## 📋 Aktualna konfiguracja mcp.json
| Serwer | Typ | Endpoint/Package | Secrets |
|--------|-----|-----------------|---------|
| github | `sse` | `https://mcp.github.com/mcp` | brak ✅ |
| context7 | `stdio` | `@upstash/context7-mcp` | brak (wymaga PC) |
| brave-search | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` ✅ |
| telegram | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID` ✅, `TELEGRAM_API_HASH` ✅ (wymaga PC) |
| discord | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` ✅ (wymaga PC) |