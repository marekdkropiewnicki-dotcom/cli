# 🤖 Copilot Instructions — marekdkropiewnicki-dotcom/cli

---

## ⚡ @sync — Szybki status

| | |
|---|---|
| 📅 **Data ostatniego sync** | 2026-04-01 |
| 📱 **Urządzenie** | iPhone 16 — tylko iOS |
| 🌿 **Branch (cli)** | `trunk` |
| 🟢 **Stan** | Zsynchronizowane ✅ |

**MCP:** `github` ✅ `brave-search` ✅ `huggingface` ✅ `context7` ✅ `telegram` ✅ `discord` ✅
**Railway** → Railway app + Shellfish 💡 | **Groq / KuCoin** → bezpośrednie API w kodzie

> ⚠️ GitHub app na iOS resetuje kontekst — po powrocie wpisz `@sync`

---

## 🗺️ MAPA PROJEKTÓW — gdzie jesteśmy

### 🥇 Priorytet 1 — GeNCorE (działa na produkcji)
> Telegram bot na Railway. Fundament wszystkiego.

**Repo:** `marekdkropiewnicki-dotcom/GentelmeN-CorE`
**Branch główny:** `GentelmeN@CorE`

🟢 **Bugi:**
- `/rysuj` — 410 error → ✅ Naprawiony (SDXL → FLUX.1-schnell, commit `ac1f084`)
- Voice → `/rysuj` routing → ✅ Już działało (zweryfikowane)

🌿 **Branche:**
- Tylko 1 branch: `GentelmeN@CorE` ✅
- 5 branchy `copilot/*` → ✅ Usunięte przez Marka (2026-04-01)

🎯 **Stan GeNCorE:**
- Stabilny, produkcja działa ✅

---

### 🥈 Priorytet 2 — claude-remote-control (w budowie)
> Panel webowy do sterowania agentami AI. Budowany na Vercelu.

**Repo:** `marekdkropiewnicki-dotcom/claude-remote-control`
**Live:** https://claude-remote-control-gilt.vercel.app
**Stack:** Next.js + Tailwind CSS + Vercel

💡 **Wizja (ustalona 2026-04-01):**
Jeden panel — trzy zakładki:
- 💬 Chat z Claude AI
- 🤖 Zlecaj zadania agentom (Copilot / Claude / Codex)
- 🔀 Przeglądaj i merguj PR-y GeNCorE

🔗 **Powiązania z innymi projektami:**
- GeNCorE bot → komendy `/pr lista`, `/zadanie`, `/deploy` przez Telegram
- cli/gh → GitHub CLI operacje z Shellfish

📋 **Stan PRów:**
- PR #1 (Claude) — Chat z Claude AI, Next.js 15 — Draft ⏳
- PR #2 (Copilot) — Command Center, Next.js 14 + Tailwind — Draft ⏳

🎯 **Następny krok:**
1. Merge PR #1 (Claude) → `main` jako fundament
2. Rozbudowa o zakładki Agenci + PR-y

⚙️ **Env vars do ustawienia w Vercel:**
```
GITHUB_TOKEN=
ADMIN_TOKEN=
NEXT_PUBLIC_REPO_OWNER=marekdkropiewnicki-dotcom
NEXT_PUBLIC_REPO_NAME=GentelmeN-CorE
```

---

### 🥉 Priorytet 3 — cli/gh (workspace + przyszłość)
> Fork GitHub CLI. Teraz: główny workspace Copilota. Przyszłość: integracja z panelem.

**Repo:** `marekdkropiewnicki-dotcom/cli`
**Branch:** `trunk`

---

### 🔮 Wizja długoterminowa (NIE TERAZ)
> Zapisane żeby nie zgubić — wrócimy gdy będzie gotowa podstawa.

- GeNCorE Token — własna kryptomoneta, dostęp do premium funkcji bota
- GeNCorE jako AI dla monety — trading, analiza, doradztwo
- Ekosystem: claude-remote-control ↔ GeNCorE ↔ cli/gh

---

## 🚦 Zasada pracy — JEDEN KROK NA RAZ

```
Aktualny focus → claude-remote-control (GeNCorE jest stabilny ✅)
NIE robimy wszystkiego naraz
NIE skaczemy do wizji długoterminowej
```

Jeśli Marek się gubi → pokaż tę mapę i zapytaj o jeden priorytet.

---

## 🗂️ O tym repo (cli)

Fork oficjalnego GitHub CLI (`gh`), napisanego w Go.
Służy jako **główny workspace** Copilota na iOS.

- **Właściciel:** marekdkropiewnicki-dotcom
- **Device:** iPhone 16 (iOS) — wszystkie sesje na iOS
- **Branch:** `trunk`

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
| Premium requests | reset 2026-04-01 |
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

---

## 🔌 MCP Servers

| Serwer | Typ | Endpoint / Package | Secrets |
|---|---|---|---|
| `github` | `sse` | `https://mcp.github.com/mcp` | — |
| `brave-search` | `sse` | `https://server.smithery.ai/@arjunkmrm/brave-search-mcp-server/mcp` | `SMITHERY_API_KEY` |
| `huggingface` | `sse` | `https://hf.co/mcp/sse` | `HUGGINGFACE_API_KEY` |
| `context7` | `stdio` | `@upstash/context7-mcp` | — |
| `telegram` | `stdio` | `mcp-telegram` | `TELEGRAM_API_ID`, `TELEGRAM_API_HASH` |
| `discord` | `stdio` | `@scarecr0w12/discord-mcp` | `DISCORD_BOT_TOKEN` |

**Brak MCP:**
- Railway → Railway app + Shellfish
- Groq / KuCoin → bezpośrednie API w kodzie

---

## 📱 iOS Setup

| App | Rola |
|---|---|
| **GitHub app** | Przeglądanie repo, Copilot Chat |
| **Working Copy** | Git: commit, push, pull |
| **Textastic** | Edytor kodu |
| **Shellfish** | Terminal SSH 🔥 |
| **Railway app** | Deployment, logi |
| **Code app** | Edytor kodu (alternatywa) |
| **Source Remote** | Repo Git w Files app |
| **FTP Servers** | FTP/SFTP w Files app |
| **S3 Servers** | AWS/S3 w Files app |
| **Brave** | Przeglądarka |

---

## 🤝 Zasady współpracy

- Komunikacja po **polsku** 🇵🇱
- Krótkie, konkretne odpowiedzi
- **Jeden krok na raz** — nie przytłaczaj opcjami
- Pracujemy na iPhone — zero narzędzi desktopowych
- Jeśli Marek się gubi → wróć do mapy projektów

---

## 📋 Session History

### 2026-03-05
- Workspace `cli` skonfigurowany jako główny kontekst Copilota ✅
- GeNCorE aktywny, Copilot Pro+ skonfigurowany ✅

### 2026-03-06
- `.github/mcp.json` stworzony, 6 serwerów MCP ✅
- `copilot-instructions.md` + `NOTES.md` scalone ✅

### 2026-03-09
- Repo GentelmeN-CorE upublicznione ✅
- 5 pustych WIP PRów zamkniętych ✅

### 2026-03-13
- PR #14 (Codex) zmergowany — performance fixes ✅

### 2026-04-01
- Premium requests zresetowane — 100% ✅
- Bug #1 `/rysuj` naprawiony: SDXL → FLUX.1-schnell (`ac1f084`) ✅
- Bug #2 voice→/rysuj — zweryfikowany, już działał ✅
- 5 branchy `copilot/*` w GeNCorE → ✅ Usunięte przez Marka
- claude-remote-control: PR #1 (Claude) + PR #2 (Copilot) — Draft ⏳
- Wizja ekosystemu: GeNCorE + claude-remote-control + cli ✅
- Mapa projektów + zasada "jeden krok na raz" wdrożona 🗺️ ✅
- GeNCorE stabilny — focus przechodzi na claude-remote-control 🎯