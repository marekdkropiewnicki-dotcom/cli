# 🤖 Copilot Instructions — marekdkropiewnicki-dotcom/cli

---

## ⚡ @sync — Szybki status

| | |
|---|---|
| 📅 **Data** | 2026-03-06 |
| 📱 **Urządzenie** | iPhone 16 — tylko iOS |
| 🌿 **Branch** | `trunk` |
| 🟢 **Stan** | Wszystko gotowe i zsynchronizowane |

**MCP:** `github` ✅ `brave-search` ✅ `huggingface` ✅ `context7` ✅ `telegram` ✅ `discord` ✅
**Railway** → Railway app + Shellfish 💡 | **Groq / KuCoin** → bezpośrednie API w kodzie

> ⚠️ GitHub app na iOS resetuje kontekst — po powrocie wpisz `@sync`

---

## 🗂️ O tym repo

To repozytorium (`cli`) służy jako **główny workspace** do codziennej pracy na iPhone (iOS).
Jest to fork oficjalnego GitHub CLI (`gh`), napisanego w Go.

- **Właściciel:** marekdkropiewnicki-dotcom
- **Device:** iPhone (iOS) — wszystkie sesje prowadzone na iOS
- **Branch:** `trunk`

---

## 🚀 Główny projekt: GeNCorE

**Repo:** `marekdkropiewnicki-dotcom/GentelmeN-CorE`

| Komponent | Technologia |
|---|---|
| Telegram bot | Python (`python-telegram-bot`) |
| AI chat | Groq (`llama-3.3-70b-versatile`, `llama-3.1-8b-instant`, `qwen-2.5-32b`) |
| Generowanie obrazów | Hugging Face |
| Kryptowaluty | KuCoin via `ccxt` |
| Wyszukiwanie | Brave Search API |
| Deployment | Railway |

---

## 👥 Team AI

| Kto | Rola |
|---|---|
| 👨 Marek | Pomysłodawca, developer |
| 🤖 GitHub Copilot | Kod, PR, GitHub, Chat |
| 🧠 Claude (Anthropic) | Coding agent — włączony |
| ⚡ Codex | Coding agent — włączony |

---

## 💳 Subskrypcje

| Serwis | Plan |
|---|---|
| **GitHub** | Copilot Pro+ |
| **Groq** | Pro |
| **Hugging Face** | Pro |
| **Railway** | Pro |
| **Telegram** | Pro + Biznes |
| **KuCoin** | Level 1 (zweryfikowany) |
| **Brave** | Pro |
| **Discord** | Pro |
| **Gravatar** | Pro (opłacony przez WordPress) |

---

## ⚙️ Copilot Setup

| Funkcja | Stan |
|---|---|
| Plan | Copilot Pro+ |
| Premium requests | ~49.8% wykorzystane (reset 1. dnia miesiąca) |
| Coding agent — Copilot | ✅ Włączony |
| Coding agent — Claude | ✅ Włączony |
| Coding agent — Codex | ✅ Włączony |
| Automatic code review | ✅ Enabled |
| Copilot Memory | ✅ Enabled (Preview) |
| MCP servers | ✅ Enabled |
| Copilot Spaces | ✅ Enabled |
| Copilot-generated commit messages | ✅ Enabled |
| AI model training | ❌ Disabled (świadoma decyzja) |

---

## 🌌 Copilot Spaces

| | |
|---|---|
| **Space** | GentelmeN-CorE |
| **Model** | Claude Opus 4.6 |
| **Sources** | `marekdkropiewnicki-dotcom/GentelmeN-CorE` |
| **Link** | https://github.com/copilot/spaces |

**Instructions (Space):**

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

---

## 🔌 MCP Servers

### Aktywne (`mcp.json`)

| Serwer | Typ | Endpoint / Package | Secrets |
|---|---|---|---|
| `github` | `sse` | `https://mcp.github.com/mcp` | — |
| `brave-search` | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` |
| `huggingface` | `sse` | `https://hf.co/mcp/sse` | `HUGGINGFACE_API_KEY` |
| `context7` | `stdio` | `@upstash/context7-mcp` | — |
| `telegram` | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID`, `TELEGRAM_API_HASH` |
| `discord` | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` |

### Brak MCP — obsługa alternatywna

| Serwis | Alternatywa |
|---|---|
| **Railway** | Railway app + Shellfish (iOS) 💡 |
| **Groq** | Bezpośrednie API w kodzie |
| **KuCoin** | Bezpośrednie API via `ccxt` |

### Secrets (repo)

`SMITHERY_API_KEY` · `HUGGINGFACE_API_KEY` · `DISCORD_BOT_TOKEN` · `TELEGRAM_API_ID` · `TELEGRAM_API_HASH` · `BRAVE_API_KEY`

> Wszystkie klucze w secrets — brak plain text. Secret scanning zaakceptowany.

---

## 📱 iOS Setup

> 💡 Trzy siostrzane appki (Source Remote, FTP Servers, S3 Servers) — ta sama idea, różne protokoły: zdalny zasób dostępny jak lokalny dysk w Files app.

| App | Rola |
|---|---|
| **GitHub app** | Przeglądanie repo, Copilot Chat — główny |
| **Working Copy** | Git: commit, push, pull — główny |
| **Textastic** | Edytor kodu — główny |
| **Shellfish** | Terminal SSH 🔥 |
| **Railway app** | Deployment, logi Railway |
| **Code app** | Edytor kodu (alternatywa) |
| **Source Remote** | Dostęp do repo Git w Files app bez klonowania |
| **FTP Servers** | Dostęp do FTP/SFTP w Files app |
| **S3 Servers** | Dostęp do AWS/S3 w Files app |
| **Brave** | Przeglądarka |
| **Station** | TBD |

---

## 🤝 Zasady współpracy

- Komunikacja po **polsku** 🇵🇱
- Krótkie, konkretne odpowiedzi — bez zbędnego gadania
- Jeden wybór na raz — nie przytłaczaj opcjami
- Pracujemy na iPhone — zero narzędzi desktopowych
- Główna gałąź: `trunk`

---

## 📋 Session History

### 2026-03-05
- Workspace `cli` skonfigurowany jako główny kontekst Copilota
- GeNCorE aktywny (PR #7 — naming, HF 410, voice routing)
- Copilot Pro+ skonfigurowany: agents, Memory, MCP, Spaces ✅
- Space GentelmeN-CorE: Claude Opus 4.6, instructions + sources ✅
- Pełny arsenał iOS udokumentowany ✅
- Subskrypcje zapisane: wszystkie Pro ✅

### 2026-03-06
- `.github/mcp.json` stworzony ✅
- 6 serwerów MCP skonfigurowanych ✅
- Railway / Groq / KuCoin — alternatywy udokumentowane ✅
- `copilot-instructions.md` + `NOTES.md` scalone w jeden plik ✅
- `copolitan-instructions.md` (literówka iOS) — wyczyszczony ✅
- Struktura `.github/` uporządkowana ✅

### 2026-03-09

- Repo GentelmeN-CorE upublicznione ✅
- 5 pustych WIP PRów (#8–#12) zamkniętych, branche usunięte ✅
- Root cause PRów: Railway log error (nie był błędem kodu) ✅
- Copilot premium limit wyczerpany — agenci zatrzymani ✅
- Przegląd inspiracji: freeCodeCamp, gh cli fork, first-contributions ✅
- Wizja: GeNCorE → suwerenna AI (RAG, orkiestracja, autonomia) 🎯