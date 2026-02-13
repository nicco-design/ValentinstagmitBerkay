# Valentinstag Website

Diese Seite ist für **GitHub Pages** vorbereitet.

## Deployment über GitHub Pages

1. Repository auf GitHub pushen.
2. In GitHub zu **Settings → Pages** gehen.
3. Bei **Build and deployment** auswählen:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (oder dein Branch)
   - **Folder:** `/ (root)` **oder** `/docs`
4. **Save** klicken.
5. Nach dem Speichern zeigt GitHub oben den Live-Link an: `Your site is live at ...`.

## Wo ist die URL?

Die URL hängt vom Repo-Typ ab:

- **User/Org-Repo** (Name exakt `<user>.github.io`):
  - `https://<user>.github.io/`
- **Projekt-Repo** (z. B. `Valentinstag-Final`):
  - `https://<user>.github.io/<repo>/`
  - Beispiel: `https://maxmustermann.github.io/Valentinstag-Final/`

> Hinweis: Die Auswahl `/ (root)` oder `/docs` ändert nur den Veröffentlichungsordner, nicht das URL-Schema.

## Falls weiterhin 404 kommt

- Prüfen, ob der richtige Branch veröffentlicht wird.
- Prüfen, ob die Projekt-URL korrekt ist: `https://<user>.github.io/<repo>/`
- In **Settings → Pages** prüfen, ob die Seite als "live" angezeigt wird.
- Nach Änderungen 1–2 Minuten warten (Pages-Deploy kann kurz dauern).

## Merge-Konflikte vermeiden

Falls beim Mergen Konfliktmarker wie `<<<<<<<`, `=======`, `>>>>>>>` auftauchen:

1. Konfliktmarker entfernen.
2. Nur eine finale Version des betroffenen Abschnitts stehen lassen.
3. Mit `git add README.md` markieren und committen.

Prüfen mit:

```bash
rg -n "^(<<<<<<<|=======|>>>>>>>)" README.md
```
