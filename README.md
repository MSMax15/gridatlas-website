# GridAtlas Website – Growth Ready

Öffentliche Marketing-, Selbstcheck- und Pilot-Website für **https://gridatlas.de**.


## Update v2 – Accessibility und Pilotklarheit

- kleine Akzenttexte besitzen jetzt ausreichend WCAG-AA-Kontrast
- Heading-Struktur der Startseite wurde korrigiert
- Tastaturfokus ist deutlicher sichtbar
- Pilotbewerbung und tatsächlicher Testzugang sind klar getrennt
- Product-Core-Aussagen wurden gegen Mission 013 und Wissensbasis v5.2 geprüft

Das Update benötigt keine neue DNS-, Pages- oder Formspree-Konfiguration. Bestehende Dateien können direkt überschrieben werden.

## Sofort veröffentlichen

1. Inhalt dieses Ordners in die Root-Ebene des öffentlichen Repositorys `MSMax15/gridatlas-website` hochladen.
2. GitHub: `Settings → Pages → Deploy from a branch → main → /(root)`.
3. Custom Domain: `gridatlas.de`; danach `Enforce HTTPS` aktivieren.
4. Prüfen, dass `CNAME` nur `gridatlas.de` enthält.

Bei jedem Commit auf `main` aktualisiert GitHub Pages die Seite automatisch. Es ist kein GitHub-Actions-Workflow und keine Build-Abhängigkeit notwendig.

## Formspree

Der aktuell verbundene Endpoint steht in `assets/js/config.js`:

```js
formEndpoint: "https://formspree.io/f/xlgqnnel"
```

Der Endpoint ist kein geheimer API-Schlüssel. Trotzdem müssen Formspree-Konto, Empfängeradresse, Spamfilter und Benachrichtigungen geschützt werden.

Formtypen:
- `self_check` – Nutzer sendet den erzeugten Prozessbericht
- `pilot_application` – Pilotbewerbung

## Suchmaschinen – Null-Euro-Start

### Google Search Console
1. Domain-Property `gridatlas.de` anlegen.
2. Per DNS-TXT verifizieren.
3. `https://gridatlas.de/sitemap.xml` einreichen.
4. Startseite, Check, Checkliste und Produktseite über URL-Prüfung anfordern.

### Bing Webmaster Tools
1. Domain hinzufügen oder aus Search Console importieren.
2. Sitemap einreichen.
3. Die wichtigsten URLs manuell einreichen.
4. Site Scan ausführen.

Indexierung braucht Zeit und ist nicht garantiert. Der kostenlose Selbstcheck und die Fachseiten sorgen für klare Suchintention und interne Verlinkung.

## Sicherheit

- Nur statisches HTML/CSS/JavaScript.
- Keine Datenbank, keine Dokumentenuploads, keine Zugangsdaten.
- Keine externen Schriften oder Analyse-Skripte.
- CSP als Meta-Policy, HTTPS-only URLs, strikte Referrer-Policy.
- Keine Speicherung der Selbstcheck-Antworten in Local Storage.
- DOM-Ausgabe ausschließlich über `textContent`.
- Begrenzte Feldlängen und Honeypot.
- `security.txt` vorhanden.

**Wichtige technische Grenze:** GitHub Pages erlaubt keine frei konfigurierbaren HTTP-Sicherheitsheader pro Repository. Für die spätere Produkt-App mit Logins und Kundendokumenten ist GitHub Pages deshalb ungeeignet. Diese Website ist sicherheitsbewusst für Marketing und Lead-Erfassung, aber keine „unknackbare Steel Wall“.

Empfohlen im GitHub-Konto:
- Zwei-Faktor-Authentifizierung
- Domain verifizieren
- Branch Protection für `main`
- Secret Scanning aktivieren
- nur notwendige Collaborators
- Enforce HTTPS

## Dateien lokal testen

```bash
python -m http.server 8000
```

Dann `http://localhost:8000` öffnen.

## Vor Veröffentlichung prüfen

- Formspree-Test mit eigener E-Mail
- Datenschutz und Impressum fachlich prüfen
- GitHub-Domainverifizierung behalten
- HTTPS aktiv
- mobile Darstellung testen
- keine Testdaten oder internen Dateien im Repository
