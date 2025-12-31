# Politique de Confidentialité - IndéFiscal

Ce dépôt contient la politique de confidentialité d'IndéFiscal, hébergée sur GitHub Pages.

## 🚀 Instructions de déploiement

### Étape 1 : Créer le dépôt GitHub

1. Va sur [github.com](https://github.com) et connecte-toi
2. Clique sur le bouton **"New"** (ou "+" → "New repository")
3. Configure le dépôt :
   - **Repository name** : `indefiscal-privacy`
   - **Description** : `Politique de confidentialité pour l'application IndéFiscal`
   - **Public** ou **Private** : Sélectionne **Public** (obligatoire pour GitHub Pages gratuit)
   - ❌ **Ne coche PAS** "Add a README file" (on va l'ajouter après)
4. Clique sur **"Create repository"**

### Étape 2 : Uploader les fichiers

**Option A : Via l'interface web GitHub (le plus simple)**

1. Sur la page de ton nouveau dépôt, clique sur **"uploading an existing file"**
2. Drag & drop les fichiers :
   - `index.html`
   - `README.md`
3. Scroll en bas et clique sur **"Commit changes"**

**Option B : Via Git en ligne de commande**

```bash
# Clone le dépôt
git clone https://github.com/TON_USERNAME/indefiscal-privacy.git
cd indefiscal-privacy

# Copie les fichiers index.html et README.md dans ce dossier

# Ajoute et commit
git add .
git commit -m "Add privacy policy"
git push origin main
```

### Étape 3 : Activer GitHub Pages

1. Sur GitHub, va dans ton dépôt `indefiscal-privacy`
2. Clique sur **"Settings"** (⚙️ en haut)
3. Dans le menu de gauche, clique sur **"Pages"** (sous "Code and automation")
4. Dans **"Source"**, sélectionne :
   - **Branch** : `main` (ou `master`)
   - **Folder** : `/ (root)`
5. Clique sur **"Save"**
6. ⏱️ Attends 1-2 minutes que GitHub déploie ta page

### Étape 4 : Récupérer l'URL

1. Rafraîchis la page **Settings → Pages**
2. Tu verras un message en haut :
   ```
   Your site is live at https://TON_USERNAME.github.io/indefiscal-privacy/
   ```
3. **C'est cette URL que tu vas mettre dans App Store Connect !**

### Étape 5 : Vérifier que ça fonctionne

1. Ouvre l'URL dans ton navigateur : `https://TON_USERNAME.github.io/indefiscal-privacy/`
2. Tu devrais voir ta politique de confidentialité s'afficher correctement

### Étape 6 : Ajouter l'URL dans App Store Connect

1. Retourne sur [App Store Connect](https://appstoreconnect.apple.com)
2. Va dans **Mes Apps** → **IndéFiscal**
3. Clique sur **"App Information"** (dans le menu de gauche)
4. Dans le champ **"Privacy Policy URL"**, colle :
   ```
   https://TON_USERNAME.github.io/indefiscal-privacy/
   ```
   (Remplace `TON_USERNAME` par ton nom d'utilisateur GitHub)
5. Clique sur **"Save"** en haut à droite

---

## ✏️ Personnalisation

### Modifier l'email de contact

Dans le fichier `index.html`, cherche la ligne 263 :

```html
<strong>Email :</strong> contact@indefiscal.app<br>
```

Remplace par ton vrai email :

```html
<strong>Email :</strong> ton.email@exemple.com<br>
```

### Modifier le nom du développeur

Dans le fichier `index.html`, cherche la ligne 265 :

```html
<strong>Développeur :</strong> [Votre nom ou nom de votre société]
```

Remplace par :

```html
<strong>Développeur :</strong> Ton Nom
```

---

## 🔄 Mettre à jour la politique plus tard

Si tu veux modifier ta politique de confidentialité plus tard :

1. Modifie le fichier `index.html` localement
2. Change la date dans cette ligne (ligne 42) :
   ```html
   <div class="last-update">Dernière mise à jour : 31 décembre 2024</div>
   ```
3. Uploade le fichier modifié sur GitHub (remplace l'ancien)
4. GitHub Pages se mettra automatiquement à jour en 1-2 minutes

---

## ✅ Checklist finale

- [ ] Dépôt GitHub créé et public
- [ ] Fichiers `index.html` et `README.md` uploadés
- [ ] GitHub Pages activé (Settings → Pages)
- [ ] URL récupérée : `https://TON_USERNAME.github.io/indefiscal-privacy/`
- [ ] URL testée dans le navigateur (elle affiche bien la page)
- [ ] Email de contact personnalisé dans `index.html`
- [ ] Nom du développeur personnalisé dans `index.html`
- [ ] URL ajoutée dans App Store Connect → App Information → Privacy Policy URL
- [ ] Sauvegardé dans App Store Connect

---

## ❓ Problèmes fréquents

**La page GitHub affiche un 404**
- Attends 2-3 minutes après activation de GitHub Pages
- Vérifie que le dépôt est bien "Public"
- Vérifie que tu as bien sélectionné la branch `main` dans Settings → Pages

**L'URL ne fonctionne pas dans App Store Connect**
- Vérifie que l'URL commence bien par `https://`
- Vérifie qu'il n'y a pas d'espaces ou de fautes de frappe
- Assure-toi que la page est bien accessible publiquement

**Je veux changer l'URL plus tard**
- Tu peux renommer ton dépôt dans Settings → General → Repository name
- La nouvelle URL sera : `https://TON_USERNAME.github.io/NOUVEAU_NOM/`
- N'oublie pas de mettre à jour l'URL dans App Store Connect

---

## 📧 Support

Si tu as des questions sur le déploiement, crée une issue sur ce dépôt ou contacte-moi.

---

**Licence** : Ce document est fourni "tel quel" pour l'application IndéFiscal. Tu es libre de le modifier selon tes besoins.
