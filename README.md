# GAB-AIR ACARS

[![Download](https://img.shields.io/badge/Download-Latest%20Release-blue.svg?logo=github)](https://github.com/g9rthgbfr5-create/NextGen-ACARS-GABAIR-Public/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux-lightgrey.svg)](https://github.com/g9rthgbfr5-create/NextGen-ACARS-GABAIR-Public/releases)
[![Status](https://img.shields.io/badge/Status-Beta%20%26%20Stable-green.svg)](https://github.com/g9rthgbfr5-create/NextGen-ACARS-GABAIR-Public/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Moderne, hochpräzise ACARS-Anwendung für die Virtual Airline **GAB AIR**. Verbindet Microsoft Flight Simulator (MSFS 2020 / MSFS 2024) sowie X-Plane 11 / 12 mit dem VA-Backend und bietet Live-Telemetrie, automatisches PIREP-Filing, Wetterradar, SimBrief-Integration und detaillierte Lande- und Fluganalysen als native Desktop-App für **Windows und Linux**.

---

## Download & Installation

Die aktuellsten Versionen findest du immer unter **[GitHub Releases](https://github.com/g9rthgbfr5-create/NextGen-ACARS-GABAIR-Public/releases)**.

| Betriebssystem | Paket | Beschreibung |
|---|---|---|
| **Windows** | `.exe` | Windows-Setup (empfohlen für Windows 10/11) |
| **Linux** | `.AppImage` | Portables Paket für alle gängigen Distributionen |
| **Linux (Debian/Ubuntu)** | `.deb` | Natives Installationspaket |
| **Linux (Fedora/RHEL)** | `.rpm` | Natives Installationspaket |

---

## Schnellstart für Piloten

1. **Herunterladen & Starten:** Lade die passende Version für dein Betriebssystem herunter und starte NextGen ACARS.
2. **1-Klick-Konfiguration:** Klicke im Crew-Center auf der GAB AIR Website auf **"ACARS konfigurieren"** – Zugangsdaten und Server-URL werden automatisch übernommen (`nextgen-acars://import-config`). Alternativ kannst du deinen API-Key manuell in den *Einstellungen* eintragen.
3. **Simulator vorbereiten:**
   - **MSFS 2020 / 2024:** Keine Zusatzsoftware erforderlich. Verbindet sich automatisch via SimConnect.
   - **X-Plane 11 / 12:** Benötigt [XPPython3](https://xppython3.readthedocs.io/). Öffne die ACARS-Einstellungen (*Simulator Setup*) und klicke auf **"X-Plane Plugin installieren"**, um die Telemetrie-Bridge automatisch in deinen Simulator einzuspielen.
4. **Flug buchen & loslegen:** Buche einen Flug im Crew-Center, starte ACARS und klicke auf **"Flug starten"**. Bei aktiviertem *Pushback Auto-Start* startet die Aufzeichnung sogar vollautomatisch beim Verlassen des Gates!

---

## Features

- **Dual-Simulator-Support:** Volle Unterstützung für MSFS 2020/2024 und X-Plane 11/12.
- **Pushback Auto-Start:** Erkennt Pushback oder Rollbeginn am Gate automatisch, warnt mit Cockpit-Gong und startet die Aufzeichnung nach einem 10-Sekunden-Countdown.
- **Cockpit-Avionics-HUD:** Permanente Zulu-Uhr (UTC), Cockpit-Statusleiste (Flugphase, Route, ETA) und leuchtende Rundinstrumente (Höhe, Ground Speed, V/S).
- **Interaktive Live-Karte:** Hardwarebeschleunigte Karte mit Live-Flugroute, VATSIM/IVAO-Traffic und Online-ATC-Sektoren.
- **Wetter & SimBrief:** Live-Niederschlagsradar (RainViewer/OpenWeatherMap), automatische METAR- und D-ATIS-Aktualisierungen mit Windrose sowie integrierte SimBrief-OFP- und Navigraph-Panels.
- **Stabilized Approach Monitor:** Überwachung der Anflugstabilität ab 1.000 ft GND auf Basis von über 60.000 weltweiten Flughäfen mit akustischen Ansagen ("Stable"/"Unstable").
- **In-Game Approach Overlay:** Schwebendes, transparentes Overlay (unter Linux nahtloses In-App-Overlay) für den Anflugstatus direkt über dem Simulator.
- **Präzise Landeanalyse:** Pistenrelative Landerate (berücksichtigt Bahnneigung), Touchdown Zone (TDZ in Metern), Centerline-Abweichung (CLD), Threshold Crossing Height (TCH) und Bounces.
- **Offline-Sicherheit & Queue:** Flug-Events und Routenpunkte werden bei Verbindungsverlust zwischengespeichert und automatisch nachgesendet.
- **Auto-Updater mit Kanalwahl:** Wahl zwischen *Stable* (empfohlen) und *Beta* (Vorabversionen) direkt in den App-Einstellungen.

---

## Systemanforderungen

- **Windows:** Windows 10 oder Windows 11 (64-Bit)
- **Linux:** Ubuntu 22.04+, Fedora 39+, Arch Linux oder kompatibel
- **Simulator:** Microsoft Flight Simulator (2020/2024) oder X-Plane 11/12

---

## Support & Feedback

Bei Fragen, Fehlern oder Feedback:
- Erstelle ein [GitHub Issue](https://github.com/g9rthgbfr5-create/NextGen-ACARS-GABAIR-Public/issues)
- Melde dich im **GAB AIR Discord** im ACARS-Support-Kanal.

---

## Lizenz

Dieses Projekt steht unter der **MIT-Lizenz**. Siehe [`LICENSE`](LICENSE) für weitere Informationen.
```
