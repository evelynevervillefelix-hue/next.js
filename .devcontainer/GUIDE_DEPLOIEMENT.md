# 📱 Guide de Déploiement - Stock MR Application

## 🎯 Objectif
Déployer l'application **Stock MR** sur **Firebase Hosting** pour y accéder depuis n'importe quel iPhone avec une URL web permanente.

---

## 📋 Prérequis

1. **Node.js et npm** installés sur votre ordinateur
   - Télécharger depuis : https://nodejs.org/
   
2. **Compte Firebase** (déjà créé)
   - Projet : **mrmega-461f4**

3. **Accès à un ordinateur** (pour cette étape unique de déploiement)

---

## 🚀 Étapes de Déploiement

### Étape 1 : Installer Firebase CLI

Ouvrez un terminal/invite de commande sur votre ordinateur et exécutez :

```bash
npm install -g firebase-tools
```

### Étape 2 : Se Connecter à Firebase

```bash
firebase login
```

Cela ouvrira votre navigateur pour vous connecter avec votre compte Google. Autorisez l'accès.

### Étape 3 : Initialiser le Projet

Naviguez vers le dossier `megastockmr` que vous avez décompressé :

```bash
cd chemin/vers/megastockmr
```

Initialisez Firebase Hosting :

```bash
firebase init hosting
```

**Répondez aux questions comme suit :**
- `What do you want to use as your public directory?` → Tapez : `.` (point)
- `Configure as a single-page app?` → Tapez : `y` (oui)
- `Set up automatic builds and deploys with GitHub?` → Tapez : `n` (non)

### Étape 4 : Déployer l'Application

```bash
ffirebase init hosting
```

Attendez que le déploiement se termine. Vous verrez un message comme :

```
✔  Deploy complete!

Project Console: https://console.firebase.google.com/project/mrmega-461f4/overview
Hosting URL: https://mrmega-461f4.web.app
```

**Notez l'URL de Hosting** (ex: `https://mrmega-461f4.web.app`)

---

## 📲 Accéder à l'Application sur iPhone

1. Ouvrez Safari (ou un autre navigateur) sur votre iPhone
2. Allez à l'URL : `https://mrmega-461f4.web.app`
3. L'application s'affichera avec le design complet et fonctionnera parfaitement !

**Vous pouvez partager cette URL avec les 4 autres membres de votre équipe.**

---

## 📊 Importer les Données Initiales

Une fois l'application en ligne :

### 1️⃣ Importer les Véhicules

1. Cliquez sur l'onglet **"🚗 Stock"**
2. Cliquez sur le bouton **"📥 Importer CSV"**
3. Sélectionnez le fichier : **`STOCK MR ACHAT RICHARD - STOCK GLOBAL (1).csv`**
4. Attendez que l'import se termine (vous verrez un message de confirmation)

### 2️⃣ Importer les Factures

1. Cliquez sur l'onglet **"📑 Factures"**
2. Cliquez sur le bouton **"📥 Importer CSV"**
3. Sélectionnez le fichier : **`factures_initiales.csv`**
4. Attendez que l'import se termine

---

## ✅ Vérification

Après l'import :

1. Allez à l'onglet **"🚗 Stock"**
2. Vous devriez voir **106 véhicules** affichés
3. Cliquez sur le bouton **"👁️"** (œil) d'un véhicule pour voir ses détails
4. Vous verrez toutes les factures liées à ce véhicule et le **Profit/Perte** calculé automatiquement

---

## 🎮 Utilisation de l'Application

### Ajouter un Nouveau Véhicule
1. Onglet **"🚗 Stock"**
2. Bouton **"➕ Ajouter Véhicule"**
3. Remplissez le formulaire et cliquez **"Enregistrer"**

### Ajouter une Facture
1. Onglet **"📑 Factures"**
2. Bouton **"➕ Ajouter Facture"**
3. Sélectionnez le véhicule (MR) concerné
4. Remplissez les détails et cliquez **"Enregistrer"**

### Voir les Détails d'un Véhicule
1. Onglet **"🚗 Stock"**
2. Cliquez sur le bouton **"👁️"** (œil) du véhicule
3. Vous verrez :
   - Toutes les factures liées
   - Le coût total (achat + factures)
   - Le profit/perte (vente - coût total)

### Statistiques
1. Onglet **"⚙️ Admin"**
2. Vous verrez les statistiques globales de votre stock

---

## 🔄 Synchronisation Multi-Utilisateur

**Tous les utilisateurs qui accèdent à l'URL verront les mêmes données en temps réel.**

Lorsqu'une personne ajoute/modifie/supprime un véhicule ou une facture, les autres utilisateurs verront la mise à jour instantanément.

---

## 📞 Besoin d'Aide ?

Si vous rencontrez des problèmes :

1. **Vérifiez que Node.js est installé** : `node --version`
2. **Vérifiez que Firebase CLI est installé** : `firebase --version`
3. **Assurez-vous d'être connecté** : `firebase login`
4. **Vérifiez le statut du déploiement** : `firebase hosting:channel:list`

---

## 🎉 Bravo !

Votre application **Stock MR** est maintenant en ligne et accessible depuis n'importe quel iPhone !

**URL Permanente** : `https://mrmega-461f4.web.app`

Partagez cette URL avec votre équipe et commencez à gérer votre stock ensemble.
