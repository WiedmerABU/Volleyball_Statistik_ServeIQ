# ServeIQ 0.2 – GitHub Pages / Funktionstest

## Installieren / Aktualisieren auf GitHub
1. Dieses ZIP auf dem Laptop **entpacken**.
2. GitHub-Repository `ServeIQ` öffnen → **Code → Add file → Upload files**.
3. **Alle Dateien und den Ordner `icons` aus diesem entpackten Ordner** ins Stammverzeichnis des Repositorys hochladen. Vorhandene gleichnamige Dateien ersetzen.
4. **Commit changes** wählen, z. B. mit Nachricht `ServeIQ Version 0.2 – Regel- und Speichertests`.
5. **Settings → Pages**: Source `Deploy from a branch`, Branch `main`, Folder `/(root)`.
6. Nach Veröffentlichung Link `https://BENUTZERNAME.github.io/ServeIQ/` öffnen. Bei veralteter Ansicht `Strg+F5` oder Browser-Cache prüfen.

**Wichtig:** `index.html` muss unmittelbar im Stammverzeichnis liegen und darf nicht in einem weiteren Unterordner sein. Nur das ZIP hochzuladen funktioniert nicht.

## Nutzung und Speicherung
- Die App ist für **6:6-Volleyball** ausgelegt; Spezialregeln für Kids Volley oder 4:4 fehlen.
- Browserdaten werden **lokal auf dem aktuellen Gerät und derselben Website** gespeichert. Keine Datenbank, kein Login, **keine automatische Synchronisation** zwischen Smartphone und Laptop.
- Automatische Speicherung in IndexedDB und als lokale Browser-Notfallsicherung. Dennoch können Private-Mode, voller Speicher, Browserbereinigung, beschädigte Geräte oder abgebrochene Dateien zu Datenverlust führen.
- **Regelmässig unter Einstellungen → Datensicherung erstellen (JSON) herunterladen.** JSON lässt sich über Einstellungen wieder importieren. Vor Import werden bestehende Daten nach Bestätigung ersetzt.
- **Excel-Export im Archiv** ist nur für die statistische Auswertung, nicht zur Wiederherstellung eines Spiels.
- Wenn bisher die GitHub-Version 0.1 verwendet wurde: **vor der Aktualisierung eine JSON-Datensicherung erstellen**. Die Version 0.2 verwendet einen anderen Browser-Speicherbereich; alte Daten erscheinen möglicherweise nicht automatisch. Importiere die Sicherung und prüfe Kader und Spiele.
- Offline-Nutzung: GitHub-Pages-Seite **einmal online öffnen**, bevor die Verbindung wegfällt. Service Worker und Installation als PWA erfordern HTTPS. Die direkt geöffnete HTML-Datei bleibt eine Testmöglichkeit, bietet jedoch keine garantierte Offline-Installation.

## Funktionale Hinweise
- Neues Team speichern → direkt zum Teamkader; Spielerin speichern → im Kader bleiben; Kader speichern → Teams-Startseite.
- Matchkader: zunächst keine Spielerin ausgewählt; erst bei mindestens sechs regulären Spielerinnen zur Aufstellung.
- Satzaufstellungen sind ab Satz 2 wieder leer; Aufstellung per Ziehen oder Antippen.
- Satz 2–4: erster Service und Spielfeldseite wechseln automatisch. Satz 5: neue Auswahl; Seitenwechsel beim ersten achten Punkt.
- Live-Game: Ein Klick auf `Normaler Service` zählt noch keinen Punkt; die anschliessende Auswahl schliesst den Ballwechsel ab.
- `Punkt zurücknehmen` und `Punkt vorwärts` berücksichtigen zugehörige Statistik, Rotation und Satzgrenzen.
- Libera: nur symbolisch ausgewiesen, keine Wechselerfassung oder Service-Statistik. **Die Einsatzstatistik regulärer Spielerinnen kann bei tatsächlichen Libera-Einsätzen von der realen Feld-Einsatzzeit abweichen.**
- Nur reguläre Spielerwechsel (max. sechs pro Satz und Rückwechselregeln) werden im Live-Game erfasst. Verletzungs-/Ausnahmewechsel und Sanktionen sind nicht vollständig abgebildet.

Die Version ist eine **funktionsfähige Testversion**, keine Garantie für absolute Fehlerfreiheit. Weitere technische Prüfschritte stehen in `TESTPROTOKOLL.md`.
