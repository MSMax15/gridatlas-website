# GridAtlas QR-Code – dauerhaft und unabhängig

## Dauerhafte Zieladresse

Der QR-Code zeigt ausschließlich auf:

```text
https://gridatlas.de/brief/
```

Diese Adresse niemals entfernen oder umbenennen. Der Inhalt der Seite darf jederzeit geändert werden. Solange Domain und Pfad gleich bleiben, funktionieren bereits gedruckte QR-Codes weiter.

## Warum kein externer dynamischer QR-Anbieter nötig ist

Ein statischer QR-Code enthält direkt die eigene GridAtlas-Adresse. Er benötigt kein fremdes Konto, kein Abo und keinen QR-Weiterleitungsdienst. Der wichtigste langfristige Bestandteil ist deshalb nicht ein QR-Anbieter, sondern die eigene Domain `gridatlas.de`.

Auch bei einem späteren Wechsel von GitHub Pages zu Hostinger bleibt der QR-Code gültig, wenn dort weiterhin `/brief/` erreichbar ist.

## GitHub-Upload

Diese Dateien hochladen:

```text
brief/index.html
assets/qr/gridatlas-brief-qr.svg
assets/qr/gridatlas-brief-qr.png
sitemap.xml
```

Danach testen:

```text
https://gridatlas.de/brief/
https://gridatlas.de/assets/qr/gridatlas-brief-qr.svg
```

## Druckempfehlung

- bevorzugt die SVG-Datei verwenden
- QR-Code mindestens 35–40 mm breit drucken
- schwarz auf weiß
- weißen Rand nicht abschneiden
- nicht verzerren
- kein Logo über den QR-Code legen
- zusätzlich `gridatlas.de/brief` lesbar unter den QR-Code schreiben
- Testscan mit mindestens zwei verschiedenen Handys durchführen

## Änderungen in Zukunft

Erlaubt:

- Text, Video, Bilder und Buttons auf `/brief/` ändern
- Website von GitHub zu Hostinger umziehen
- neue Formulare ergänzen

Nicht tun:

- `/brief/` löschen
- die Domain aufgeben
- den QR-Code nachträglich auf eine fremde Kurz-URL umstellen

## Kampagnenmessung

Die Seite verlinkt intern mit `ref=brief`. Dadurch kann der Herkunftswert beim freiwilligen Formularversand an Formspree mitgesendet werden. Für verschiedene Briefvarianten können später zusätzliche Zielpfade wie `/brief-a/` oder Query-Parameter genutzt werden. Der dauerhafte Standardcode sollte aber bei `/brief/` bleiben.
