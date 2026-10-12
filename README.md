# Empfehlungsbund – Codex-Marketplace

Plugins von [pludoni](https://www.pludoni.de) für [OpenAI Codex](https://developers.openai.com/codex).

| Plugin | Für | Server |
|---|---|---|
| `empfehlungsbund-arbeitgeber` | Partnerfirmen und Kunden des Empfehlungsbunds | `https://login.empfehlungsbund.de/mcp` |

## Empfehlungsbund für Arbeitgeber

Verbindet Codex per OAuth mit dem eigenen Firmen-Account unter [login.empfehlungsbund.de](https://login.empfehlungsbund.de):
Firmenprofil, Ansprechpartner, Standorte und Stellen pflegen, Stellenentwürfe anlegen, Klick- und Bewerbungsstatistiken
sowie Meldungen abrufen. Neue Stellen entstehen als unsichtbarer Entwurf; Bewerberdaten sind über die Schnittstelle
nicht zugänglich.

Voraussetzung: Der KI-Agenten-Zugang ist für die Firma freigeschaltet. Anleitung und bestehende Verbindungen im Login
unter **Account → KI-Agenten**.

### Installation

```bash
codex plugin marketplace add pludoni/codex-marketplace
codex plugin add empfehlungsbund-arbeitgeber@empfehlungsbund
```

Bei der Installation öffnet Codex die Anmeldung bei login.empfehlungsbund.de. Dort bestätigen, ob der Agent nur lesen
oder auch schreiben darf. Eine Verbindung gilt 30 Tage und lässt sich jederzeit im Login trennen.

Ohne Plugin geht es auch direkt als MCP-Server:

```bash
codex mcp add empfehlungsbund-arbeitgeber --url https://login.empfehlungsbund.de/mcp
```

## Kontakt

pludoni GmbH · info@pludoni.de · [Datenschutz](https://www.empfehlungsbund.de/datenschutz) · [AGB](https://www.empfehlungsbund.de/agb)
