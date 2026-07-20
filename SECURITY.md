# Security Policy

## Scope
Dieses Repository enthält ausschließlich die öffentliche statische Website. Keine Produktdaten, Secrets, Kundendokumente oder Backend-Komponenten gehören hierher.

## Reporting
Meldungen an kontakt@gridatlas.de. Bitte keine sensiblen Daten oder Schadsoftware senden.

## Hardening
- GitHub 2FA und Domain Verification
- Enforce HTTPS
- Branch Protection
- minimale Collaborator-Rechte
- keine Drittanbieter-Skripte
- Content Security Policy im HTML
- Formspree-Honeypot und serverseitige Spamfilter

## Limitation
GitHub Pages unterstützt keine frei konfigurierbaren Response Header. Die spätere Anwendung muss auf einer Plattform mit serverseitigen Sicherheitsheadern, Authentifizierung, Mandantentrennung, Backups und Logging betrieben werden.
