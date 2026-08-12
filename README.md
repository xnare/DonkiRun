# Donki Run 🫏

Ein kleines Jump'n'Run: Ein Esel geht auf Reisen durch Österreich, London, Norwegen und Japan.
Weiche Erpeln und Riesen-Hippos aus und fang bunte Schmetterlinge für Punkte.

Tippen = springen, nochmal tippen = Doppelsprung.

---

## Auf GitHub Pages hochladen

### 1. Repository anlegen
1. Auf [github.com](https://github.com) einloggen (oder kostenlos registrieren).
2. Oben rechts auf **+** → **New repository**.
3. Name z. B. `donki-run` eingeben, **Public** auswählen, dann **Create repository**.

### 2. Dateien hochladen
1. Im leeren Repository auf **uploading an existing file** klicken
   (oder **Add file** → **Upload files**).
2. **Alle** Dateien aus diesem Ordner hineinziehen:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icon-180.png`
   - `icon-192.png`
   - `icon-512.png`
   - `icon-512-maskable.png`
   
   Die `README.md` kannst du mitnehmen, ist aber nicht nötig.
3. Unten auf **Commit changes** klicken.

### 3. Pages aktivieren
1. Im Repository oben auf **Settings**.
2. Links auf **Pages**.
3. Bei **Source** die Option **Deploy from a branch** wählen.
4. Bei **Branch** `main` auswählen, Ordner `/ (root)` lassen, **Save**.
5. Kurz warten (1–2 Minuten). Oben erscheint dann die Adresse, etwa:
   `https://DEINNAME.github.io/donki-run/`

---

## Aufs iPhone zum Homescreen hinzufügen

1. Die Pages-Adresse in **Safari** öffnen (nicht Chrome – das Homescreen-Feature
   funktioniert am iPhone nur über Safari).
2. Unten auf das **Teilen-Symbol** tippen (Quadrat mit Pfeil nach oben).
3. **Zum Home-Bildschirm** wählen.
4. Name bestätigen → **Hinzufügen**.

Fertig. Das Esel-Icon liegt jetzt am Homescreen und startet im Vollbild –
ohne Safari-Leiste, wie eine echte App. Dank Offline-Cache läuft es auch
ohne Internet, sobald es einmal geladen wurde.

---

## Etwas ändern?

Alles steckt in `index.html`. Nach einer Änderung die Datei bei GitHub neu
hochladen (überschreiben). Damit die Homescreen-App die neue Version sicher
zieht, in `sw.js` die Zeile `const CACHE = 'donki-run-v1';` auf `v2`, `v3` …
hochzählen.
