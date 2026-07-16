# KI-Consulting Website

Statische One-Pager-Website für KI-Consulting und digitale Lösungen (Zielgruppe: kleine und mittlere Unternehmen, Region Limburg-Weilburg und remote).

## Struktur

| Datei | Inhalt |
|-------|--------|
| `index.html` | Startseite (Hero mit animierter Netzgrafik, Leistungen, Praxisbeispiele, Über uns, FAQ, Kontakt) |
| `impressum.html` | Impressum (Platzhalterseite) |
| `datenschutz.html` | Datenschutzerklärung (Platzhalterseite) |

Reines HTML/CSS/JS ohne Build-Schritt und ohne externe Laufzeit-Abhängigkeiten. Lokal einfach `index.html` im Browser öffnen oder statisch hosten.

## Vor dem Livegang ausfüllen

Firmendaten sind bewusst Platzhalter (`[Unternehmensname]`, `[E-Mail-Adresse]`, `[Telefonnummer]`, `[Adresse]`, `[LinkedIn-Profil]`).

Oben im `<script>`-Block von `index.html` gibt es ein `CONFIG`-Objekt:

```js
var CONFIG = {
  companyName: '',
  email:       '',
  phone:       '',
  address:     '',
  linkedin:    ''
};
```

Werte eintragen — die Platzhalter werden dann automatisch überall (inkl. Seitentitel, `mailto:`- und `tel:`-Links) ersetzt. Links mit leeren Feldern werden deaktiviert, damit sie nicht versehentlich als kaputte Kontaktwege veröffentlicht werden.

`impressum.html` und `datenschutz.html` enthalten bewusst keine erfundenen rechtlichen Angaben und werden vor Veröffentlichung juristisch geprüft ergänzt.

GitHub Pages oder ein anderes öffentliches Hosting darf erst aktiviert werden, wenn alle fünf `CONFIG`-Werte sowie Impressum, Datenschutzerklärung und der Abschnitt zu Personen und Qualifikationen vollständig ausgefüllt sind.
