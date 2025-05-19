# 🩺 CareSyncServer

Ein TCP-basierter Kommunikations- und Verwaltungsserver für medizinische Einrichtungen.  
Dieses CLI-Tool dient als zentrale Instanz für Nachrichtenübermittlung und Patientendatenverwaltung.

---

## 📦 Projektüberblick

- **Sprache:** C++
- **Build-System:** CMake
- **Datenbank:** SQLite
- **Kommunikation:** TCP-Sockets
- **Anwendung:** CLI-Server zur Verwaltung von Patientendaten und Echtzeit-Kommunikation mit GUI-Clients

---

## 📁 Projektstruktur

```
CareSyncServer/
├── main.cpp                   # Einstiegspunkt
├── include/
│   ├── Server.hpp             # TCP-Server
│   ├── ClientHandler.hpp      # Verarbeitung einzelner Clients
│   ├── DatabaseManager.hpp    # SQLite-Handling
│   └── Utils.hpp              # Hilfsfunktionen
├── src/
│   ├── Server.cpp
│   ├── ClientHandler.cpp
│   ├── DatabaseManager.cpp
│   └── Utils.cpp
├── data/
│   └── patients.db            # Lokale SQLite-Datenbank
└── logs/
    └── server.log             # Server-Logs
```

---

## ⚙️ Setup & Build

### Voraussetzungen
- C++17 oder neuer
- [CMake](https://cmake.org/) 3.10+
- SQLite3 (wird automatisch über das Projekt eingebunden oder Systemabhängig installiert)

### Kompilierung
```bash
git clone https://github.com/dein-username/CareSyncServer.git
cd CareSyncServer
mkdir build && cd build
cmake ..
make
```

---

## 🚀 Starten des Servers

```bash
./CareSyncServer
```

Standardmäßig öffnet der Server Port `54000` und lauscht auf eingehende Verbindungen.

---

## 🧪 Funktionen

✅ Verwaltung von Patientendaten (CRUD)  
✅ Mehrere gleichzeitig verbundene Clients (multithreaded)  
✅ Kommunikation über TCP (Textbasiertes Protokoll)  
✅ Speicherung in SQLite-Datenbank  
✅ Erweiterbar für Authentifizierung und Verschlüsselung

---

## 🧱 Erweiterungsmöglichkeiten

- Authentifizierung pro Client
- Nachrichten-Queue mit Zeitstempeln
- Verschlüsselung (TLS)
- REST-Schnittstelle zur externen Kommunikation

---

## 🤝 Lizenz

MIT – frei nutzbar für Studien-, Lehr- oder Praxiszwecke.

---

## 📬 Kontakt

Projekt von Maxim Skalenko  
