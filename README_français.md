<div align="center">

# 🤖 Qubic Proposal Bot

### **Résumés Automatiques des Propositions pour la Communauté Qubic en 13 Langues**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

--- 
</div>

## 📖 Table des Matières

- [🚀 À Propos du Projet](#-à-propos-du-projet)
- [🏗️ Architecture & Technologie](#️-architecture--technologie)
- [📋 Langues Supportées](#-langues-supportées)
- [🎯 Fonctionnalités en Détail](#-fonctionnalités-en-détail)
- [💬 Utilisation Discord](#-utilisation-discord)
  - [Ajouter le Bot à Votre Serveur](#ajouter-le-bot-à-votre-serveur)
  - [Commandes Discord](#commandes-discord)
- [📱 Utilisation Telegram](#-utilisation-telegram)
  - [Ajouter le Bot à Votre Groupe](#ajouter-le-bot-à-votre-groupe)
  - [Commandes Telegram](#commandes-telegram)
- [⚙️ Gestion d'État](#️-gestion-détat)
- [❓ Questions Fréquemment Posées (FAQ)](#-questions-fréquemment-posées-faq)
- [🛠️ Support](#️-support)

## 🚀 À Propos du Projet

Le **Bot de Propositions Qubic** est un bot spécialement développé pour la communauté Qubic qui détecte automatiquement les nouvelles propositions de gouvernance, les résume en utilisant l'IA dans 13 langues différentes et les publie dans les serveurs Discord et les groupes Telegram.

### 🌟 Avantages Principaux

- **🔍 Détection Automatique** - Surveille continuellement les nouvelles propositions Qubic
- **🌍 Accessibilité Multilingue** - Rend les propositions accessibles aux membres de la communauté non anglophones
- **🤖 Résumés par IA** - Utilise DeepSeek AI pour des résumés précis et faciles à comprendre
- **⏰ Notifications Rapides** - Publie les nouvelles propositions dans les 15 minutes suivant leur publication
- **📊 Résultats des Votes** - Publie automatiquement les résultats à la fin de chaque époque

## 🏗️ Architecture & Technologie

Le bot est basé sur une architecture multi-plateforme robuste :

### Composants Principaux

- **Intégration API Qubic** - Récupère les propositions actives et terminées
- **DeepSeek AI** - Crée des résumés multilingues
- **Ponts Discord & Telegram** - Distribution multiplateforme
- **Stockage basé sur GitHub** - Gestion d'état persistante et mise en cache
- **Cache Intelligent** - Évite les appels API en double

## 📋 Langues Supportées

Le bot supporte actuellement **13 langues** :

| Langue | Code |
|--------|------|
| Allemand | `de` |
| Anglais | `en` |
| Français | `fr` |
| Espagnol | `es` |
| Italien | `it` |
| Portugais | `pt` |
| Russe | `ru` |
| Japonais | `ja` |
| Chinois | `zh` |
| Coréen | `ko` |
| Arabe | `ar` |
| Turc | `tr` |
| Vietnamien | `vi` |

## 🎯 Fonctionnalités en Détail

### 🤖 Détection Automatique des Propositions
- **Intervalle de 15 Minutes** - Vérifie régulièrement les nouvelles propositions
- **Traitement par Époque** - Gestion d'état séparée par époque
- **Détection des Doublons** - Empêche les notifications multiples

### 🧠 Résumés IA Intelligents
- **Résumé Contextuel** - Extrait les points clés de chaque proposition
- **Formatage Spécifique à la Langue** - Adapté aux nuances culturelles
- **Mécanisme de Cache** - Évite les appels IA en double pour les mêmes propositions

### 🔄 Gestion d'État Robuste
- **État par Serveur/par Chat** - Chaque communauté gère son propre statut
- **Persistance GitHub** - Les états survivent aux redémarrages
- **Nettoyage Automatique** - Supprime les données d'époque obsolètes

### 🌐 Support Multi-Plateforme
- **Intégration Discord Transparente** - Commandes slash et messages embed
- **Optimisation Telegram** - Claviers inline et support Markdown
- **Expérience Cohérente** - Mêmes fonctionnalités sur les deux plateformes

## 💬 Utilisation Discord

### Ajouter le Bot à Votre Serveur
1. Utilisez le [**lien d'invitation**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Accordez les **permissions administrateur** et ajoutez le bot au canal souhaité
3. Effectuez la **configuration** avec `/setup`

### Commandes Discord

| **Commande** | **Description** | **Paramètres** |
|--------------|-----------------|----------------|
| ❔ `/help` | Afficher l'aide | Aide détaillée et instructions |
| ⚙️ `/setup` | Configure le bot pour votre serveur | • `channel`: Le canal pour les résumés de propositions<br>• `language`: Langue pour les résumés |
| ℹ️ `/info` | Affiche des informations détaillées sur l'état du bot | • Canal et langue configurés<br>• Époque actuelle<br>• Nombre de propositions actives<br>• Statut de l'API DeepSeek<br>• Temps de fonctionnement du bot<br>• Intervalle de vérification |

## 📱 Utilisation Telegram

### Ajouter le Bot à Votre Groupe
1. **Gérer le groupe**
2. **Ajouter des membres**
3. **Rechercher le bot :** `@QubicTranslationBot`
4. **Ajouter au groupe** en tant qu'administrateur
5. **Effectuer la configuration** dans le chat souhaité avec `/setup`

> [!IMPORTANT]
> La commande `/setup` <ins>**doit**</ins> être utilisée dans le chat où les résumés doivent être publiés.

### Commandes Telegram

| **Commande** | **Description** | **Paramètres** |
|--------------|-----------------|----------------|
| ❔ `/start` ou `/help` | Afficher l'aide | Aide détaillée et instructions |
| ⚙️ `/setup` | Ouvre un clavier inline pour la sélection de la langue | • Clavier inline avec options de langue<br>• Sélectionner la langue souhaitée |
| ℹ️ `/info` | Affiche des informations détaillées sur l'état du bot | • Chat et langue configurés<br>• Époque actuelle<br>• Nombre de propositions actives<br>• Statut de l'API DeepSeek<br>• Temps de fonctionnement du bot<br>• Intervalle de vérification |

## ⚙️ Gestion d'État

Le bot gère pour chaque époque :

- **Propositions Traitées** - Évitation des doublons
- **Compteur de Propositions** - Numérotation continue par époque
- **États Spécifiques à la Langue** - Permet de changer de langue sans perte de données

## ❓ Questions Fréquemment Posées (FAQ)

### 🤔 Questions Générales

**Q: Quelles langues sont supportées ?**  
R: Actuellement 13 langues : Allemand, Anglais, Français, Espagnol, Italien, Portugais, Russe, Japonais, Chinois, Coréen, Arabe, Turc, Vietnamien.

**Q: Quelle est l'actualité des résumés de propositions ?**  
R: Les nouvelles propositions sont détectées et résumées dans les 15 minutes suivant leur publication.

**Q: Puis-je changer la langue plus tard ?**  
R: Oui, utilisez simplement `/setup` à nouveau. Les propositions déjà traitées seront livrées dans la nouvelle langue.

### 🔧 Questions Techniques

**Q: Le bot ne répond pas aux commandes - que faire ?**  
R: Assurez-vous que le bot a les permissions nécessaires et réessayez la commande.

**Q: Comment les résultats des votes sont-ils annoncés ?**  
R: Chaque mercredi à 12:15 UTC, les résultats de l'époque précédente sont automatiquement publiés.

### 🌐 Questions Spécifiques à la Plateforme

**Q: Toutes les commandes fonctionnent-elles sur les deux plateformes ?**  
R: Oui, la fonctionnalité de base est identique sur Discord et Telegram.

**Q: Puis-je utiliser le bot sur Discord et Telegram ?**  
R: Oui, vous pouvez utiliser le bot sur les deux plateformes en parallèle.

**Q: Quelles permissions le bot nécessite-t-il sur Discord ?**  
R: Le bot a besoin des permissions pour envoyer des messages, intégrer des liens et utiliser les commandes slash.

## 🛠️ Support

Pour des questions ou des problèmes avec le bot, veuillez contacter :

**📞 Contact Discord/Telegram :** MDC

**⚠️ Important :**  
Veuillez vous assurer d'avoir les informations suivantes prêtes :
- ID du serveur/chat où le problème se produit
- Commande exacte qui ne fonctionne pas
- Moment du problème
- Message d'erreur (si disponible)

---

<div align="center">

**🌍 Un Projet pour la Communauté Qubic**  
*Rendre les propositions accessibles à tous, dans toutes les langues*

</div>
