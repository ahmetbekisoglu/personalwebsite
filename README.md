# Website Ahmet Bekisoglu (minimalistische Version)

Statische Website: eine HTML-Datei pro Seite, kein Build, keine Abhängigkeiten.

## Auf GitHub Pages veröffentlichen (einmalig)

1. Auf github.com anmelden, oben rechts **+** → **New repository**.
   Name z. B. `website`, **Public**, Häkchen bei „Add a README" **nicht** setzen → **Create repository**.
2. Auf der leeren Repository-Seite auf **uploading an existing file** klicken.
3. Den kompletten Inhalt dieses Ordners (alle Dateien und den Ordner `logos`) ins Browserfenster ziehen.
   Wichtig: den Inhalt ziehen, nicht den Ordner selbst. Versteckte Dateien `.nojekyll` und `.gitignore` mitnehmen.
4. Unten **Commit changes** klicken.
5. Im Repository auf **Settings** → links **Pages** → unter „Build and deployment" bei **Branch** `main` und `/ (root)` wählen → **Save**.
6. Nach ein bis zwei Minuten steht die Adresse oben auf der Pages-Seite: `https://DEINNAME.github.io/website/`

## Eigene Domain (optional)

1. In **Settings → Pages** unter „Custom domain" die Domain eintragen, z. B. `ahmetbekisoglu.de`, und speichern.
2. Beim Domain-Anbieter im DNS anlegen:
   - `A`-Einträge für `@` auf `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` für `www` auf `DEINNAME.github.io`
3. Zurück in den Pages-Einstellungen **Enforce HTTPS** aktivieren, sobald das Häkchen grün ist.

## Änderungen später

Datei im Repository anklicken → Stift-Symbol → bearbeiten → **Commit changes**. Die Seite aktualisiert sich innerhalb einer Minute.
Oder lokal ändern und die Datei erneut per **Add file → Upload files** hochladen; gleiche Dateinamen werden ersetzt.

## Vor dem Go-live ausfüllen

- `index.html`: E-Mail-Adresse – alle Vorkommen von `mail@platzhalter.de` ersetzen (Formate, Kontakt, JSON-LD oben im Kopf), absolute URL für `og:image`
- `impressum.html` und `datenschutz.html`: alle gelb markierten Stellen, danach die gelben Hinweisboxen löschen
