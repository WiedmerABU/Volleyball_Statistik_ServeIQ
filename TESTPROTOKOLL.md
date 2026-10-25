# ServeIQ 0.2 – Qualitätssicherung

## Bereits automatisiert geprüft (simulierter Chromium-Browser)
- Team mit Saison und Kader anlegen, Speicherbestätigung, Rückkehr zu Teams
- Doppelte Trikotnummer im Teamkader abweisen
- Team und Spielerinnen nach simuliertem Neuladen wieder verfügbar
- Spieldaten speichern → Matchkader → Startaufstellung → Match speichern
- Spielentwurf speichern, wieder öffnen und fortsetzen
- Interlaken links **und** rechts, Punktebuttons und Counter-Seitenzuordnung
- Ass, normaler Service, Servicefehler, Side-out und Rotation
- `Punkt zurücknehmen` und `Punkt vorwärts`, einschliesslich Statistik, Wechsel und Aufschlagfolge
- Wechsel und regelkonformer Rückwechsel, unveränderter Spielstand
- Statistiken und beide dynamischen Diagramme, Schliessen → Teams
- Kein Javascript-Laufzeitfehler in den geprüften Bedienpfaden

## Noch auf echtem Gerät und nach GitHub-Deployment testen
- Speicherung und erneutes Öffnen auf **deinem** Smartphone und Laptop
- Unterbrechung der Internetverbindung und Offline-Aufruf nach erster Online-Nutzung
- Touch-Drag-and-drop bei Satz 2–5 und unterschiedliche Bildschirmgrössen
- Ein vollständiges Spiel mit fünf Sätzen, Seitenwechsel bei acht Punkten
- Erzeugte Excel-Datei in Microsoft Excel öffnen
- JSON-Datensicherung exportieren, nach Probe-Import identische Daten prüfen
- Browser-Neustart, längere Partie, schneller Klickrhythmus, möglicher voller Gerätespeicher

## Bekannte fachliche Einschränkungen
- Keine Liberawechsel-Erfassung; daher keine exakten Einsatzzeiten für Libera und ihre Ersatzspielerinnen.
- Kein spezieller 4:4-/Kids-Volley-Modus.
- Ausnahmen wie Verletzungswechsel und Strafpunkte separat prüfen; die Regeloberfläche unterstützt regulären 6:6-Spielbetrieb.
- Ohne Cloud-Datenbank bleiben Spielstände pro Gerät/Browser getrennt.
