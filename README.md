# Pong Turbo Arcade

Eigenständiger Multiplayer-Prototyp für 1–4 **getrennte Telefone** mit **Klassisch** (zwei Seiten) oder **Arena** (vier Seiten), automatischen Computergegnern und drei Schwierigkeitsstufen.

## Entwicklung

```bash
npm install
npm run server
# zweites Terminal
npm run dev
```

Die Website läuft lokal auf http://localhost:5173 und der autoritative Socket.IO-Server auf Port 3001. Für Handys an anderen Orten beide gemeinsam auf einer öffentlich erreichbaren HTTPS-Domain betreiben. GitHub ist kein Echtzeit-Server.

Der Host erstellt eine Lobby und teilt den angezeigten Code. Andere Spieler treten über ihren eigenen Browser bei. Der Host startet, freie Plätze füllt die KI. Klassisch: 15 Punkte zum Sieg, ab 5 Punkten Rückstand bekommt der benachteiligte Spieler einen grösseren Schläger. Turbo/Fire per Taste. Arcade-Musik wird mit WebAudio erzeugt, Rockriffs begleiten Spezialschläge; Vibration nur bei unterstützten Geräten.

**Status:** Erste Entwicklungsfassung, noch keine produktive Bereitstellung oder geräteübergreifende Integrationstests.
