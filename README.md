# RSB Webapps – Template

Ein fertig eingerichtetes Dashboard, mit dem du interaktive HTML-Lern-Apps direkt im Browser erstellen, bearbeiten und per GitHub Pages veröffentlichen kannst – ohne Backend, ohne Build-System.

---

## Schnellstart (5 Minuten)

### Schritt 1 – Eigenes Repository erstellen

Klicke oben rechts auf **"Use this template"** → **"Create a new repository"**.

- Vergib einen Namen, z. B. `meine-webapps`
- Sichtbarkeit: **Public** (wird für GitHub Pages benötigt)
- Klicke auf **"Create repository"**

---

### Schritt 2 – GitHub Pages aktivieren

In deinem neuen Repository:

1. **Settings** → **Pages**
2. Unter *Branch* → `main` auswählen, Ordner `/root` lassen
3. **Save** klicken
4. Nach ca. 1 Minute ist das Dashboard erreichbar unter:
   `https://<dein-nutzername>.github.io/<repo-name>/`

---

### Schritt 3 – GitHub Token erstellen

Das Dashboard benötigt einen Token, um Apps in deinem Repository zu speichern.

1. Gehe zu [GitHub → Settings → Developer Settings → Fine-grained Tokens](https://github.com/settings/tokens?type=beta)
2. Klicke auf **"Generate new token"**
3. Vergib einen Namen (z. B. `webapps-token`) und ein Ablaufdatum
4. Unter **Repository access** → nur dein neues Repository auswählen
5. Unter **Permissions → Repository permissions** → `Contents` auf **Read and write** setzen
6. Token generieren und kopieren (nur einmal sichtbar!)

---

### Schritt 4 – Dashboard konfigurieren

1. Öffne dein Dashboard: `https://<dein-nutzername>.github.io/<repo-name>/`
2. Klicke oben rechts auf das **Zahnrad-Symbol**
3. Trage ein:
   - **GitHub-Benutzername** – dein GitHub-Username
   - **Repository-Name** – der Name des Repos aus Schritt 1
   - **Personal Access Token** – der Token aus Schritt 3
   - **Anthropic API Key** *(optional)* – für automatische KI-Beschreibungen
4. Einstellungen speichern

---

### Schritt 5 – Erste App erstellen

1. Dateiname eingeben (z. B. `meine-app`)
2. HTML/CSS/JS im Editor schreiben
3. Optional: **Vorschau** anzeigen lassen
4. **Deploy** klicken – die App ist sofort erreichbar unter:
   `https://<dein-nutzername>.github.io/<repo-name>/apps/meine-app.html`

---

## Features

- **Code-Editor** – CodeMirror 5 mit Syntax-Highlighting und Dracula-Theme
- **Live-Vorschau** – Sandboxed Iframe vor dem Deployment
- **Ein-Klick-Deploy** – direkt auf GitHub Pages via REST API
- **App-Verwaltung** – Bearbeiten, Löschen, Metadaten pflegen
- **Suche & Filter** – nach Fach, Kategorie, Stichwort
- **QR-Codes** – für jede App zum Teilen (z. B. im Unterricht)
- **KI-Beschreibungen** – automatische Metadaten via Claude API *(optional)*

---

## Projektstruktur

```
meine-webapps/
├── index.html          # Dashboard (Single-Page-App)
├── descriptions.json   # Metadaten der Apps (wird automatisch befüllt)
├── apps/               # Hier landen deine veröffentlichten Apps
└── README.md
```

---

## Basiert auf

Dieses Template basiert auf [rsb-webapps](https://github.com/fbinder14/rsb-webapps) der Realschule Bobingen.
