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

## Subskrypcje

Wszystkie kluczowe serwisy są na płatnych planach:

| Serwis | Plan |
|--------|------|
| **GitHub** | Copilot Pro+ |
| **Groq** | Pro |
| **Hugging Face** | Pro |
| **Railway** | Pro |
| **Telegram** | Pro + Biznes |
| **KuCoin** | Level 1 (zweryfikowany) |
| **Brave** | Pro |
| **Discord** | Pro |
| **Gravatar** | Pro (opłacony przez WordPress) |

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
- **Sources:** `marekdkropiewnicki-dotcom/GentelmeN-CorE` ✅
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

### Aktywne MCP (`mcp.json`)

| Serwer | Typ | Endpoint / Package | Secrets |
|---|---|---|---|
| `github` | `sse` | `https://mcp.github.com/mcp` | — |
| `brave-search` | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` |
| `huggingface` | `sse` | `https://hf.co/mcp/sse` | `HUGGINGFACE_API_KEY` |
| `context7` | `stdio` | `@upstash/context7-mcp` | — |
| `telegram` | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID`, `TELEGRAM_API_HASH` |
| `discord` | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` |

### Brak MCP — obsługa alternatywna

| Serwis | Powód | Alternatywa |
|---|---|---|
| **Railway** | Brak MCP w `mcp.json` | Railway app + Shellfish (iOS) 💡 |
| **Groq** | Brak publicznego MCP | Bezpośrednie API w kodzie |
| **KuCoin** | Brak publicznego MCP | Bezpośrednie API via ccxt |

### Czego Copilot nie ma

| Brak dostępu | Uwagi |
|---|---|
| ❌ Copilot Spaces API | Preview — brak publicznego API |
| ❌ Groq MCP | Brak oficjalnego MCP |
| ❌ KuCoin MCP | Brak oficjalnego MCP |

## Privacy

- **Suggestions matching public code:** ✅ Allowed
- **Allow data for product improvements:** ✅ Enabled (domyślne)
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
- Workspace `cli` skonfigurowany jako główny kontekst Copilota
- GeNCorE aktywny (PR #7 otwarty — naming, HF 410, voice routing)
- Copilot Pro+ skonfigurowany: agents (Copilot + Claude + Codex), Memory, MCP, Spaces ✅
- Space GentelmeN-CorE: model Claude Opus 4.6, instructions dodane ✅, sources dodane ✅
- MCP zbadane: Railway/HF/Telegram/Brave ✅ | Groq/KuCoin ❌ (brak MCP)
- Pełny arsenał iOS: GitHub, Working Copy, Textastic, Shellfish, Railway app, Code, FTP Servers, S3 Servers, Source Remote, Station, Brave
- Subskrypcje zapisane: GitHub/Groq/HF/Railway/Telegram/KuCoin/Brave/Discord/Gravatar — wszystkie Pro ✅
- Opisy siostrzanych appek (Source Remote, FTP Servers, S3 Servers) zaktualizowane ✅

### 2026-03-06
- `.github/mcp.json` stworzony ✅
- MCP skonfigurowane: github ✅ | brave-search ✅ | huggingface ✅ | context7 ✅ | telegram ✅ | discord ✅
- Railway — brak MCP, obsługa via Railway app + Shellfish (iOS) 💡
- Groq/KuCoin — brak MCP, bezpośrednie API w kodzie
- `NOTES.md` — posprzątany, spójny, estetyczny ✅
- `copilot-instructions.md` — zaktualizowany i zsynchronizowany z `mcp.json` ✅
- Sync zweryfikowany (2026-03-06)