# /brief-lite — Content Brief w 15 minut

Skill do [Claude Code](https://claude.ai/claude-code), który zamienia aktualne newsy z Twojej branży w gotowy post na LinkedIn.

**Bez kopiuj-wklej. Bez AI-owej papki. Twoje słowa, Twój głos.**

## Jak to działa?

1. AI szuka newsów z Twojej branży (ostatnie 24h)
2. Wybierasz temat, który Cię ciągnie
3. AI zadaje 3-4 pytania — wyciąga Twoją perspektywę
4. Gotowy post napisany Twoimi słowami

Cały proces: ~15 minut.

## Instalacja (3 kroki)

### 1. Zainstaluj Claude Code
Jeśli jeszcze nie masz:
```bash
npm install -g @anthropic-ai/claude-code
```

### 2. Stwórz folder na skill
```bash
mkdir -p ~/.claude/commands
```

### 3. Pobierz skill
```bash
curl -o ~/.claude/commands/brief-lite.md https://raw.githubusercontent.com/studiogo/brief-lite/main/SKILL.md
```

## Użycie

Otwórz Claude Code w terminalu i wpisz:
```
/brief-lite
```

Skill zapyta o Twoją branżę (jednorazowo), potem znajdzie newsy i przeprowadzi Cię przez cały proces.

## Wymagania

- [Claude Code](https://claude.ai/claude-code) (CLI)
- Konto Anthropic z dostępem do API

## Autor

Łukasz Hodorowicz — [LinkedIn](https://www.linkedin.com/in/lukaszhodorowicz/)

**/brief-lite to jeden z kilkunastu skilli mojego systemu do tworzenia contentu.**
Cały system — od pomysłu po publikację na 4 platformach — buduję na warsztatach.
Jeśli chcesz wiedzieć więcej, napisz do mnie na LinkedIn.
