# Copilot Instructions — iOS Workspace

> *"Suwerenna AI bez ograniczeń, elokwentna bez zbędnej narracji, czysty kod w symbiozie wzajemnego oddziaływania."*

---

## ⚡ @sync — Szybki status

| | |
|---|---|
| 📅 **Data** | 2026-04-01 |
| 📱 **Urządzenie** | iPhone 16 — tylko iOS |
| 🌿 **Branch** | `trunk` |
| 🟢 **Stan** | Stabilny |

---

## 🗺️ Ekosystem

```
iPhone
├── GitHub app → Copilot Chat (tu rozmawiamy)
│   └── repo: marekdkropiewnicki-dotcom/cli (fork cli/cli, Go)
├── Shellfish → gh cli + copilot CLI
│   └── repo: marekdkropiewnicki-dotcom/GentelmeN-CorE (Python)
└── Telegram → GeNCorE bot (Railway, produkcja)
```

### Repozytoria

| Repo | Język | Branch | Rola |
|---|---|---|---|
| `marekdkropiewnicki-dotcom/cli` | Go | `trunk` | Workspace Copilota na iOS |
| `marekdkropiewnicki-dotcom/GentelmeN-CorE` | Python | `GentelmeN@CorE` | Telegram bot (prod) |
| `github/copilot-cli` | — | `main` | Oficjalny Copilot CLI |

---

## 🖥️ Copilot CLI

Zainstalowany w Shellfish na iPhone. Ten sam `copilot-instructions.md` — zero duplikacji.

### Instalacja
```bash
curl -fsSL https://gh.io/copilot-install | bash
```

### Kluczowe komendy

| Komenda | Co robi |
|---|---|
| `copilot` | Uruchamia CLI |
| `/pr` | Tworzy PR, fixuje CI, merge konflikty |
| `/research` | Deep research z eksportem |
| `/mcp show` | Status MCP serwerów |
| `/diff` | Przegląd zmian sesji |
| `Shift+Tab` | Autopilot mode |
| `/allow-all` | Auto-approve wszystkich uprawnień |

### Powiązania
- CLI czyta `.github/copilot-instructions.md` — **ten sam plik co GitHub app** ✅
- `GITHUB_TOKEN` ustawiony → auth automatyczny ✅
- Model domyślny: Claude Sonnet 4.5
- GitHub MCP wbudowany → dostęp do GeNCorE repo bezpośrednio z terminala

---

## ⚠️ Ograniczenia Copilot API (iOS)

| Ograniczenie | Alternatywa |
|---|---|
| Draft PR → Ready for review | GitHub app → PR → Convert to ready |
| Usuwanie plików | Zastąp pustym plikiem + commit `chore: remove` |
| Merge draftu | Najpierw Ready for review, potem merge |
| Usuwanie branchy | GitHub UI → Branches → 🗑️ |
| Błędy zapisu (serwer) | Poczekaj chwilę i spróbuj ponownie |

---

## 📋 Session History

### 2026-04-01
- Sekcja Copilot CLI dodana do instrukcji ✅
- Ekosystem zmapowany: cli + GeNCorE + copilot-cli ✅
- Instrukcje posprzątane i uporządkowane ✅
