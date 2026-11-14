# GAB-AIR ACARS

Tauri 2
React 19
TypeScript
Rust
Platform
License: MIT

Moderne, hochpräzise ACARS-Anwendung für die Virtual Airline GAB AIR. Verbindet Microsoft Flight Simulator (MSFS 2020 / MSFS 2024) via SimConnect sowie X-Plane 11/12 via UDP-Telemetrie mit dem VA-Backend (phpVMS-kompatibel). Bietet Live-Telemetrie, vollautomatisches PIREP-Filing, Wetter-Overlays, interaktive Karten und lückenlose Post-Flight-Analyse als native Desktop-Applikation für Windows und Linux.

Highlights & Features
🚀 Flugverfolgung & Telemetrie
Cross-Platform: Native Binärdateien für Windows (.exe) und Linux (.AppImage, .deb, .rpm mit voller Wayland- und Mesa-Unterstützung).
Dual-Simulator-Support:
MSFS 2020/2024: Direkte, performante SimConnect-Integration mit entlastetem 5-Hz-UI-Rendering und voller nativer Physik-Abtastrate.
X-Plane 11/12: Robuste UDP-Telemetrie mit frei konfigurierbarem Port (Standard: 52001).
X-Plane 1-Klick Bridge-Installer: Das integrierte XPPython3-Skript (PI_ezva_acars.py) kann direkt aus den Einstellungen installiert und auf Versionsaktualisierungen geprüft werden.
MobiFlight WASM Bridge: LVar-Support für komplexe Addon-Flugzeuge im MSFS (z. B. FSLabs A321 Flap Surface / Lever) mit automatischem Retry-Cooldown.
Cockpit-Avionics-HUD: Permanente digitale Zulu-Uhr (UTC), zweizeilige Cockpit-Statusleiste (avionics-status-bar) mit Flugstatus-HUD (ALT · DTG · ETA / RTE), Live-Flugphase und Piloten-Karrierestatistik.
Neon-Cyan Rundinstrumente: Dynamische Cockpit-Instrumente für Höhe (ALTITUDE), Fluggeschwindigkeit über Grund (GROUND SPD) und Vertikalgeschwindigkeit (V/S).
Pushback Auto-Start: Erkennt das Lösen der Parkbremse und Rollbeginn am Gate automatisch, warnt mit Zweiton-Cockpit-Gong, Sprachansage und In-Sim-Banner und startet das Flug-Tracking nach einem abbrechbaren 10-Sekunden-Countdown.
🌐 Wetter, Karten & Flugplanung
Interaktive Live-Map: Hardware-beschleunigte React-Leaflet-Karte mit Esri-Canvas-Basemaps (Dark/Light Gray), geflogener Route, VATSIM/IVAO-Traffic und Online-ATC-Sektoren.
Wetter-Overlays: Live-Niederschlagsradar (RainViewer) und optionale OpenWeatherMap-Ebenen (Niederschlag, Wind, Bewölkung, Temperatur).
METAR & D-ATIS: Automatische Wetter-Aktualisierung (periodisch sowie beim Sinkflug/Anflug) mit strukturierter Windrose, Wetter-Pills (QNH, WIND, VIS, VFR) und Digital-ATIS-Abruf für VATSIM/IVAO.
SimBrief & Navigraph: Vollständiges Operational Flight Plan (OFP)-Panel mit Routen-Import sowie integrierter Navigraph-Charts-Viewer.
Flightplan Prefile: 1-Klick-Prefile für VATSIM (my.vatsim.net) und IVAO (fpl.ivao.aero) mit vorausgefüllter Route, Callsign, Altitude und Remarks.
🎯 Anflug-Stabilität & Landeanalyse
Stabilized Approach Monitor: Präzise Überwachung der Stabilisierungskriterien ab 1.000 ft über Platzhöhe auf Basis einer integrierten globalen Offline-Flughafendatenbank (60.000+ Airports – verlässlich auch bei spontanen Ausweichlandungen/Diversions).
In-Game Approach Overlay: Separates, transparentes Always-on-Top-Fenster (unter Linux als integriertes In-App-Overlay) für Live-Anzeige von STABLE / UNSTABLE APPROACH inkl. akustischen Sprach-Callouts.
Pistenrelative Landerate: Berechnung der Touchdown-Sinkrate relativ zur realen Neigung der Pistenoberfläche (inkl. Displaced-Threshold-Berechnung und Drift-Projektion).
Erweiterte Landeparameter: Exakte Ermittlung von Touchdown Zone (TDZ in Metern), Threshold Crossing Height (TCH in Fuß), Centerline Deviation (CLD in Metern) und Bounce-Erkennung.
Detaillierter Incident-Report: Protokollierung von Überschreitungen (Overspeed, Taxi-Speed, Flaps/Gear-Limits, G-Force, Cabin Altitude, Unstable Approach) mit Strafpunkt-Bewertung.
Aircraft-Limit-Profile: Maßgeschneiderte Limit-Profile für alle Airbus-Modelle (A220 bis A380) mit 
𝑉
FE
V
FE
	​

-Klappenlogik, Entprellung und Windböen-Toleranzpuffern.
🛡️ Sicherheit, Datenintegrität & Automation
Offline-Queueing & Recovery: Vollständige Zwischenspeicherung von Flug-Events und Trajektorien (FIFO-Queue) bei Verbindungsabbrüchen mit automatischem Nachsenden bei Wiederherstellung. Wiederaufnahme nach Simulator-Crashes ohne Datenverlust.
Treibstoff-Plausibilitätsprüfung: Sicherheitswarnung vor Abflug bei drastischer Abweichung (> 40 %) zwischen real getanktem Treibstoff und SimBrief-Blockfuel.
Simulator Auto-Start & Auto-Close: Automatischer Start der App mit MSFS/X-Plane sowie konfigurierbares automatisches Beenden beim Schließen des Simulators (geschützt während aktiver Flüge).
Release-Kanäle & Auto-Update: Integrierter, SHA-256-verifizierter Auto-Updater mit Wahlmöglichkeit zwischen dem Stable- und Beta-Kanal im Einstellungsmenü, 24h-Pause-Option und Update-Modal samt Release Notes.
1-Klick VA-Import: Nahtlose Übernahme der API-Konfiguration via Deep-Link (nextgen-acars://import-config).
Moderne Einstellungs-UX: Strukturierte Tabs (Simulator Setup, Integrationen & API, Darstellung & App, Updates), Passwort-Auge für API-Keys, Sofort-Verbindungstest und animierte Speicherbestätigung.
Zweisprachig & Streamer-Safe: Vollständige DE/EN-Lokalisierung mit Inline-SVG-Umschalter sowie Streamer-Modus zum Ausblenden privater Zugangsdaten.
Tech-Stack
Komponente	Technologie
Desktop Shell	Tauri 2
 (Sicherheits-Sandboxing, CSP, Rust-IPC)
Frontend Framework	React 19
 & Vite

Programmiersprachen	TypeScript
 (Strict Mode) & Rust

Karten & Geo	Leaflet
 & React-Leaflet
 (Esri Canvas, RainViewer)
Simulator-Anbindung	Microsoft SimConnect SDK, Custom UDP Socket Listener, MobiFlight WASM Bridge
Testing & QA	Vitest
 (Frontend & Utilities), cargo test (Rust Backend), TypeScript tsc --noEmit
Voraussetzungen
Für Anwender
Betriebssystem:
Windows: Windows 10 oder Windows 11 (64-Bit)
Linux: Moderne Distributionen (Ubuntu 22.04+, Fedora 39+, Arch, etc.) mit WebKitGTK 4.1
Simulator:
Microsoft Flight Simulator 2020 oder 2024
X-Plane 11 oder X-Plane 12 (mit installiertem XPPython3)
Für Entwickler
Node.js
 (v20+ LTS empfohlen) & npm
Rust
 (stable toolchain)
Windows Build-Tools: Visual Studio 2022 C++ Workload & LLVM
 (C:\Program Files\LLVM\bin für simconnect Bindgen)
Linux Build-Tools: build-essential, libwebkit2gtk-4.1-dev, libayatana-appindicator3-dev, librsvg2-dev
Entwicklung & Build
Development-Server starten
powershell
# Windows (initialisiert Visual Studio C++ Environment und LLVM automatisch)
.\run-dev.bat
# Oder manuell über npm:
npm install
npm run tauri dev
Tests ausführen & Code-Qualität prüfen

Vor jedem Commit oder Release sollte die Test-Suite durchlaufen werden:

bash
npm test              # Frontend-Tests (Vitest)
npm run test:rust     # Rust Backend-Tests (cargo test)
npm run test:all      # Führt alle Tests aus
npx tsc --noEmit      # Strikter TypeScript Type-Check
Produktions-Builds erstellen
powershell
# Lokaler Entwickler-Build mit vorgeschaltetem Test-Gate
.\build.bat
# Vollständiger Release-Build (erzeugt Installer, SHA-256 Hashes und Update-Metadaten)
.\build_release.bat
Projektstruktur
├── src/                        # React Frontend (React 19, TypeScript)
│   ├── assets/                 # SVGs, Icons, Audiosignale (Gongs, Callouts)
│   ├── components/             # Modulare UI-Komponenten (Header, Sidebar, Map, Modals, Widgets)
│   ├── data/                   # Statische Datenbanken (Flughäfen, Runways, Aircraft-Profile)
│   ├── hooks/                  # Wiederverwendbare React-Hooks (Telemetrie, Timers, Hotkeys)
│   ├── i18n/                   # Lokalisierung (DE/EN Übersetzungstabellen)
│   ├── pages/                  # Hauptansichten & Dashboard-Panels
│   ├── services/               # API-Services (phpVMS, Logbuch, SimBrief, Updater)
│   ├── types/                  # Strikte TypeScript-Typdefinitionen & DTOs
│   ├── utils/                  # Reine Hilfsfunktionen & mathematische Modelle (inkl. Unit-Tests)
│   └── App.tsx                 # Zentrale Orchestrierungskomponente
├── src-tauri/                  # Rust Backend (Tauri 2)
│   ├── src/
│   │   ├── api.rs              # Sichere HTTP-Kommunikation mit Backend & Logbuch
│   │   ├── config.rs           # OS-spezifische Konfiguration und Keyring-Speicher
│   │   ├── lib.rs              # Tauri Commands, Auto-Updater & SimConnect-Listener
│   │   ├── logger.rs           # File-Logger (`acars.log`)
│   │   ├── main.rs             # Einstiegspunkt Desktop-Runtime
│   │   └── mobiflight.rs       # MobiFlight WASM Bridge (LVar-Integration)
│   ├── capabilities/           # Tauri 2 Sicherheits- und Rechte-Deklarationen
│   └── tauri.conf.json         # Tauri-Konfiguration (Fenster, Bundles, CSP)
├── docs/                       # Entwickler-Dokumentation, Roadmap und UI-Konzepte
├── build.bat                   # Build-Pipeline mit automatischem Test-Gate
├── build_release.bat           # Release-Pipeline mit Signierung & Hash-Generierung
├── CHANGELOG.md                # Detaillierte Versionshistorie
└── AGENTS.md                   # Richtlinien für AI- und Entwickler-Agenten
Roadmap & Weiterentwicklung

Die zukünftige Planung, Meilensteine (z. B. v1.2.0 Refactoring, Discord Rich Presence, v1.6.0 Live-Map Redesign) und Entwürfe sind dokumentiert in:

docs/ROADMAP.md – Gesamt-Roadmap und Backlog
REFACTORING_PLAN_1.2.0.md – Architekturplan für v1.2.x
Lizenz

Dieses Projekt steht unter der MIT-Lizenz. Einzelheiten entnehmen Sie bitte der Datei LICENSE.
