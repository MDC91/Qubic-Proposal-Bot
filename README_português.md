<div align="center">

# 🤖 Bot de Propostas Qubic

### **Resumos Automáticos de Propostas<br>para a Comunidade Qubic em 13 Idiomas**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
</div>

## 📖 Índice

- [🚀 Sobre o Projeto](#-sobre-o-projeto)
- [🏗️ Arquitetura & Tecnologia](#️-arquitetura--tecnologia)
- [📋 Idiomas Suportados](#-idiomas-suportados)
- [🎯 Funcionalidades em Detalhe](#-funcionalidades-em-detalhe)
- [💬 Uso no Discord](#-uso-no-discord)
  - [Adicionar o Bot ao Seu Servidor](#adicionar-o-bot-ao-seu-servidor)
  - [Comandos do Discord](#comandos-do-discord)
- [📱 Uso no Telegram](#-uso-no-telegram)
  - [Adicionar o Bot ao Seu Grupo](#adicionar-o-bot-ao-seu-grupo)
  - [Comandos do Telegram](#comandos-do-telegram)
- [⚙️ Gerenciamento de Estado](#️-gerenciamento-de-estado)
- [❓ Perguntas Frequentes (FAQ)](#-perguntas-frequentes-faq)
- [🛠️ Suporte](#️-suporte)

## 🚀 Sobre o Projeto

O **Bot de Propostas Qubic** é um bot desenvolvido especificamente para a comunidade Qubic que detecta automaticamente novas propostas de governança, as resume usando IA em 13 idiomas diferentes e as publica em servidores do Discord e grupos do Telegram.

### 🌟 Benefícios Principais

- **🔍 Detecção Automática** - Monitora continuamente novas propostas Qubic
- **🌍 Acessibilidade Multilíngue** - Torna as propostas acessíveis para membros da comunidade não anglófonos
- **🤖 Resumos com IA** - Usa DeepSeek AI para resumos precisos e fáceis de entender
- **⏰ Notificações Oportunas** - Publica novas propostas em 15 minutos após a publicação
- **📊 Resultados de Votação** - Publica automaticamente resultados no final de cada época

## 🏗️ Arquitetura & Tecnologia

O bot é baseado em uma arquitetura multiplataforma robusta:

### Componentes Principais

- **Integração API Qubic** - Recupera propostas ativas e concluídas
- **DeepSeek AI** - Cria resumos multilíngues
- **Pontes Discord & Telegram** - Distribuição multiplataforma
- **Armazenamento baseado no GitHub** - Gerenciamento de estado persistente e cache
- **Cache Inteligente** - Evita chamadas API duplicadas

## 📋 Idiomas Suportados

O bot suporta atualmente **13 idiomas**:

| Idioma | Código |
|--------|--------|
| Alemão | `de` |
| Inglês | `en` |
| Francês | `fr` |
| Espanhol | `es` |
| Italiano | `it` |
| Português | `pt` |
| Russo | `ru` |
| Japonês | `ja` |
| Chinês | `zh` |
| Coreano | `ko` |
| Árabe | `ar` |
| Turco | `tr` |
| Vietnamita | `vi` |

## 🎯 Funcionalidades em Detalhe

### 🤖 Detecção Automática de Propostas
- **Intervalo de 15 Minutos** - Verifica regularmente novas propostas
- **Processamento por Época** - Gerenciamento de estado separado por época
- **Detecção de Duplicados** - Previne notificações múltiplas

### 🧠 Resumos de IA Inteligentes
- **Resumo Consciente do Contexto** - Extrai pontos-chave de cada proposta
- **Formatação Específica por Idioma** - Adaptada a nuances culturais
- **Mecanismo de Cache** - Evita chamadas de IA duplicadas para as mesmas propostas

### 🔄 Gerenciamento de Estado Robusto
- **Estado por Servidor/por Chat** - Cada comunidade gerencia seu próprio estado
- **Persistência no GitHub** - Os estados sobrevivem a reinicializações
- **Limpeza Automática** - Remove dados de época obsoletos

### 🌐 Suporte Multiplataforma
- **Integração Perfeita no Discord** - Comandos slash e mensagens embed
- **Otimização para Telegram** - Teclados inline e suporte Markdown
- **Experiência Consistente** - Mesmas funcionalidades em ambas as plataformas

## 💬 Uso no Discord

### Adicionar o Bot ao Seu Servidor
1. Use o [**link de convite**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Conceda **permissões de administrador** e adicione o bot ao canal desejado
3. Execute a **configuração** com `/setup`

### Comandos do Discord

| **Comando** | **Descrição** | **Parâmetros** |
|-------------|---------------|----------------|
| ❔ `/help` | Mostrar ajuda | Ajuda detalhada e instruções |
| ⚙️ `/setup` | Configura o bot para seu servidor | • `channel`: O canal para resumos de propostas<br>• `language`: Idioma para os resumos |
| ℹ️ `/info` | Mostra informações detalhadas do estado do bot | • Canal e idioma configurados<br>• Época atual<br>• Número de propostas ativas<br>• Estado da API DeepSeek<br>• Tempo de atividade do bot<br>• Intervalo de verificação |

## 📱 Uso no Telegram

### Adicionar o Bot ao Seu Grupo
1. **Gerenciar grupo**
2. **Adicionar membros**
3. **Buscar bot:** `@QubicTranslationBot`
4. **Adicionar ao grupo** como administrador
5. **Executar configuração** no chat desejado com `/setup`

> [!IMPORTANT]
> O comando `/setup` <ins>**deve**</ins> ser usado no chat onde os resumos serão publicados.

### Comandos do Telegram

| **Comando** | **Descrição** | **Parâmetros** |
|-------------|---------------|----------------|
| ❔ `/start` ou `/help` | Mostrar ajuda | Ajuda detalhada e instruções |
| ⚙️ `/setup` | Abre um teclado inline para seleção de idioma | • Teclado inline com opções de idioma<br>• Selecionar idioma desejado |
| ℹ️ `/info` | Mostra informações detalhadas do estado do bot | • Chat e idioma configurados<br>• Época atual<br>• Número de propostas ativas<br>• Estado da API DeepSeek<br>• Tempo de atividade do bot<br>• Intervalo de verificação |

## ⚙️ Gerenciamento de Estado

O bot gerencia para cada época:

- **Propostas Processadas** - Evitação de duplicatas
- **Contador de Propostas** - Numeração contínua por época
- **Estados Específicos por Idioma** - Permite mudar idioma sem perda de dados

## ❓ Perguntas Frequentes (FAQ)

### 🤔 Perguntas Gerais

**P: Quais idiomas são suportados?**  
R: Atualmente 13 idiomas: Alemão, Inglês, Francês, Espanhol, Italiano, Português, Russo, Japonês, Chinês, Coreano, Árabe, Turco, Vietnamita.

**P: Quão atualizados estão os resumos de propostas?**  
R: Novas propostas são detectadas e resumidas em 15 minutos após a publicação.

**P: Posso mudar o idioma depois?**  
R: Sim, simplesmente use `/setup` novamente. Propostas já processadas serão entregues no novo idioma.

### 🔧 Perguntas Técnicas

**P: O bot não responde aos comandos - o que fazer?**  
R: Certifique-se de que o bot tem as permissões necessárias e tente o comando novamente.

**P: Como os resultados de votação são anunciados?**  
R: Toda quarta-feira às 12:15 UTC, os resultados da época anterior são publicados automaticamente.

### 🌐 Perguntas Específicas por Plataforma

**P: Todos os comandos funcionam em ambas as plataformas?**  
R: Sim, a funcionalidade básica é idêntica no Discord e Telegram.

**P: Posso usar o bot tanto no Discord quanto no Telegram?**  
R: Sim, você pode usar o bot em ambas as plataformas em paralelo.

**P: Quais permissões o bot precisa no Discord?**  
R: O bot precisa de permissões para enviar mensagens, incorporar links e usar comandos slash.

## 🛠️ Suporte

Para perguntas ou problemas com o bot, entre em contato com:

**📞 Contato Discord/Telegram:** MDC

**⚠️ Importante:**  
Certifique-se de ter as seguintes informações prontas:
- ID do servidor/chat onde ocorre o problema
- Comando exato que não funciona
- Momento do problema
- Mensagem de erro (se disponível)

---

<div align="center">

**🌍 Um Projeto para a Comunidade Qubic**  
*Tornando as propostas acessíveis a todos, em todos os idiomas*

</div>
