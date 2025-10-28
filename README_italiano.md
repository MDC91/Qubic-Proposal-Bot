<div align="center">

# 🤖 Qubic Proposal Bot

### **Riepilogo Automatico delle Proposte per la Comunità Qubic in 13 Lingue**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
</div>

## 📖 Indice dei Contenuti

- [🚀 Informazioni sul Progetto](#-informazioni-sul-progetto)
- [🏗️ Architettura & Tecnologia](#️-architettura--tecnologia)
- [📋 Lingue Supportate](#-lingue-supportate)
- [🎯 Funzionalità in Dettaglio](#-funzionalità-in-dettaglio)
- [💬 Utilizzo Discord](#-utilizzo-discord)
  - [Aggiungere il Bot al Tuo Server](#aggiungere-il-bot-al-tuo-server)
  - [Comandi Discord](#comandi-discord)
- [📱 Utilizzo Telegram](#-utilizzo-telegram)
  - [Aggiungere il Bot al Tuo Gruppo](#aggiungere-il-bot-al-tuo-gruppo)
  - [Comandi Telegram](#comandi-telegram)
- [⚙️ Gestione dello Stato](#️-gestione-dello-stato)
- [❓ Domande Frequenti (FAQ)](#-domande-frequenti-faq)
- [🛠️ Supporto](#️-supporto)

## 🚀 Informazioni sul Progetto

Il **Bot Proposte Qubic** è un bot sviluppato specificamente per la comunità Qubic che rileva automaticamente le nuove proposte di governance, le riassume utilizzando l'IA in 13 lingue diverse e le pubblica su server Discord e gruppi Telegram.

### 🌟 Vantaggi Principali

- **🔍 Rilevamento Automatico** - Monitora continuamente le nuove proposte Qubic
- **🌍 Accessibilità Multilingue** - Rende le proposte accessibili ai membri della comunità non anglofoni
- **🤖 Riassunti con IA** - Utilizza DeepSeek AI per riassunti precisi e facili da comprendere
- **⏰ Notifiche Tempestive** - Pubblica nuove proposte entro 15 minuti dalla pubblicazione
- **📊 Risultati delle Votazioni** - Pubblica automaticamente i risultati alla fine di ogni epoca

## 🏗️ Architettura & Tecnologia

Il bot si basa su un'architettura multi-piattaforma robusta:

### Componenti Principali

- **Integrazione API Qubic** - Recupera proposte attive e completate
- **DeepSeek AI** - Crea riassunti multilingue
- **Ponti Discord & Telegram** - Distribuzione multi-piattaforma
- **Archiviazione basata su GitHub** - Gestione dello stato persistente e caching
- **Caching Intelligente** - Evita chiamate API duplicate

## 📋 Lingue Supportate

Il bot supporta attualmente **13 lingue**:

| Lingua | Codice |
|--------|--------|
| Tedesco | `de` |
| Inglese | `en` |
| Francese | `fr` |
| Spagnolo | `es` |
| Italiano | `it` |
| Portoghese | `pt` |
| Russo | `ru` |
| Giapponese | `ja` |
| Cinese | `zh` |
| Coreano | `ko` |
| Arabo | `ar` |
| Turco | `tr` |
| Vietnamita | `vi` |

## 🎯 Funzionalità in Dettaglio

### 🤖 Rilevamento Automatico delle Proposte
- **Intervallo di 15 Minuti** - Verifica regolarmente le nuove proposte
- **Elaborazione per Epoca** - Gestione dello stato separata per epoca
- **Rilevamento Duplicati** - Previene notifiche multiple

### 🧠 Riassunti IA Intelligenti
- **Riassunto Consapevole del Contesto** - Estrae i punti chiave di ogni proposta
- **Formattazione Specifica per Lingua** - Adattata alle sfumature culturali
- **Meccanismo di Cache** - Evita chiamate IA duplicate per le stesse proposte

### 🔄 Gestione dello Stato Robusta
- **Stato per Server/per Chat** - Ogni comunità gestisce il proprio stato
- **Persistenza GitHub** - Gli stati sopravvivono ai riavvii
- **Pulizia Automatica** - Rimuove i dati delle epoche obsolete

### 🌐 Supporto Multi-Piattaforma
- **Integrazione Discord Trasparente** - Comandi slash e messaggi embed
- **Ottimizzazione Telegram** - Tastiere inline e supporto Markdown
- **Esperienza Coerente** - Stesse funzionalità su entrambe le piattaforme

## 💬 Utilizzo Discord

### Aggiungere il Bot al Tuo Server
1. Usa il [**link di invito**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Concedi i **permessi di amministratore** e aggiungi il bot al canale desiderato
3. Esegui la **configurazione** con `/setup`

### Comandi Discord

| **Comando** | **Descrizione** | **Parametri** |
|-------------|-----------------|---------------|
| ❔ `/help` | Mostra aiuto | Aiuto dettagliato e istruzioni |
| ⚙️ `/setup` | Configura il bot per il tuo server | • `channel`: Il canale per i riassunti delle proposte<br>• `language`: Lingua per i riassunti |
| ℹ️ `/info` | Mostra informazioni dettagliate sullo stato del bot | • Canale e lingua configurati<br>• Epoca attuale<br>• Numero di proposte attive<br>• Stato API DeepSeek<br>• Tempo di attività del bot<br>• Intervallo di verifica |

### Aggiungi il bot al tuo gruppo
1. **Gestisci gruppo**
2. **Aggiungi membri**
3. **Cerca bot:** `@QubicTranslationBot`
4. **Aggiungi al gruppo** come amministratore
5. **Abilita** "Gestire i topic" <br>

<img width="358" height="621" alt="admin_italian" src="https://github.com/user-attachments/assets/d9605485-3d39-403a-bd49-e51524bd0c4e" />

6. **Esegui configurazione** con `/setup`

> [!IMPORTANT]
> Il comando `/setup` crea il nuovo argomento "Proposals". Puoi rinominare l'argomento in seguito. Il bot utilizza la chat principale come fallback se non vengono concessi i diritti di amministratore.

### Comandi Telegram

| **Comando** | **Descrizione** | **Parametri** |
|-------------|-----------------|---------------|
| ❔ `/start` o `/help` | Mostra aiuto | Aiuto dettagliato e istruzioni |
| ⚙️ `/setup` | Apre una tastiera inline per la selezione della lingua | • Tastiera inline con opzioni di lingua<br>• Seleziona la lingua desiderata |
| ℹ️ `/info` | Mostra informazioni dettagliate sullo stato del bot | • Chat e lingua configurati<br>• Epoca attuale<br>• Numero di proposte attive<br>• Stato API DeepSeek<br>• Tempo di attività del bot<br>• Intervallo di verifica |

## ⚙️ Gestione dello Stato

Il bot gestisce per ogni epoca:

- **Proposte Elaborate** - Evitazione duplicati
- **Contatore Proposte** - Numerazione continua per epoca
- **Stati Specifici per Lingua** - Permette di cambiare lingua senza perdita di dati

## ❓ Domande Frequenti (FAQ)

### 🤔 Domande Generali

**D: Quali lingue sono supportate?**  
R: Attualmente 13 lingue: Tedesco, Inglese, Francese, Spagnolo, Italiano, Portoghese, Russo, Giapponese, Cinese, Coreano, Arabo, Turco, Vietnamita.

**D: Quanto sono aggiornati i riassunti delle proposte?**  
R: Le nuove proposte vengono rilevate e riassunte entro 15 minuti dalla pubblicazione.

**D: Posso cambiare la lingua in seguito?**  
R: Sì, utilizza semplicemente `/setup` nuovamente. Le proposte già elaborate verranno consegnate nella nuova lingua.

### 🔧 Domande Tecniche

**D: Il bot non risponde ai comandi - cosa fare?**  
R: Assicurati che il bot abbia i permessi necessari e riprova il comando.

**D: Come vengono annunciati i risultati delle votazioni?**  
R: Ogni mercoledì alle 12:15 UTC, i risultati dell'epoca precedente vengono pubblicati automaticamente.

### 🌐 Domande Specifiche per Piattaforma

**D: Tutti i comandi funzionano su entrambe le piattaforme?**  
R: Sì, la funzionalità di base è identica su Discord e Telegram.

**D: Posso usare il bot sia su Discord che Telegram?**  
R: Sì, puoi usare il bot su entrambe le piattaforme in parallelo.

**D: Quali permessi servono al bot su Discord?**  
R: Il bot ha bisogno dei permessi per inviare messaggi, incorporare link e usare i comandi slash.

## 🛠️ Supporto

Per domande o problemi con il bot, contatta:

**📞 Contatto Discord/Telegram:** MDC

**⚠️ Importante:**  
Assicurati di avere le seguenti informazioni pronte:
- ID server/chat dove si verifica il problema
- Comando esatto che non funziona
- Momento del problema
- Messaggio di errore (se disponibile)

---

<div align="center">

**🌍 Un Progetto per la Comunità Qubic**  
*Rendere le proposte accessibili a tutti, in ogni lingua*

</div>
