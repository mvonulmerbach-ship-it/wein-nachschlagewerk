# Wein – Nachschlagewerk

Nachschlagewerk zum Wein: Grundlagen, Verkostung, Rebsorten und Regionen in kurzen, verlinkten Artikeln.

**Live:** https://mvonulmerbach-ship-it.github.io/wein-nachschlagewerk/

## Inhalt

29 Artikel in diesen Bereichen: 🍇 Grundlagen · 👅 Verkostung & Aromen (mit Aromarad) · 🍷 Rebsorten · 🌍 Regionen · ✨ Besondere Weine · 🌡️ Servieren & Genießen · 📚 Service.

## Funktionen

- Menü ☰ mit allen Bereichen (am Desktop als Seitenleiste), Logo führt zur Startseite.
- Jeder Artikel hat eine eigene Adresse (z. B. `#aromarad`), Querverweise im Text springen direkt zum Artikel.
- **Suche** über Titel und Text; Treffer im Titel stehen zuerst (exakt, dann Anfang, dann irgendwo im Titel, dann nur im Text).
- Hell/Dunkel oben rechts: ◐ System (Standard) · ☀️ Hell · 🌙 Dunkel. Die Wahl gilt für alle fünf Nachschlagewerke (`localStorage`, Schlüssel `nsw_theme`).
- Die Lern-App [Vino – Wein lernen](https://mvonulmerbach-ship-it.github.io/wein-lern-app/) bettet das Nachschlagewerk ein und gibt dabei `?theme=dark|light` mit; dieser Parameter hat Vorrang.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | die ganze App (HTML, CSS, JavaScript und alle Artikel) |
| `aromarad.html` | Aromarad, Kopie aus dem Repo `aroma-rad` – dort ändern, dann kopieren |
| `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `icon-maskable.png` | Installation als App |
| `sw.js` | Service Worker für den Offline-Betrieb |

## Auf dem Handy installieren

Seite in Chrome öffnen → Menü ⋮ → „Zum Startbildschirm hinzufügen“ (Safari: Teilen → „Zum Home-Bildschirm“).

## Offline

Nach dem ersten Öffnen läuft das Nachschlagewerk ohne Netz (Service Worker, network first mit Cache als Rückfall).
