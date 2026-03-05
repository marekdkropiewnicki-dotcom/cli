# Copilot Instructions for cli (workspace)

## O tym repo

To repozytorium (`cli`) służy jako **główny workspace** do codziennej pracy na iPhone (iOS).
Jest to fork oficjalnego GitHub CLI (`gh`), napisanego w Go.

## Właściciel

- **GitHub:** marekdkropiewnicki-dotcom
- **Device:** iPhone (iOS) — wszystkie sesje prowadzone na iOS

## Główny projekt: GeNCorE

Równolegle prowadzimy projekt AI — **GeNCorE** (`marekdkropiewnicki-dotcom/GentelmeN-CorE`):
- Telegram bot w Pythonie
- AI chat via Groq (llama-3.3-70b-versatile, llama-3.1-8b-instant, qwen-2.5-32b)
- Generowanie obrazów via Hugging Face
- Kryptowaluty via KuCoin (ccxt)
- Wyszukiwanie via Brave Search API
- Deployment na Railway

## Team AI

| Kto | Rola |
|-----|------|
| 👨 Marek | Pomysłodawca, developer |
| 🤖 GitHub Copilot | Kod, PR, GitHub, Chat |
| 🧠 Claude (Anthropic) | Coding agent — włączony |
| ⚡ Codex | Coding agent — włączony |

## Copilot Setup

- **Plan:** Copilot Pro+
- **Premium requests:** ~49.8% wykorzystane (reset 1. dnia miesiąca)
- **Coding agents:** Copilot ✅ Claude ✅ Codex ✅
- **Automatic code review:** ✅ Enabled
- **Copilot Memory:** ✅ Enabled (Preview)
- **MCP servers:** ✅ Enabled
- **Copilot Spaces:** ✅ Enabled
- **Copilot-generated commit messages:** ✅ Enabled
- **AI model training:** ❌ Disabled (świadoma decyzja prywatności)

## Copilot Spaces

- **Space:** GentelmeN-CorE — aktywny
- **Model:** Claude Opus 4.6 ✅
- **Link:** https://github.com/copilot/spaces
- **Instructions:**

```
You are an AI coding assistant for the GeNCorE project — a Telegram bot written in Python.

Stack:
- AI chat: Groq (llama-3.3-70b-versatile, llama-3.1-8b-instant, qwen-2.5-32b)
- Image generation: Hugging Face
- Crypto: KuCoin via ccxt
- Search: Brave Search API
- Deployment: Railway

Focus on:
- Python best practices
- Telegram bot architecture (python-telegram-bot)
- API integrations and error handling
- Railway deployment optimization

Avoid:
- Suggesting desktop tools (owner works on iPhone/iOS)
- Overcomplicated solutions — keep it simple and clean
- English responses — always respond in Polish 🇵🇱
```

## Privacy

- **Suggestions matching public code:** ✅ Allowed
- **Allow data for product improvements:** ✅ Enabled (ptaszek — domyślne)
- **Allow data for AI model training:** ❌ Disabled (świadoma decyzja)

## Setup (iPhone iOS)

- **GitHub app + Copilot Pro+** — przeglądanie repo, Copilot Chat
- **Working Copy** — Git (commit, push, pull)
- **Textastic** — edytor kodu
- **Brave** — przeglądarka
- ⚠️ GitHub app czasem wyrzuca sesję — po powrocie wracamy do `cli` repo jako kontekst

## Zasady współpracy

- Komunikacja po **polsku** 🇵🇱
- Krótkie, konkretne odpowiedzi — bez zbędnego gadania
- Zawsze pytaj o jeden wybór na raz — nie przytłaczaj opcjami
- Pamiętaj że pracujemy na iPhone — nie sugeruj narzędzi desktopowych
- Główna gałąź: `trunk`

## Session History

### 2026-03-05
- Stworzono `.github/copilot-instructions.md` w `cli` jako główny workspace
- Ustalono setup: GitHub app + Working Copy + Textastic + Brave
- Aktywny projekt: GeNCorE (PR #7 otwarty — Fix GeNCorE naming, HF 410, voice routing)
- Skonfigurowano Copilot Pro+: coding agents (Copilot + Claude + Codex), automatic code review, Memory, MCP
- Copilot Spaces — aktywne, Space GentelmeN-CorE utworzony
- Model w Space: zmieniony na Claude Opus 4.6 ✅
- Instructions w Space — dodane ✅
- Sprawdzono wszystkie ustawienia Copilot — wszystko ✅ Enabled
- AI model training — ❌ Disabled (świadoma decyzja)
- Product improvements — ✅ Enabled (ptaszek, domyślne)
- Premium requests: 49.8% wykorzystane
- GitHub app wyrzuca sesję — dodano notatkę do Setup
- Copilot-generated commit messages — ✅ Enabled