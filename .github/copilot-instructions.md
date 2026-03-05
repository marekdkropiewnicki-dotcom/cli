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
- **Sources:** do dodania ręcznie — `marekdkropiewnicki-dotcom/GentelmeN-CorE`
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

## MCP Servers

### Dostępne MCP dla GeNCorE stacku

| API | MCP | Status | Link |
|-----|-----|--------|------|
| **GitHub** | ✅ Oficjalny | ✅ Enabled | [github/mcp-server](https://github.com/github/mcp-server) |
| **Railway** | ✅ Oficjalny | ⏳ TODO | [railwayapp/railway-mcp-server](https://github.com/railwayapp/railway-mcp-server) |
| **Hugging Face** | ✅ Oficjalny | ⏳ TODO | [hf.co/mcp](https://huggingface.co/docs/hub/agents-mcp) |
| **Telegram** | ✅ Community | ⏳ TODO | [sparfenyuk/mcp-telegram](https://github.com/sparfenyuk/mcp-telegram) |
| **Brave Search** | ✅ Oficjalny | ⏳ TODO | [brave/brave-search-mcp-server](https://github.com/brave/brave-search-mcp-server) |
| **Groq** | ❌ Brak MCP | ❌ | — |
| **KuCoin** | ❌ Brak MCP | ❌ | — |
| **Copilot API** | ❌ Brak publicznego API | ❌ | — |

### Kolejność konfiguracji
1. **Railway MCP** ⏳ — następne w kolejce
2. Hugging Face MCP
3. Telegram MCP
4. Brave Search MCP

### Czego Copilot nie ma (bez MCP)

| Brak dostępu | Uwagi |
|---|---|
| ❌ Copilot Spaces API | Preview — brak publicznego API |
| ❌ Railway API | Deployment, logi — wymaga Railway MCP |
| ❌ Telegram Bot API | Bezpośrednie akcje — wymaga Telegram MCP |
| ❌ Groq API | Modele — brak MCP |
| ❌ Hugging Face API | Modele/obrazy — wymaga HF MCP |
| ❌ KuCoin API | Krypto — brak MCP |
| ❌ Brave Search API | Tylko przez kod w GeNCorE — wymaga Brave MCP |

## Privacy

- **Suggestions matching public code:** ✅ Allowed
- **Allow data for product improvements:** ✅ Enabled (ptaszek — domyślne)
- **Allow data for AI model training:** ❌ Disabled (świadoma decyzja)

## Setup (iPhone iOS)

> Trzy siostrzane appki (Source Remote, FTP Servers, S3 Servers) — ta sama idea, różne protokoły: zdalny zasób dostępny jak lokalny dysk w Files app.

| App | Do czego |
|-----|---------|
| **GitHub app** | Przeglądanie repo, Copilot Chat ✅ główny |
| **Working Copy** | Git (commit, push, pull) ✅ główny |
| **Textastic** | Edytor kodu ✅ główny |
| **Shellfish** | Terminal SSH na iOS 🔥 |
| **Railway app** | Deployment, logi Railway ✅ |
| **Code app** | Edytor kodu (alternatywa dla Textastic) |
| **FTP Servers** | Dostęp do serwerów FTP/SFTP bezpośrednio w Files app — jak lokalny dysk |
| **S3 Servers** | Dostęp do bucketów AWS/S3 bezpośrednio w Files app — jak lokalny dysk |
| **Source Remote** | Dostęp do repo Git (GitHub, GitLab, Gitea, BitBucket) w Files app bez klonowania |
| **Station** | TBD |
| **Brave** | Przeglądarka |

- ⚠️ GitHub app czasem wyrzuca sesję — po powrocie wracamy do `cli` repo jako kontekst
- 💡 Railway app + Shellfish = dostęp do Railway bez MCP!

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
- Sources w Space — do dodania ręcznie (brak API) ⏳
- MCP Servers — zbadane: Railway ✅, HF ✅, Telegram ✅, Brave ✅, Groq ❌, KuCoin ❌
- Kolejność konfiguracji MCP: Railway → HF → Telegram → Brave
- Dodano tabelkę "Czego Copilot nie ma bez MCP"
- Copilot API — nie istnieje publicznie ❌
- Sprawdzono wszystkie ustawienia Copilot — wszystko ✅ Enabled
- AI model training — ❌ Disabled (świadoma decyzja)
- Product improvements — ✅ Enabled (ptaszek, domyślne)
- Premium requests: 49.8% wykorzystane
- GitHub app wyrzuca sesję — dodano notatkę do Setup
- Copilot-generated commit messages — ✅ Enabled
- Pełny arsenał iOS apps: GitHub, Working Copy, Textastic, Shellfish, Railway app, Code, FTP Servers, S3 Servers, Source Remote, Station, Brave
- Railway app + Shellfish = dostęp do Railway bez MCP ✅
- Usunięto błędną linię z commit message wklejoną przez Claude Opus
- Zaktualizowano opisy 3 appek w Setup: Source Remote, FTP Servers, S3 Servers — rodzina siostrzanych appek (ta sama idea, różne protokoły)