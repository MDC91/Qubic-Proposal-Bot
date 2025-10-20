<div align="center">

# 🤖 Qubic Proposal Bot
  
### **Automatische Proposal-Zusammenfassungen für die Qubic-Community in 13 Sprachen**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
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

| Sprache | Code |
|---------|------|
| Deutsch | `de` |
| Englisch | `en` |
| Französisch | `fr` |
| Spanisch | `es` |
| Italienisch | `it` |
| Portugiesisch | `pt` |
| Russisch | `ru` |
| Japanisch | `ja` |
| Chinesisch | `zh` |
| Koreanisch | `ko` |
| Arabisch | `ar` |
| Türkisch | `tr` |
| Vietnamesisch | `vi` |

## 🎯 Funktionen im Detail

### 🤖 Automatische Proposal-Erkennung
- **15-Minuten-Intervall** - Regelmäßige Überprüfung auf neue Proposals
- **Epochen-basierte Verarbeitung** - Separate Zustandsverwaltung pro Epoche
- **Duplikatserkennung** - Verhindert mehrfache Benachrichtigungen

### 🧠 Intelligente KI-Zusammenfassungen
- **Kontextbewusste Zusammenfassung** - Extrahiert Kernpunkte jedes Proposals
- **Sprachspezifische Formatierung** - Angepasst an kulturelle Nuancen
- **Cache-Mechanismus** - Vermeidet doppelte AI-Aufrufe für dieselben Proposals

### 🔄 Robuste State-Verwaltung
- **Per-Server/Per-Chat State** - Jede Community wird durch ihren eigenen Status verwaltet
- **GitHub-Persistenz** - Zustände bleiben über Neustarts hinweg erhalten
- **Automatische Bereinigung** - Entfernt veraltete Epochen-Daten

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

| **Befehl** | **Beschreibung** | **Parameter** |
|------------|------------------|---------------|
| ❔ `/help`   | Hilfe anzeigen | Ausführliche Hilfe und Anleitung |
| ⚙️ `/setup` | Richtet den Bot für Ihren Server ein | • `channel`: Der Kanal für Proposal-Zusammenfassungen<br>• `language`: Sprache für die Zusammenfassungen |
| ℹ️ `/info`  | Zeigt detaillierte Informationen über den Bot-Status | • Konfigurierter Kanal und Sprache<br>• Aktuelle Epoche<br>• Anzahl aktiver Proposals<br>• DeepSeek API Status<br>• Bot Uptime<br>• Check-Interval |



## 📱 Telegram Verwendung

### Bot zu Ihrer Gruppe hinzufügen
1. **Gruppe verwalten** 
2. **Mitglieder hinzufügen**
3. **Bot suchen:** `@QubicTranslationBot`
4. **Zur Gruppe hinzufügen** als Administrator
5. **Setup durchführen** im gewünschten Chat mit `/setup`

> [!IMPORTANT]
> Der `/setup` Befehl <ins>**muss**</ins> in dem Chat genutzt werden in dem auch die Zusammenfassungen gepostet werden sollen.

### Telegram Befehle

| **Befehl** | **Beschreibung** | **Parameter** |
|------------|------------------|---------------|
| ❔ `/start` oder `/help` | Hilfe anzeigen | Ausführliche Hilfe und Anleitung |
| ⚙️ `/setup` | Öffnet ein Inline Keyboard zur Sprachauswahl | • Inline Keyboard mit Sprachoptionen<br>• Gewünschte Sprache auswählen |
| ℹ️ `/info`  | Zeigt detaillierte Informationen über den Bot-Status | • Konfigurierter Chat und Sprache<br>• Aktuelle Epoche<br>• Anzahl aktiver Proposals<br>• DeepSeek API Status<br>• Bot Uptime<br>• Check-Interval |




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

**Q: Der Bot antwortet nicht auf Befehle - was tun?**  
A: Stellen Sie sicher, dass der Bot die notwendigen Berechtigungen hat und versuchen Sie den Befehl erneut.

**Q: Wie werden Voting-Ergebnisse angekündigt?**  
A: Jeden Mittwoch um 12:15 UTC werden die Ergebnisse der vorherigen Epoche automatisch gepostet.

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

**🌍 Ein Projekt für die Qubic-Community**  
*Proposals für alle zugänglich machen, in jeder Sprache*

</div>
