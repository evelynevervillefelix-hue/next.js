# 🚀 Déploiement Simple - Stock MR Application

## ⚡ Méthode Rapide (Sans Cloud Build)

Cette méthode est la plus simple et la plus rapide pour déployer votre application sur Firebase Hosting.

---

## 📋 Prérequis

1. **Node.js et npm** installés
   - Télécharger : https://nodejs.org/
   - Vérifier : `node --version` et `npm --version`

2. **Compte Firebase** (déjà créé)
   - Projet : **mrmega-461f4**

---

## 🎯 Étapes de Déploiement (5 minutes)

### Étape 1 : Installer Firebase CLI

Ouvrez un terminal/invite de commande et exécutez :

```bash
npm install -g firebase-tools
```

### Étape 2 : Se Connecter à Firebase

```bash
firebase login
```

**Cela ouvrira votre navigateur. Connectez-vous avec votre compte Google et autorisez l'accès.**

### Étape 3 : Naviguer vers le Dossier

```bash
cd chemin/vers/megastockmr
```

(Remplacez `chemin/vers/megastockmr` par le chemin réel du dossier que vous avez décompressé)

### Étape 4 : Déployer l'Application

```bash
firebase deploy --only hosting
```

**Attendez que le déploiement se termine. Vous verrez :**

```
✔  Deploy complete!

Project Console: https://console.firebase.google.com/project/mrmega-461f4/overview
Hosting URL: https://mrmega-461f4.web.app
```

---

## ✅ C'est Fini !

Votre application est maintenant en ligne à l'adresse :

### 🌐 **https://mrmega-461f4.web.app**

---

## 📲 Accéder depuis iPhone

1. Ouvrez **Safari** (ou un autre navigateur)
2. Allez à : **https://mrmega-461f4.web.app**
3. L'application s'affichera parfaitement avec le design complet !

**Partagez cette URL avec les 4 autres membres de votre équipe.**

---

## 📊 Importer les Données

Une fois en ligne :

### 1️⃣ Importer les Véhicules

1. Onglet **"🚗 Stock"**
2. Bouton **"📥 Importer CSV"**
3. Fichier : **`STOCK MR ACHAT RICHARD - STOCK GLOBAL (1).csv`**
4. Attendez la confirmation

### 2️⃣ Importer les Factures

1. Onglet **"📑 Factures"**
2. Bouton **"📥 Importer CSV"**
3. Fichier : **`factures_initiales.csv`**
4. Attendez la confirmation

---

## 🎮 Utilisation

### Voir les Détails d'un Véhicule

1. Onglet **"🚗 Stock"**
2. Cliquez sur **"👁️"** (œil) du véhicule
3. Vous verrez :
   - Toutes les factures liées
   - Coût total (achat + factures)
   - Profit/Perte (vente - coût total)

### Ajouter une Nouvelle Facture

1. Onglet **"📑 Factures"**
2. Cliquez **"➕ Ajouter Facture"**
3. Sélectionnez le véhicule (MR)
4. Remplissez et enregistrez

---

## 🔄 Synchronisation Multi-Utilisateur

**Tous les utilisateurs voient les mêmes données en temps réel !**

Lorsqu'une personne ajoute/modifie/supprime un véhicule ou une facture, les autres utilisateurs voient la mise à jour instantanément.

---

## 🆘 Problèmes Courants

### "firebase: command not found"
**Solution :** Réinstallez Firebase CLI :
```bash
npm install -g firebase-tools
```

### "Permission denied"
**Solution :** Assurez-vous d'être connecté :
```bash
firebase login
```

### "Cannot find module 'firebase'"
**Solution :** Vous êtes probablement dans le mauvais dossier. Assurez-vous d'être dans le dossier `megastockmr` :
```bash
cd chemin/vers/megastockmr
```

---

## 📞 Besoin d'Aide ?

Si vous avez des problèmes :

1. Vérifiez que **Node.js** est installé : `node --version`
2. Vérifiez que **Firebase CLI** est installé : `firebase --version`
3. Vérifiez que vous êtes **connecté** : `firebase login`
4. Vérifiez que vous êtes dans le **bon dossier** : `ls` (devrait afficher `index.html`, `app.js`, etc.)

---

## 🎉 Bravo !

Votre application **Stock MR** est maintenant en ligne !

**URL** : https://mrmega-461f4.web.app

Partagez cette URL avec votre équipe et commencez à gérer votre stock ensemble depuis n'importe quel iPhone ! 📱
