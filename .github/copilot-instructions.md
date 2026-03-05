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
- **Copilot Memory:** ✅ Enabled
- **MCP servers:** ✅ Enabled
- **Copilot Spaces:** ✅ Enabled (wymaga VSCode — na razie pomijamy)
- **AI model training:** ❌ Disabled (świadoma decyzja prywatności)

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
- Copilot Spaces — pomijamy (wymaga VSCode, nie dostępne na iOS)
- Sprawdzono wszystkie ustawienia Copilot — wszystko ✅ Enabled
- AI model training — ❌ Disabled (świadoma decyzja)
- Premium requests: 49.8% wykorzystane
- GitHub app wyrzuca sesję — dodano notatkę do Setup
