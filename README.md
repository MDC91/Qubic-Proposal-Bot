# 🤖 Qubic Proposal Bot

<div align="center">

![Qubic Logo](https://raw.githubusercontent.com/your-username/your-repo/main/assets/logo.png) <!-- Platzhalter für Logo -->

**Automatische Proposal-Zusammenfassungen für die Qubic-Community in 13 Sprachen**

[![Discord](https://img.shields.io/badge/Discord-Join%20Community-7289da?style=for-the-badge&logo=discord)](https://discord.gg/qubic)
[![Telegram](https://img.shields.io/badge/Telegram-Join%20Channel-26A5E4?style=for-the-badge&logo=telegram)](https://t.me/your-channel)

</div>

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

┌─────────────────┐ ┌──────────────────┐ ┌─────────────────┐
│ Qubic API │◄───│ Proposal Bot │───►│ Discord & │
│ proposals.li │ │ (Hauptlogik) │ │ Telegram │
└─────────────────┘ └──────────────────┘ └─────────────────┘
│
▼
┌──────────────────┐
│ DeepSeek AI │
│ (Zusammen- │
│ fassungen) │
└──────────────────┘
│
▼
┌──────────────────┐
│ GitHub Storage │
│ (State & Cache) │
└──────────────────┘
