# /brief-lite — Content Brief w 15 minut

Skill, który zamienia aktualne newsy z Twojej branży w gotowy post na LinkedIn.

**Bez kopiuj-wklej. Bez AI-owej papki. Twoje słowa, Twój głos.**

## Jak to działa?

1. AI szuka newsów z Twojej branży (ostatnie 24h)
2. Wybierasz temat, który Cię ciągnie
3. AI zadaje 3-4 pytania — wyciąga Twoją perspektywę
4. Gotowy post napisany Twoimi słowami

Cały proces: ~15 minut.

---

## Instalacja

Skill działa z **Claude Code** i **Gemini CLI**. Wybierz swoje narzędzie:

### Opcja A: Claude Code

<details>
<summary><strong>macOS / Linux</strong></summary>

**1. Zainstaluj Claude Code** (jeśli nie masz):
```bash
npm install -g @anthropic-ai/claude-code
```
Nie masz npm? Zainstaluj [Node.js](https://nodejs.org/) (wersja 18+) — npm jest w pakiecie.

**2. Pobierz skill:**
```bash
mkdir -p ~/.claude/commands
curl -o ~/.claude/commands/brief-lite.md https://raw.githubusercontent.com/studiogo/brief-lite/main/SKILL.md
```

**3. Uruchom:**
```bash
claude
```
W Claude Code wpisz:
```
/brief-lite
```
</details>

<details>
<summary><strong>Windows</strong></summary>

**1. Zainstaluj Node.js:**
- Pobierz z [nodejs.org](https://nodejs.org/) (wersja 18+)
- Uruchom instalator, klikaj "Next" — npm zainstaluje się automatycznie

**2. Zainstaluj Claude Code:**

Otwórz **PowerShell** (kliknij prawym na Start → "Terminal" lub "PowerShell"):
```powershell
npm install -g @anthropic-ai/claude-code
```

**3. Pobierz skill:**
```powershell
mkdir -Force "$env:USERPROFILE\.claude\commands"
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/studiogo/brief-lite/main/SKILL.md" -OutFile "$env:USERPROFILE\.claude\commands\brief-lite.md"
```

**4. Uruchom:**
```powershell
claude
```
W Claude Code wpisz:
```
/brief-lite
```
</details>

---

### Opcja B: Gemini CLI

Gemini CLI od Google używa formatu TOML zamiast Markdown. W repozytorium jest gotowy plik `brief-lite.toml`.

<details>
<summary><strong>macOS / Linux</strong></summary>

**1. Zainstaluj Gemini CLI** (jeśli nie masz):
```bash
npm install -g @anthropic-ai/gemini-cli
```
Oficjalna instrukcja: [gemini CLI](https://github.com/google-gemini/gemini-cli)

**2. Pobierz skill:**
```bash
mkdir -p ~/.gemini/commands
curl -o ~/.gemini/commands/brief-lite.toml https://raw.githubusercontent.com/studiogo/brief-lite/main/brief-lite.toml
```

**3. Uruchom:**
```bash
gemini
```
W Gemini CLI wpisz:
```
/brief-lite
```
</details>

<details>
<summary><strong>Windows</strong></summary>

**1. Zainstaluj Node.js** z [nodejs.org](https://nodejs.org/) (wersja 18+)

**2. Zainstaluj Gemini CLI:**
```powershell
npm install -g @google/gemini-cli
```

**3. Pobierz skill:**
```powershell
mkdir -Force "$env:USERPROFILE\.gemini\commands"
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/studiogo/brief-lite/main/brief-lite.toml" -OutFile "$env:USERPROFILE\.gemini\commands\brief-lite.toml"
```

**4. Uruchom:**
```powershell
gemini
```
W Gemini CLI wpisz:
```
/brief-lite
```
</details>

---

## Wymagania

| Narzędzie | Konto | Koszt |
|-----------|-------|-------|
| Claude Code | [Anthropic API](https://console.anthropic.com/) lub subskrypcja Claude Max | API: pay-as-you-go (~$0.05/brief) |
| Gemini CLI | [Google AI Studio](https://aistudio.google.com/) | Darmowy tier dostępny |

---

## FAQ

**Nie znam się na terminalu. Dam radę?**
Tak. Kopiujesz 3 komendy, wklejasz w terminal, gotowe. Nie musisz nic programować.

**Muszę coś konfigurować?**
Tylko za pierwszym razem — skill zapyta o Twoją branżę (jedno zdanie). Potem pamięta.

**Czy mogę użyć tego z ChatGPT?**
Nie bezpośrednio — ChatGPT nie obsługuje custom commands. Ale możesz skopiować zawartość pliku `SKILL.md` i wkleić jako "Custom Instructions" lub system prompt w API.

**Czy to jest bezpieczne?**
Skill to plik tekstowy z instrukcjami dla AI. Nie instaluje żadnego oprogramowania, nie zbiera danych, nie łączy się z zewnętrznymi serwisami (poza wyszukiwarką newsów).

---

## Autor

Łukasz Hodorowicz — [LinkedIn](https://www.linkedin.com/in/lukaszhodorowicz/)

**/brief-lite to jeden z kilkunastu skilli mojego systemu do tworzenia contentu.**
Cały system — od pomysłu po publikację na 4 platformach — buduję na warsztatach.
Jeśli chcesz wiedzieć więcej, napisz do mnie na LinkedIn.
