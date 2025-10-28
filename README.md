<div align="center">
  
# 🤖 Qubic Proposal Bot

### **Automatic Proposal Summaries for the Qubic Community in 13 Languages**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
</div>

## 📖 Table of Contents

- [🚀 About the Project](#-about-the-project)
- [🏗️ Architecture & Technology](#️-architecture--technology)
- [📋 Supported Languages](#-supported-languages)
- [🎯 Features in Detail](#-features-in-detail)
- [💬 Discord Usage](#-discord-usage)
  - [Add Bot to Your Server](#add-bot-to-your-server)
  - [Discord Commands](#discord-commands)
- [📱 Telegram Usage](#-telegram-usage)
  - [Add Bot to Your Group](#add-bot-to-your-group)
  - [Telegram Commands](#telegram-commands)
- [⚙️ State Management](#️-state-management)
- [❓ Frequently Asked Questions (FAQ)](#-frequently-asked-questions-faq)
- [🛠️ Support](#️-support)

## 🚀 About the Project

The **Qubic Proposal Bot** is a bot specifically developed for the Qubic community that automatically detects new governance proposals, summarizes them using AI in 13 different languages, and publishes them in Discord servers and Telegram groups.

### 🌟 Main Benefits

- **🔍 Automatic Detection** - Continuously monitors new Qubic proposals
- **🌍 Multilingual Accessibility** - Makes proposals available for non-English speaking community members
- **🤖 AI-Powered Summaries** - Uses DeepSeek AI for precise, easy-to-understand summaries
- **⏰ Timely Notifications** - Posts new proposals within 15 minutes of publication
- **📊 Voting Results** - Automatically publishes results at the end of each epoch

## 🏗️ Architecture & Technology

The bot is based on a robust multi-platform architecture:

### Core Components

- **Qubic API Integration** - Retrieves active and completed proposals
- **DeepSeek AI** - Creates multilingual summaries
- **Discord & Telegram Bridges** - Cross-platform distribution
- **GitHub-based Storage** - Persistent state management and caching
- **Intelligent Caching** - Avoids duplicate API calls

## 📋 Supported Languages

The bot currently supports **13 languages**:

| Language | Code |
|----------|------|
| German | `de` |
| English | `en` |
| French | `fr` |
| Spanish | `es` |
| Italian | `it` |
| Portuguese | `pt` |
| Russian | `ru` |
| Japanese | `ja` |
| Chinese | `zh` |
| Korean | `ko` |
| Arabic | `ar` |
| Turkish | `tr` |
| Vietnamese | `vi` |

## 🎯 Features in Detail

### 🤖 Automatic Proposal Detection
- **15-Minute Interval** - Regularly checks for new proposals
- **Epoch-based Processing** - Separate state management per epoch
- **Duplicate Detection** - Prevents multiple notifications

### 🧠 Intelligent AI Summaries
- **Context-Aware Summarization** - Extracts key points from each proposal
- **Language-Specific Formatting** - Adapted to cultural nuances
- **Cache Mechanism** - Avoids duplicate AI calls for the same proposals

### 🔄 Robust State Management
- **Per-Server/Per-Chat State** - Each community manages its own status
- **GitHub Persistence** - States survive restarts
- **Automatic Cleanup** - Removes outdated epoch data

### 🌐 Multi-Platform Support
- **Seamless Discord Integration** - Slash commands and embed messages
- **Telegram Optimization** - Inline keyboards and Markdown support
- **Consistent Experience** - Same features on both platforms

## 💬 Discord Usage

### Add Bot to Your Server
1. Use the [**invitation link**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Grant **admin permissions** and add the bot to the desired channel
3. Perform **setup** with `/setup`

### Discord Commands

| **Command** | **Description** | **Parameters** |
|-------------|-----------------|----------------|
| ❔ `/help` | Show help | Detailed help and instructions |
| ⚙️ `/setup` | Sets up the bot for your server | • `channel`: The channel for proposal summaries<br>• `language`: Language for the summaries |
| ℹ️ `/info` | Shows detailed information about bot status | • Configured channel and language<br>• Current epoch<br>• Number of active proposals<br>• DeepSeek API status<br>• Bot uptime<br>• Check interval |

## 📱 Telegram Usage

### Add Bot to Your Group
1. **Manage group**
2. **Add members**
3. **Search for bot:** `@QubicTranslationBot`
4. **Add to group** as administrator
5. **Enable** "Manage Topics" <br>

<img width="363" height="621" alt="admin_rights" src="https://github.com/user-attachments/assets/f11920b4-213a-4361-aaf8-cd66f2fcc383" />


7. **Perform setup** with `/setup`

> [!IMPORTANT]
> The `/setup` command is creating the new topic "Proposals". You can rename the topic afterwards.

### Telegram Commands

| **Command** | **Description** | **Parameters** |
|-------------|-----------------|----------------|
| ❔ `/start` or `/help` | Show help | Detailed help and instructions |
| ⚙️ `/setup` | Opens an inline keyboard for language selection | • Inline keyboard with language options<br>• Select desired language |
| ℹ️ `/info` | Shows detailed information about bot status | • Configured chat and language<br>• Current epoch<br>• Number of active proposals<br>• DeepSeek API status<br>• Bot uptime<br>• Check interval |

## ⚙️ State Management

The bot manages for each epoch:

- **Processed Proposals** - Avoidance of duplicates
- **Proposal Counter** - Continuous numbering per epoch
- **Language-Specific States** - Enables language switching without data loss

## ❓ Frequently Asked Questions (FAQ)

### 🤔 General Questions

**Q: Which languages are supported?**  
A: Currently 13 languages: German, English, French, Spanish, Italian, Portuguese, Russian, Japanese, Chinese, Korean, Arabic, Turkish, Vietnamese.

**Q: How current are the proposal summaries?**  
A: New proposals are detected and summarized within 15 minutes of publication.

**Q: Can I change the language later?**  
A: Yes, simply use `/setup` again. Already processed proposals will be delivered in the new language.

### 🔧 Technical Questions

**Q: The bot doesn't respond to commands - what to do?**  
A: Make sure the bot has the necessary permissions and try the command again.

**Q: How are voting results announced?**  
A: Every Wednesday at 12:15 UTC, the results of the previous epoch are automatically posted.

### 🌐 Platform-Specific Questions

**Q: Do all commands work on both platforms?**  
A: Yes, the core functionality is identical on Discord and Telegram.

**Q: Can I use the bot on both Discord and Telegram?**  
A: Yes, you can use the bot on both platforms in parallel.

**Q: What permissions does the bot need on Discord?**  
A: The bot needs permissions to send messages, embed links, and use slash commands.

## 🛠️ Support

For questions or problems with the bot, please contact:

**📞 Discord/Telegram Contact:** MDC

**⚠️ Important:**  
Please make sure you have the following information ready:
- Server/Chat ID where the problem occurs
- Exact command that doesn't work
- Time of the problem
- Error message (if available)

---

<div align="center">

**🌍 A Project for the Qubic Community**  
*Making proposals accessible to everyone, in every language*

</div>
