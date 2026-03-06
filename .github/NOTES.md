# 🧠 Copilot Memory — NOTES.md

## Kod wywołania: `@sync`
Użyj `@sync` żeby przypomnieć mi kontekst sesji.

---

## 📌 Status projektu (2026-03-06)

### Co robimy?
Konfigurujemy MCP serwery dla GitHub Copilot w repo `marekdkropiewnicki-dotcom/cli`.

### Co już zrobione?
- ✅ `.github/mcp.json` — skonfigurowany z serwerami:
  - railway
  - brave-search
  - telegram
  - huggingface
  - discord (token jako `${{ secrets.DISCORD_BOT_TOKEN }}`)
- ✅ Secret `DISCORD_BOT_TOKEN` dodany do repo secrets
- ✅ Secret scanning — zaakceptowany (wybrano "It's used in tests")

### Problem
- ⚠️ iOS / gh app resetuje kontekst rozmowy — Copilot traci pamięć sesji
- ⚠️ Przez to trzeba zaczynać od nowa za każdym razem

### Następne kroki
- 🔲 Przetestować działanie Discord MCP
- 🔲 Ewentualnie dodać kolejne MCP serwery

---

## 🔑 Ważne informacje
- Repo: `marekdkropiewnicki-dotcom/cli`
- Branch: `trunk`
- Właściciel: `marekdkropiewnicki-dotcom`