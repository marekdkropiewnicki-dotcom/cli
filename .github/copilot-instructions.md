## 🖥️ Copilot CLI

Zainstalowany w Shellfish na iPhone. Uzupełnia GitHub app — ten sam `copilot-instructions.md`, zero duplikacji.

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

### Powiązanie z GeNCorE
- CLI czyta `.github/copilot-instructions.md` — **ten sam plik co GitHub app** ✅
- `GITHUB_TOKEN` ustawiony → auth automatyczny ✅
- Model domyślny: Claude Sonnet 4.5
- GitHub MCP wbudowany → dostęp do GeNCorE repo bezpośrednio z terminala

### Powiązanie z gh cli
- `marekdkropiewnicki-dotcom/cli` = fork `cli/cli` (Go)
- Workspace Copilota na iOS
- Branch: `trunk`