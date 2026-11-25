<div align="center">

# git-handout

**Handout und Hands-on zum Vortrag**
*„Git – The information manager from hell."*

[![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white&style=flat-square)](https://git-scm.com)
[![Dauer](https://img.shields.io/badge/Dauer-ca.%203%20Min.-2b6cb0?style=flat-square)](#hands-on)
[![Account](https://img.shields.io/badge/GitHub--Account-nicht%20erforderlich-2f855a?style=flat-square)](#hands-on)

Ernesto Behrendt &nbsp;|&nbsp; OSZ Technik Teltow &nbsp;|&nbsp; 09.10.2026

[Handout](handout/GIT-HANDOUT.md) &nbsp;·&nbsp; [Hands-on](#hands-on) &nbsp;·&nbsp; [Ohne Installation](#ohne-git-installation-im-browser) &nbsp;·&nbsp; [Weiterlesen](#zum-weiterlesen)

</div>

---

## Hands-on

Aufgabe: Repository clonen und ein Kompliment zum Vortrag committen.

| Schritt | Beschreibung | Befehl |
| :---: | --- | --- |
| 1 | Repository klonen | `git clone` |
| 2 | Kompliment-Datei anlegen | Vorlage kopieren |
| 3 | Änderung committen | `git add`, `git commit` |
| 4 | Ergebnis ansehen | `git log` |

### Voraussetzung

Git muss installiert sein. Prüfen im Terminal:

```bash
git --version
```

> [!NOTE]
> Kommt eine Versionsnummer, kannst du loslegen. Andernfalls installierst du Git von
> [git-scm.com/downloads](https://git-scm.com/downloads) und startest das Terminal neu.
> Einen GitHub-Account brauchst du für diesen Teil nicht.

### 1. Repository clonen

```bash
git clone https://github.com/OWNER/git-handout.git
cd git-handout
```

### 2. Datei anlegen

Kopiere die Vorlage und nenne die Kopie nach dir (statt `DEIN-NAME` z. B. `max`):

<details open>
<summary><b>Linux / macOS / Git Bash</b></summary>

```bash
cp kudos/_TEMPLATE.md kudos/DEIN-NAME.md
```

</details>

<details>
<summary><b>Windows (Eingabeaufforderung)</b></summary>

```bat
copy kudos\_TEMPLATE.md kudos\DEIN-NAME.md
```

</details>

Öffne die neue Datei in einem Editor und schreibe dein Kompliment hinein.

### 3. Committen

```bash
git add kudos/DEIN-NAME.md
git commit -m "Kompliment von DEIN-NAME"
```

> [!TIP]
> Fragt Git nach deiner Identität („Author identity unknown"), setze sie einmalig und wiederhole den Commit:
>
> ```bash
> git config --global user.name "Dein Name"
> git config --global user.email "deine@mail.de"
> ```

### 4. Ergebnis ansehen

```bash
git log --oneline
```

Dein Commit steht ganz oben in der Historie.

---

## Ohne Git-Installation (im Browser)

Mit einem GitHub-Account geht es auch ohne lokale Installation:

1. Dieses Repository über **Fork** (oben rechts) in dein Konto kopieren.
2. Im Ordner `kudos` über **Add file → Create new file** eine Datei `DEIN-NAME.md` anlegen und dein Kompliment schreiben.
3. Unten auf **Commit changes** klicken.

Das ist derselbe Commit, nur führt GitHub ihn für dich aus.

---

## Zum Weiterlesen

| Ressource | Beschreibung |
| --- | --- |
| [Handout](handout/GIT-HANDOUT.md) | Die wichtigsten Befehle auf einer Seite |
| [Pro Git](https://git-scm.com/book/de/v2) | Das offizielle Buch, kostenlos und auf Deutsch |
| [Dokumentation](https://git-scm.com/docs) | Referenz aller Befehle |

<div align="center">

<sub>Vielen Dank fürs Mitmachen.</sub>

</div>
