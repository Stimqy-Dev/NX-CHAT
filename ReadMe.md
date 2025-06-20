# S-Chat - Système de Chat Amélioré pour FiveM

## Description

S-Chat est un **rework complet du système de chat de base** de FiveM, offrant une interface utilisateur moderne et des fonctionnalités avancées pour améliorer l'expérience de communication sur votre serveur.

### Fonctionnalités principales :

- 🎨 **Interface moderne** avec animations fluides
- 💬 **Messages multilignes** supportés
- 🔧 **Suggestions de commandes** intelligentes
- 👑 **Intégration ESX** pour la gestion des permissions staff
- 📢 **Commandes d'annonces** pour les administrateurs
- 🎯 **Templates personnalisables** pour les messages
- ⚡ **Performance optimisée** par rapport au chat de base
- 🎨 **Thèmes personnalisables** via CSS

## Installation

### Prérequis

- Serveur FiveM fonctionnel
- Framework ESX (pour les fonctionnalités staff)

### Étapes d'installation

1. **Téléchargement**
   ```bash
   # Clonez ou téléchargez le repository dans votre dossier resources
   cd resources
   git clone [URL_DU_REPO] s-chat
   ```

2. **Configuration du serveur**
   
   Ajoutez cette ligne dans votre `server.cfg` :
   ```cfg
   ensure s-chat
   ```
3. **Redémarrage**
   
   Redémarrez votre serveur ou utilisez :
   ```
   restart s-chat
   ```

## Configuration

### Personnalisation de l'interface

Les fichiers de configuration se trouvent dans le dossier `html/` :

- `config.default.js` - Configuration par défaut
- `config.js` - Votre configuration personnalisée (créez ce fichier)
- `index.css` - Styles CSS personnalisables

## Commandes disponibles

### Commandes joueurs
- `/clearchat` - Efface l'historique du chat

### Commandes administrateur
- `/announce [message]` - Envoie une annonce serveur (console uniquement)

## Fonctionnalités techniques

### Performance
- Chargement optimisé des ressources
- Gestion intelligente de l'affichage des messages
- Nettoyage automatique de la mémoire

## Structure du projet

```
s-chat/
├── client/
│   └── main.lua          # Script client principal
├── server/
│   └── main.lua          # Script serveur principal
├── html/
│   ├── index.html        # Interface principale
│   ├── App.js           # Application Vue.js
│   ├── Message.js       # Composant message
│   ├── Suggestions.js   # Composant suggestions
│   ├── index.css        # Styles CSS
│   ├── config.default.js # Configuration par défaut
│   └── vendor/          # Bibliothèques tierces
├── fxmanifest.lua       # Manifeste FiveM
└── README.md           # Ce fichier
```

## Support et contribution

Ce script est un rework du système de chat de base de FiveM, conçu pour offrir une meilleure expérience utilisateur et plus de fonctionnalités.

### Problèmes connus
- Assurez-vous que le chat de base est bien désactivé
- Vérifiez que ESX est correctement configuré pour les fonctionnalités staff

---

**Note :** Ce script remplace complètement le système de chat de base de FiveM. Assurez-vous de sauvegarder votre configuration existante avant l'installation.