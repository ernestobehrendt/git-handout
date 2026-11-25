<div align="center">

# 🌱 git-handout

### Handout & Hands-on zum Vortrag
**„Git – The information manager from hell."**

[![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)](https://git-scm.com)
[![Account](https://img.shields.io/badge/GitHub--Account-nicht%20n%C3%B6tig-success)](#-hands-on)
[![Handout](https://img.shields.io/badge/📄-Handout-orange)](handout/GIT-HANDOUT.md)

Ernesto Behrendt · OSZ Technik Teltow · 25.11.2026

</div>

---

## Hands-on

> **Aufgabe:** Clone dieses Repository und committe ein Kompliment zum Vortrag.
> 🔑 GitHub-Account: nicht nötig

| Schritt | Was passiert | Befehl |
| :---: | --- | --- |
| **1** | Repository klonen | `git clone` |
| **2** | Kompliment-Datei anlegen | Vorlage kopieren |
| **3** | Änderung committen | `git add` · `git commit` |
| **4** | Ergebnis ansehen | `git log` |

---

### 1️⃣ Repository klonen

```bash
git clone https://github.com/OWNER/git-handout.git
cd git-handout
```

### 2️⃣ Kompliment-Datei anlegen

Kopiere die Vorlage und ersetze `DEIN-NAME` durch deinen Namen:

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

Öffne die Datei `kudos/DEIN-NAME.md` in einem Editor und schreibe dein Kompliment.

### 3️⃣ Committen

```bash
git add kudos/DEIN-NAME.md
git commit -m "kudos: Kompliment von DEIN-NAME"
```

### 4️⃣ Ergebnis ansehen

```bash
git log --oneline
```

> ✅ **Geschafft!** Dein Commit steht ganz oben in der Historie.

> [!TIP]
> Bei der Meldung **„Author identity unknown"** einmalig Name und Mailadresse setzen:
> ```bash
> git config --global user.name "Dein Name"
> git config --global user.email "deine@mail.de"
> ```

---

## ⭐ Bonus: Veröffentlichen

Schon fertig? Mit einem GitHub-Account kannst du deinen Commit hochladen:

1. Repository oben rechts **forken**
2. Statt des Originals **deinen Fork** klonen
3. Nach dem Commit `git push` ausführen
4. Auf GitHub einen **Pull Request** öffnen

---

## 🧭 Merkhilfe

```mermaid
flowchart LR
    A[Datei ändern] -->|git add| B[Staging Area]
    B -->|git commit| C[Lokales Repository]
    C -->|git push| D[GitHub]
```

---

## 📚 Mehr zu Git

- 📄 [Handout / Cheat Sheet](handout/GIT-HANDOUT.md)
- 📘 [Pro Git (kostenlos, deutsch)](https://git-scm.com/book/de/v2)
- 📖 [Offizielle Dokumentation](https://git-scm.com/docs)

<div align="center">

**Danke fürs Mitmachen und viel Spaß mit Git! 🚀**

</div>
