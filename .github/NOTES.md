# 🧠 Copilot Memory — NOTES.md

## Kod wywołania: `@sync`
Użyj `@sync` żeby przypomnieć mi kontekst sesji.

---

## 📌 Status projektu (2026-03-06)

### Co robimy?
Konfigurujemy MCP serwery dla GitHub Copilot w repo `marekdkropiewnicki-dotcom/cli`.

### Co już zrobione?
- ✅ `.github/mcp.json` — skonfigurowany z serwerami:
  - **github** (`@modelcontextprotocol/server-github`) — zastąpił huggingface
  - **context7** (`@upstash/context7-mcp`) — zastąpił railway
  - **brave-search** — klucz jako `${{ secrets.BRAVE_API_KEY }}`
  - **telegram** — klucze jako secrets
  - **discord** — token jako `${{ secrets.DISCORD_BOT_TOKEN }}`
- ✅ Secret `DISCORD_BOT_TOKEN` dodany do repo secrets
- ✅ Secret `BRAVE_API_KEY` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_ID` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_HASH` dodany do repo secrets
- ✅ Secret scanning — zaakceptowany (wybrano "It's used in tests")
- ✅ `.github/NOTES.md` — pamięć Copilota działa
- ✅ Wszystkie klucze przeniesione do secrets (brak plain text)
- ✅ Projekt w pełni skonfigurowany!

### Problem
- ⚠️ iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji
- ✅ Rozwiązanie: `@sync` + NOTES.md

### 🔲 Jeszcze do zrobienia
- 🔲 Przetestować działanie wszystkich MCP serwerów

---

## 🔑 Ważne informacje
- Repo: `marekdkropiewnicki-dotcom/cli`
- Branch: `trunk`
- Właściciel: `marekdkropiewnicki-dotcom`
- Kod wywołania pamięci: `@sync`

---

## 📋 Aktualna konfiguracja mcp.json
| Serwer | Package | Secrets |
|--------|---------|---------|
| github | `@modelcontextprotocol/server-github` | `GITHUB_TOKEN` ✅ |
| context7 | `@upstash/context7-mcp` | brak ✅ |
| brave-search | `@brave/brave-search-mcp-server` | `BRAVE_API_KEY` ✅ |
| telegram | `mcp-telegram` | `TELEGRAM_API_ID` ✅, `TELEGRAM_API_HASH` ✅ |
| discord | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` ✅ |