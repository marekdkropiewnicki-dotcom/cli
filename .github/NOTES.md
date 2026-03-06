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
- ✅ Serwer `github` zaktualizowany na zdalny SSE endpoint
- ✅ Projekt w pełni skonfigurowany!

### Problem
- ⚠️ iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji
- ✅ Rozwiązanie: `@sync` + NOTES.md

### 🔲 Jeszcze do zrobienia
- 🔲 Przetestować działanie serwera `github` (SSE) na iOS
- 🔲 Pozostałe serwery (context7, brave, telegram, discord) wymagają PC + VS Code

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
| context7 | `stdio` | `@upstash/context7-mcp` | brak ✅ |
| brave-search | `stdio` | `@brave/brave-search-mcp-server` | `BRAVE_API_KEY` ✅ |
| telegram | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID` ✅, `TELEGRAM_API_HASH` ✅ |
| discord | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` ✅ |