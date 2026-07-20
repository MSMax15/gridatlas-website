# START HIER – bestehende GridAtlas-Website aktualisieren

Du musst das GitHub-Repository **nicht löschen**. Ersetze nur die Dateien durch dieses vollständige Paket.

## Browser-Methode

1. Dieses ZIP entpacken.
2. `https://github.com/MSMax15/gridatlas-website` öffnen.
3. `Add file → Upload files` wählen.
4. Den **gesamten Inhalt** dieses entpackten Ordners hineinziehen.
5. Bei gleichnamigen Dateien bestätigt GitHub die Aktualisierung. Neue Ordner werden ergänzt.
6. Commit-Nachricht verwenden: `Fix accessibility and align pilot messaging`.
7. `Commit changes` auswählen.
8. Unter `Settings → Pages` prüfen, dass weiterhin `main` und `/(root)` aktiv sind.
9. `CNAME` muss exakt `gridatlas.de` enthalten. DNS bei Hostinger nicht verändern.
10. Nach dem Deployment Startseite, Check und Pilotformular im privaten Fenster testen.

## Alte Dateien löschen?

Für dieses Update ist das nicht nötig, weil das Paket dieselbe Struktur verwendet. Nur Dateien löschen, die im neuen Paket bewusst nicht mehr vorhanden sind. Aktuell gibt es keine solche notwendige Löschung.

## Danach prüfen

- `https://gridatlas.de/`
- `https://gridatlas.de/pv-netzanschluss-check/`
- `https://gridatlas.de/pilot/`
- `https://gridatlas.de/sitemap.xml`
- eine Formspree-Testanfrage

**Nie öffentlich hochladen:** Product Core, Wissens-OS, Kundendokumente, `.env`, Zugangsdaten oder n8n-Konfigurationen.
