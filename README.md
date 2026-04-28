<div align="center">
  
# 🤖 TOGE-MD-V5

<img src="https://wallpapercave.com/wp/wp9620389.jpg" alt="TOGE-MD-V5 Banner" width="100%"/>

[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://whatsapp.com/channel/0029VaiJZmPxVzKkK5p3PW0U)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/toge021/TOGE-MD-V5)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)

**Un bot WhatsApp multi-session puissant, modulaire et sécurisé**

</div>

---

## 📖 À propos

**TOGE-MD-V5** est un bot WhatsApp nouvelle génération développé avec `@whiskeysockets/baileys`. Il se distingue par sa **capacité à gérer plusieurs comptes WhatsApp simultanément** avec une isolation totale des données. Chaque session possède sa propre configuration, sa base de données, ses modérateurs, ses bannis et même son propre personnage !

Que vous souhaitiez automatiser la gestion de vos groupes, créer un assistant personnel ou déployer un bot communautaire, TOGE-MD-V5 s'adapte à tous vos besoins.

---

## ✨ Fonctionnalités principales

### 🔌 Multi-Session avancé
- Gestion de **plusieurs comptes WhatsApp** en parallèle
- **Isolation complète** : chaque session a ses propres fichiers (config, DB, mods, bans)
- Stockage sécurisé dans `./sessions/session_<numéro>/`
- Connexion automatique au redémarrage

### 🔐 Système de couplage (Pairing Code)
- **Connexion sans QR code** via code à 8 chiffres
- Compatible avec tous les appareils WhatsApp
- Génération automatique si aucune session n'existe

### 👑 Système de modération complet
- **Propriétaire** : contrôle total
- **Modérateurs** : gestion des groupes et utilisateurs
- **Sudoers** : liste blanche d'utilisateurs autorisés
- **Modes disponibles** :
  - `public` : tout le monde peut utiliser le bot
  - `self` : uniquement le propriétaire
  - `private` : uniquement les utilisateurs autorisés

### 🎭 Personnages personnalisables
- Changez la personnalité du bot avec `.setchar`
- Plusieurs personnages pré-définis
- Chaque session peut avoir son propre personnage
- Dialogues contextuels adaptés

### 🛡️ Système Anti-Abuse
| Protection | Description |
|------------|-------------|
| Anti-flood | Limite le nombre de messages par utilisateur |
| Anti-spam | Bloque les messages répétitifs |
| Anti-delete | Détecte et log les messages supprimés |
| Anti-viewonce | Télécharge les messages éphémères |
| Anti-link | Bloque les liens WhatsApp et généraux |
| Anti-tag | Empêche les mentions abusives |
| Anti-kick | Protège le bot contre l'expulsion |
| Auto-kick | Expulsion temporisée des indésirables |

### 📨 Gestion de groupes intelligente
- **Messages personnalisés** : bienvenue et au revoir avec photo de profil
- **Anti-promote/demote** : bloque les promotions/déclassements abusifs
- **Auto-accept** : acceptation automatique des demandes d'entrée
- **Gestion des admins** : promote, demote, kick, add
- **Configuration par groupe** : réglages individuels pour chaque groupe

### 🧠 Modules supplémentaires
- **Chatbot privé** : discussion intelligente en message privé
- **Auto-typing** : simule l'écriture naturelle
- **Auto-recording** : simulation d'enregistrement audio
- **Auto-like status** : like automatique des statuts WhatsApp
- **Auto-verse** : verset biblique programmé quotidiennement
- **Night mode** : désactivation programmée du bot la nuit
- **Sauvegarde des statuts** : téléchargement des statuts éphémères
- **Journalisation** : logs des conversations importantes

### 📎 Gestion des médias
- Téléchargement des `view once` (messages éphémères)
- Envoi d'images, vidéos, stickers, audio (PTT)
- Envoi de documents, contacts, localisation
- Résolution automatique des LID (identifiants temporaires)

---

## 📋 Commandes principales (préfixe : `.`)

### 👑 Propriétaire & Modération
```bash
.setmod @user      # Ajouter un modérateur
.removemod @user   # Retirer un modérateur
.mods              # Liste des modérateurs
.ban @user         # Bannir un utilisateur
.unban @user       # Lever le bannissement
.banlist           # Liste des bannis
.mode public/self/private  # Changer le mode
.sudo add/remove   # Gérer la liste blanche
