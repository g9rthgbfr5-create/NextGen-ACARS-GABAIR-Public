# NextGen-ACARS-GABAIR-Public

ACARS-Anwendung für die Virtual Airline **GAB AIR**. Verbindet Microsoft Flight Simulator (MSFS 2020/2024) und X-Plane 12 über SimConnect mit dem VA-Backend (phpVMS-kompatibel) und bietet Live-Telemetrie, automatisches PIREP-Filing, Wetter, Karten und Post-Flight-Analyse.

## Features

- **SimConnect-Integration:** Live-Telemetrie (Position, Fuel, Gear, Flaps, G-Force, Landing Rate) direkt aus MSFS/X-Plane
- **Automatisches PIREP-Filing:** Start, Live-Events, Position-Reports und Abschluss werden automatisch an das VA-Backend gesendet
- **Offline-Queue:** Bei Verbindungsabbruch werden Events lokal zwischengespeichert und automatisch synchronisiert
- **Live-Map:** React-Leaflet-Karte mit Flugroute, Wetter-Overlay (RainViewer), VATSIM/IVAO-ATC und Traffic
- **Wetter:** METAR/TAF-Abruf (VATSIM + SimBrief-Fallback) für Departure, Arrival und Alternate
- **SimBrief-Integration:** OFP-Anzeige, Routen-Import, Wetter- und Alternate-Übernahme
- **Navigraph-Charts:** Eingebettetes Panel für Charts
- **Post-Flight-Analyse:** Landing Rate, G-Force, TDZ (Touchdown Zone), TCH (Threshold Crossing Height), Centerline-Deviation
- **Unstable-Approach-Warnung:** Warnung bei unstabilem Anflug direkt im Simulator via SimConnect_Text
- **MobiFlight WASM Bridge:** FSLabs A321 LVar-Support (Flap Surface, Flap Lever) für MSFS2024
- **Auto-Update:** SHA-256-verifizierter Update-Check (via GitHub Releases)
- **Deep-Link-Import:** 1-Klick-Konfiguration von der VA-Website (`nextgen-acars://import-config`)
- **Streamer-Modus:** Versteckt sensible Daten für Stream-Overlays
- **Mehrsprachig:** Deutsch und Englisch

## Lizenz

Dieses Projekt steht unter der **MIT Lizenz**. Siehe die `LICENSE` Datei für Details.
