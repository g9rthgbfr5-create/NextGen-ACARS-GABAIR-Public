# GAB-AIR ACARS

ACARS-Anwendung für die Virtual Airline **GAB AIR**. Verbindet Microsoft Flight Simulator (MSFS 2020/2024) via SimConnect sowie X-Plane 11/12 via UDP-Telemetrie mit dem VA-Backend und bietet Live-Telemetrie, automatisches PIREP-Filing, Wetter, Karten und Post-Flight-Analyse als native App für **Windows und Linux**.

## Features

- **Cross-Platform:** Native Anwendungen für Windows (.exe) und Linux (.AppImage, .deb, .rpm).
- **SimConnect & UDP-Integration:** Live-Telemetrie (Position, Fuel, Gear, Flaps, G-Force, Landing Rate) direkt aus MSFS oder X-Plane.
- **Automatisches PIREP-Filing:** Start, Live-Events, Position-Reports und Abschluss werden automatisch an das VA-Backend gesendet.
- **Offline-Queue & Logbuch:** Bei Verbindungsabbruch werden Events lokal zwischengespeichert. Erfolgreiche Flüge werden zudem in einem detaillierten, lokalen Tagebuch (Offline-Logbuch) gesichert.
- **Live-Map:** Interaktive Karte mit Flugroute, Wetter-Overlay (RainViewer), VATSIM/IVAO-ATC und Traffic.
- **Wetter & SimBrief:** METAR/TAF-Abruf für Departure, Arrival und Alternate. Volle SimBrief-Integration (OFP-Anzeige, Routen-Import).
- **Navigraph-Charts:** Eingebettetes Panel für Karten.
- **VATSIM/IVAO Flight Plan Prefile:** Vorausgefüllter Flightplan-Link zu my.vatsim.net bzw. fpl.ivao.aero (Callsign, Route, Aircraft, Cruise-Alt, Speed, Remarks) direkt aus der App heraus.
- **Live D-ATIS:** Digital-ATIS-Abruf für VATSIM und IVAO.
- **Post-Flight-Analyse:** Präzise Auswertung von Flugzeit, Fuel Burn, Landing Rate, G-Force, TDZ (Touchdown Zone in Metern), TCH (Threshold Crossing Height) und Centerline-Deviation. Zusätzlich Efficiency-Rating (Ist-Route vs. SimBrief-Route), Strafpunkte und ein Incident-Report mit allen Vorkommnissen (Overspeed, Taxi-Speed, Flap/Gear-Limits, G-Load, Cabin Altitude, Unstable Approach).
- **Stabilized-Approach & Ausweichlandungen:** Warnung bei unstabilem Anflug. Greift dank einer integrierten Offline-Datenbank (60.000+ Flughäfen) immer auf echte MSL-Elevation zurück, selbst bei spontanen Ausweichlandungen (Diversions).
- **In-Game Approach Overlay:** Separates, transparentes Always-on-Top-Fenster mit Live-Status "STABLE / UNSTABLE APPROACH" inkl. Gründen – ideal für Stream-Overlays. Zusätzlich gibt es echte Audio-Callouts ("Stable"/"Unstable").
- **Addon Support:** LVar-Unterstützung (Flap Surface, Flap Lever) für komplexe Addon-Flieger im MSFS (z.B. FSLabs A321).
- **X-Plane Plugin Installer:** Das benötigte XPPython3-Telemetrie-Skript ist in der App gebündelt und lässt sich mit einem Klick aus den Einstellungen in den Sim installieren. Die App erkennt automatisch, ob die installierte Skript-Version veraltet ist.
- **Konfigurierbarer X-Plane UDP-Port:** Der UDP-Port für die X-Plane-Telemetrie (Standard 52001) ist frei wählbar.
- **Live-Telemetrie-Gauges:** Kreisförmige Anzeigen für die wichtigsten Live-Werte direkt im Dashboard.
- **Free Flight:** Fliegen ohne aktive Bid/PIREP wird unterstützt (inkl. lokalem Logbuch-Eintrag).
- **Safe App Exit:** Bestätigungsdialog beim Schließen der App während eines laufenden Flugs.
- **Simulator Auto-Start:** MSFS und X-Plane 12 können ACARS automatisch starten (FlyWithLua-Autostart).
- **Auto-Update:** Verifizierter Auto-Updater hält die App auf dem neuesten Stand.
- **Deep-Link-Import:** 1-Klick-Konfiguration von der VA-Website (`nextgen-acars://import-config`).
- **Mehrsprachig:** Vollständige DE/EN-Übersetzung für die gesamte App.
- **Streamer-Modus:** Versteckt sensible Daten (API-Key, PIREP-Details) für Stream-Overlays.

## Lizenz

Dieses Projekt steht unter der **MIT Lizenz**. Siehe die `LICENSE` Datei für Details.
