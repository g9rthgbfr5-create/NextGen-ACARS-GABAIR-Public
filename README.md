# GAB-AIR ACARS

ACARS-Anwendung für die Virtual Airline **GAB AIR**. Verbindet Microsoft Flight Simulator (MSFS 2020/2024) via SimConnect sowie X-Plane 11/12 via UDP-Telemetrie mit dem VA-Backend und bietet Live-Telemetrie, automatisches PIREP-Filing, Wetter, Karten und Post-Flight-Analyse als native App für **Windows und Linux**.

## Features

- **Cross-Platform:** Native Anwendungen für Windows (.exe) und Linux (.AppImage).
- **SimConnect & UDP-Integration:** Live-Telemetrie (Position, Fuel, Gear, Flaps, G-Force, Landing Rate) direkt aus MSFS oder X-Plane.
- **Automatisches PIREP-Filing:** Start, Live-Events, Position-Reports und Abschluss werden automatisch an das VA-Backend gesendet.
- **Offline-Queue & Logbuch:** Bei Verbindungsabbruch werden Events lokal zwischengespeichert. Erfolgreiche Flüge werden zudem in einem detaillierten, lokalen Tagebuch (Offline-Logbuch) gesichert.
- **Live-Map:** Interaktive Karte mit Flugroute, Wetter-Overlay (RainViewer), VATSIM/IVAO-ATC und Traffic.
- **Wetter & SimBrief:** METAR/TAF-Abruf für Departure, Arrival und Alternate. Volle SimBrief-Integration (OFP-Anzeige, Routen-Import).
- **Navigraph-Charts:** Eingebettetes Panel für Karten.
- **Post-Flight-Analyse:** Präzise Auswertung von Landing Rate, G-Force, TDZ (Touchdown Zone in Metern), TCH (Threshold Crossing Height) und Centerline-Deviation.
- **Stabilized-Approach & Ausweichlandungen:** Warnung bei unstabilem Anflug. Greift dank einer integrierten Offline-Datenbank (60.000+ Flughäfen) immer auf echte MSL-Elevation zurück, selbst bei spontanen Ausweichlandungen (Diversions).
- **Addon Support:** LVar-Unterstützung (Flap Surface, Flap Lever) für komplexe Addon-Flieger im MSFS (z.B. FSLabs A321).
- **Auto-Update:** Verifizierter Auto-Updater hält die App auf dem neuesten Stand.
- **Deep-Link-Import:** 1-Klick-Konfiguration von der VA-Website (`nextgen-acars://import-config`).
- **Streamer-Modus:** Versteckt sensible Daten für Stream-Overlays (Mehrsprachig: DE/EN).

## Lizenz

Dieses Projekt steht unter der **MIT Lizenz**. Siehe die `LICENSE` Datei für Details.
