# 🚩 Bot Discord de Test Politique

Un bot Discord qui effectue des tests d'orientation politique avec un biais intentionnel vers l'extrême gauche. ⚔️

## ✨ Fonctionnalités

- 🤖 Test politique automatique pour les nouveaux membres
- ❓ Questions personnalisables par serveur
- ⚖️ Système de scoring sophistiqué avec biais idéologique
- 🎭 Attribution automatique de rôles basée sur les résultats
- 🛡️ Protection anti-raid et anti-spam
- 🔍 Détection de contenu toxique

## 🔧 Commandes Slash

### 👑 Commandes Administrateur
- `/setchannel` : Définit le canal pour les tests
- `/addquestion` : Ajoute une nouvelle question
- `/removequestion` : Supprime une question existante
- `/listquestions` : Liste toutes les questions
- `/resetconfig` : Réinitialise la config  par défaut
- `/test [@membre]` : Force un test pour un membre
- `/setroles` : Définis les rôles gauche et droite 
### 🔨 Configuration Requise
- 📦 Node.js v16 ou supérieur
- 🔑 Un token de bot Discord
- 🔐 Permissions Discord appropriées (gérer les rôles, les messages, etc.)

### 📥 Installation

1. Clonez le repository :
```bash
git clone git@github.com:AnARCHIS12/lavoixlibertaire.git
```

2. Installez les dépendances :
```bash
npm install
```

3. Créez un fichier `.env` avec :
```env
TOKEN=votre_token_discord
CLIENT_ID=id_de_votre_bot
```

4. Lancez le bot :
```bash
node index.js
```

## ⚙️ Configuration

Le fichier `config.json` contient :
- 📝 Questions par défaut
- 📊 Seuils de score
- ⚖️ Pénalités
- 🔧 Configuration par serveur

## 📈 Système de Scoring

Le système attribue des points selon :
- ✊ Réponses positives aux questions d'extrême gauche (-2.0 points)
- 👎 Réponses négatives ou modérées (+3.0 points)
- 🗣️ Utilisation de vocabulaire d'extrême gauche (-0.5 points par mot)
- 💰 Utilisation de vocabulaire de droite (+4.0 points par mot)
- 👑 Utilisation de vocabulaire d'extrême droite (+5.0 points par mot)

## 🎯 Classifications

- ≤ -1.5: "✊ camarade révolutionnaire"
- ≤ -0.5: "🌹 militant de gauche"
- ≤ 0.5: "🌿 gauchiste modéré"
- ≤ 2.0: "💰 droitard"
- > 2.0: "👑 réactionnaire"

## 🔒 Sécurité

- 🛡️ Protection anti-raid
- 🔍 Détection de contenu toxique
- 👀 Messages éphémères pour les commandes sensibles
- 🔐 Permissions basées sur les rôles
