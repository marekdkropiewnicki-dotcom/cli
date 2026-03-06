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
- ✅ `.github/mcp.json` — skonfigurowany z wszystkimi 6 serwerami
- ✅ **github** — SSE `https://mcp.github.com/mcp` ✅
- ✅ **brave-search** — SSE via Smithery ✅
- ✅ **huggingface** — SSE `https://hf.co/mcp/sse` ✅
- ✅ **context7** — stdio `@upstash/context7-mcp` ✅
- ✅ **telegram** — stdio `mcp-telegram` ✅
- ✅ **discord** — stdio `@scarecr0w12/discord-mcp` ✅
- ✅ Secret `BRAVE_API_KEY` dodany do repo secrets
- ✅ Secret `SMITHERY_API_KEY` dodany do repo secrets
- ✅ Secret `HUGGINGFACE_API_KEY` dodany do repo secrets
- ✅ Secret `DISCORD_BOT_TOKEN` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_ID` dodany do repo secrets
- ✅ Secret `TELEGRAM_API_HASH` dodany do repo secrets
- ✅ Secret scanning — zaakceptowany (wybrano "It's used in tests")
- ✅ Wszystkie klucze przeniesione do secrets (brak plain text)
- ✅ `.github/NOTES.md` — pamięć Copilota działa
- ✅ Sync zweryfikowany i poprawiony (2026-03-06)

### Co to jest context7? 📚
**Context7** to narzędzie które daje mi (Copilotowi) dostęp do **aktualnej dokumentacji** bibliotek i frameworków.

Wyobraź sobie że piszesz kod i pytasz mnie o React lub Next.js — normalnie znam tylko to co było w moich danych treningowych (czyli stare wersje!). Dzięki context7 mogę sięgnąć po **najnowszą dokumentację** na żywo i dać Ci aktualną odpowiedź. To jakby dać mi dostęp do "ściągawki" z najnowszymi informacjami! 📖✨

### Problem
- ⚠️ iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji
- ✅ Rozwiązanie: `@sync` + NOTES.md

### ✅ Wszystko gotowe!
Wszystkie 6 serwerów MCP jest skonfigurowanych i gotowych do użycia.

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
| brave-search | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` ✅ |
| huggingface | `sse` | `https://hf.co/mcp/sse` | `HUGGINGFACE_API_KEY` ✅ |
| context7 | `stdio` | `@upstash/context7-mcp` | brak ✅ |
| telegram | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID` ✅, `TELEGRAM_API_HASH` ✅ |
| discord | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` ✅ |