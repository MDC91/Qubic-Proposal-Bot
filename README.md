# 🤖 Qubic Proposal Bot
## **Automatische Proposal-Zusammenfassungen für die Qubic-Community in 13 Sprachen** 

<div align="center">
  
<img width="250" height="250" alt="icon" src="https://github.com/user-attachments/assets/73fc87fc-0a95-4ae4-bb63-0b45b89d808e" />

</div>

## 📖 Inhaltsverzeichnis

- [🚀 Über das Projekt](#-über-das-projekt)
- [🏗️ Architektur & Technologie](#️-architektur--technologie)
- [📋 Unterstützte Sprachen](#-unterstützte-sprachen)
- [🎯 Funktionen im Detail](#-funktionen-im-detail)
- [💬 Discord Verwendung](#-discord-verwendung)
  - [Bot zu Ihrem Server hinzufügen](#bot-zu-ihrem-server-hinzufügen)
  - [Discord Befehle](#discord-befehle)
- [📱 Telegram Verwendung](#-telegram-verwendung)
  - [Bot zu Ihrer Gruppe hinzufügen](#bot-zu-ihrer-gruppe-hinzufügen)
  - [Telegram Befehle](#telegram-befehle)
- [⚙️ Konfiguration](#️-konfiguration)
- [⚙️ State Management](#️-state-management)
- [❓ Häufig gestellte Fragen (FAQ)](#-häufig-gestellte-fragen-faq)
- [🛠️ Support](#️-support)


## 🚀 Über das Projekt

Der **Qubic Proposal Bot** ist ein speziell für die Qubic-Community entwickelter Bot, der automatisch neue Governance-Proposals erkennt, mittels KI in 13 verschiedenen Sprachen zusammenfasst und in Discord-Servern und Telegram-Gruppen veröffentlicht.

### 🌟 Hauptnutzen

- **🔍 Automatische Erkennung** - Überwacht kontinuierlich neue Qubic-Proposals
- **🌍 Mehrsprachige Zugänglichkeit** - Macht Proposals für nicht-englischsprachige Community-Mitglieder verfügbar
- **🤖 KI-gestützte Zusammenfassungen** - Verwendet DeepSeek AI für präzise, leicht verständliche Zusammenfassungen
- **⏰ Zeitnahe Benachrichtigungen** - Postet neue Proposals innerhalb von 15 Minuten nach Veröffentlichung
- **📊 Voting-Ergebnisse** - Veröffentlicht automatisch Ergebnisse am Ende jeder Epoche

## 🏗️ Architektur & Technologie

Der Bot basiert auf einer robusten Multi-Plattform-Architektur:

### Kernkomponenten

- **Qubic API Integration** - Ruft aktive und abgeschlossene Proposals ab
- **DeepSeek AI** - Erstellt mehrsprachige Zusammenfassungen
- **Discord & Telegram Bridges** - Plattformübergreifende Verteilung
- **GitHub-based Storage** - Persistenter State-Management und Caching
- **Intelligentes Caching** - Vermeidet doppelte API-Aufrufe

## 📋 Unterstützte Sprachen

Der Bot unterstützt derzeit **13 Sprachen**:

| Sprache | Flagge | Code |
|---------|--------|------|
| Deutsch | 🇩🇪 | `de` |
| Englisch | 🇺🇸 | `en` |
| Französisch | 🇫🇷 | `fr` |
| Spanisch | 🇪🇸 | `es` |
| Italienisch | 🇮🇹 | `it` |
| Portugiesisch | 🇵🇹 | `pt` |
| Russisch | 🇷🇺 | `ru` |
| Japanisch | 🇯🇵 | `ja` |
| Chinesisch | 🇨🇳 | `zh` |
| Koreanisch | 🇰🇷 | `ko` |
| Arabisch | 🇦🇪 | `ar` |
| Türkisch | 🇹🇷 | `tr` |
| Vietnamesisch | 🇻🇳 | `vi` |

## 🎯 Funktionen im Detail

### 🤖 Automatische Proposal-Erkennung
- **15-Minuten-Intervall** - Regelmäßige Überprüfung auf neue Proposals
- **Epoch-basierte Verarbeitung** - Separate Zustandsverwaltung pro Epoche
- **Duplikatserkennung** - Verhindert mehrfache Benachrichtigungen

### 🧠 Intelligente KI-Zusammenfassungen
- **Kontextbewusste Zusammenfassung** - Extrahiert Kernpunkte jedes Proposals
- **Sprachspezifische Formatierung** - Angepasst an kulturelle Nuancen
- **Cache-Mechanismus** - Vermeidet doppelte AI-Aufrufe für dieselben Proposals

### 🔄 Robuste State-Verwaltung
- **Per-Server/Per-Chat State** - Jede Community verwaltet ihren eigenen Status
- **GitHub-Persistenz** - Zustände bleiben über Neustarts hinweg erhalten
- **Automatische Bereinigung** - Entfernt veraltete Epoch-Daten

### 🌐 Multi-Plattform Support
- **Nahtlose Discord-Integration** - Slash-Commands und Embed-Nachrichten
- **Telegram-Optimierung** - Inline Keyboards und Markdown-Unterstützung
- **Konsistente Erfahrung** - Gleiche Funktionen auf beiden Plattformen

## 💬 Discord Verwendung

### Bot zu Ihrem Server hinzufügen
1. [**Einladungslink**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot) verwenden
2. **Admin-Berechtigungen** gewähren und den Bot im gewünschten Kanal hinzufügen
3. **Setup durchführen** mit `/setup`

### Discord Befehle

> **⚙️ `/setup` - Bot konfigurieren**  
> **Beschreibung:** Richtet den Bot für Ihren Server ein  
> **Parameter:**
> - `channel`: Der Kanal für Proposal-Zusammenfassungen
> - `language`: Sprache für die Zusammenfassungen

```text
🤖 BEFEHL: /setup - Bot konfigurieren
─────────────────────────────────────
Beschreibung: Richtet den Bot für Ihren Server ein
Parameter:
  • channel:  Der Kanal für Proposal-Zusammenfassungen
  • language: Sprache für die Zusammenfassungen

Beispiel: /setup channel: #proposals language: 🇩🇪 Deutsch
```

| **Befehl** | **Beschreibung** | **Parameter** |
|------------|------------------|---------------|
| ⚙️ `/setup` | Richtet den Bot für Ihren Server ein | • `channel`: Der Kanal für Proposal-Zusammenfassungen<br>• `language`: Sprache für die Zusammenfassungen |
| ℹ️ `/info`  | Zeigt detaillierte Informationen über den Bot-Status | • Konfigurierter Kanal und Sprache
• Aktuelle Epoche
• Anzahl aktiver Proposals
• DeepSeek API Status
• Bot Uptime
• Check-Interval |

**<ins>`/info` - Bot-Status anzeigen</ins>**\
**Beschreibung:** Zeigt detaillierte Informationen über den Bot-Status  


**Ausgabe zeigt:**
- Konfigurierter Kanal und Sprache
- Aktuelle Epoche
- Anzahl aktiver Proposals
- DeepSeek API Status
- Bot Uptime
- Check-Interval

**<ins>`/help` - Hilfe anzeigen</ins>**\
**Beschreibung:** Zeigt ausführliche Hilfe und Anleitung  

#### `/test_check` - Manuelle Proposal-Überprüfung
**Beschreibung:** Löst eine sofortige Proposal-Überprüfung für diesen Server aus 

#### `/test_results` - Manuelle Results-Überprüfung
**Beschreibung:** Löst eine sofortige Results-Überprüfung für die letzte Epoche aus  


## 📱 Telegram Verwendung

### Bot zu Ihrer Gruppe hinzufügen
1. **Bot suchen:** `@QubicTranslationBot`
2. **Zur Gruppe hinzufügen** als Administrator
3. **Setup durchführen** mit `/setup`

### Telegram Befehle

**<ins>`/start` oder `/help` - Hilfe anzeigen</ins>**\
**Beschreibung:** Startet den Bot und zeigt ausführliche Hilfe  

**<ins>`/setup` - Bot konfigurieren</ins>**\
**Beschreibung:** Öffnet ein Inline Keyboard zur Sprachauswahl  
**Prozess:**
1. Befehl `/setup` senden
2. Inline Keyboard mit Sprachoptionen erscheint
3. Gewünschte Sprache auswählen
4. Bot bestätigt die Einrichtung

**<ins>`/info` - Bot-Status anzeigen</ins>**\
**Beschreibung:** Zeigt detaillierte Informationen über den Bot-Status  


**Ausgabe zeigt:**
- Konfigurierter Chat und Sprache
- Aktuelle Epoche
- Anzahl aktiver Proposals
- DeepSeek API Status
- Bot Uptime
- Check-Interval 

#### `/test_check` - Manuelle Proposal-Überprüfung
**Beschreibung:** Startet sofortige Proposal-Überprüfung für diese Gruppe  

#### `/test_results` - Manuelle Results-Überprüfung
**Beschreibung:** Startet sofortige Results-Überprüfung für letzte Epoche 


## ⚙️ Konfiguration

### Server/Kanal Konfiguration

Jeder Server/Telegram-Chat kann unabhängig konfiguriert werden:

**Discord Beispiel-Konfiguration:**
```json
{
  "123456789012345678": {
    "channel_id": "987654321098765432",
    "language": "de"
  }
}
```

## ⚙️ State Management

Der Bot verwaltet für jede Epoche:

- **Verarbeitete Proposals** - Vermeidung von Duplikaten
- **Proposal-Zähler** - Fortlaufende Nummerierung pro Epoche  
- **Sprachspezifische States** - Ermöglicht Sprachwechsel ohne Datenverlust

## ❓ Häufig gestellte Fragen (FAQ)

### 🤔 Allgemeine Fragen

**Q: Welche Sprachen werden unterstützt?**  
A: Derzeit 13 Sprachen: Deutsch, Englisch, Französisch, Spanisch, Italienisch, Portugiesisch, Russisch, Japanisch, Chinesisch, Koreanisch, Arabisch, Türkisch, Vietnamesisch.

**Q: Wie aktuell sind die Proposal-Zusammenfassungen?**  
A: Neue Proposals werden innerhalb von 15 Minuten nach Veröffentlichung erkannt und zusammengefasst.

**Q: Kann ich die Sprache später ändern?**  
A: Ja, einfach erneut `/setup` verwenden. Bereits verarbeitete Proposals werden in der neuen Sprache nachgeliefert.

### 🔧 Technische Fragen

**Q: Warum werden manchmal Proposals doppelt gepostet?**  
A: Dies sollte normalerweise nicht vorkommen. Falls doch, verwenden Sie `/test_check` um den State zu synchronisieren.

**Q: Der Bot antwortet nicht auf Befehle - was tun?**  
A: Stellen Sie sicher, dass der Bot die notwendigen Berechtigungen hat und versuchen Sie den Befehl erneut.

**Q: Wie werden Voting-Ergebnisse angekündigt?**  
A: Jeden Mittwoch um 12:00 UTC werden die Ergebnisse der vorherigen Epoche automatisch gepostet.

### 🌐 Plattform-spezifische Fragen

**Q: Funktionieren alle Befehle auf beiden Plattformen?**  
A: Ja, die Kernfunktionalität ist auf Discord und Telegram identisch.

**Q: Kann ich den Bot sowohl auf Discord als auch Telegram verwenden?**  
A: Ja, Sie können den Bot auf beiden Plattformen parallel verwenden.

**Q: Welche Berechtigungen benötigt der Bot auf Discord?**  
A: Der Bot benötigt Berechtigungen zum Senden von Nachrichten, Embed-Links und Slash-Commands zu verwenden.

## 🛠️ Support

Bei Fragen oder Problemen mit dem Bot wenden Sie sich bitte an:

**📞 Discord/Telegram Kontakt:** MDC

**⚠️ Wichtig:**  
Bitte stellen Sie sicher, dass Sie folgende Informationen bereithalten:
- Server/Chat-ID wo das Problem auftritt
- Genauer Befehl der nicht funktioniert  
- Zeitpunkt des Problems
- Fehlermeldung (falls vorhanden)

---

<div align="center">

**🤝 Ein Projekt für die Qubic-Community**  
*Making proposals accessible to everyone, in every language*

</div>
