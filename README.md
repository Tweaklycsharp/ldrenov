# Site Couvreur - Déploiement Vercel

Site vitrine moderne pour couvreur spécialisé en petits travaux de toiture (Morbihan/Finistère).

## 🚀 Déploiement sur Vercel

### 1. Créer un compte Formspree (gratuit)

1. Aller sur [formspree.io](https://formspree.io/)
2. Créer un compte gratuit
3. Créer un nouveau formulaire
4. Copier l'ID du formulaire (format: `xxxxxxxxxxx`)

### 2. Configurer le formulaire

Dans le fichier `index.html`, ligne 1031, remplacer :
```html
<form id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Par :
```html
<form id="contactForm" action="https://formspree.io/f/VOTRE_ID_ICI" method="POST">
```

### 3. Personnaliser le site

Remplacer `[VOTRE NOM]` par le nom du couvreur (3 occurrences) :
- Ligne 283 : Logo header
- Ligne 332 : Hero section  
- Ligne 1045 : Footer

### 4. Déployer sur Vercel

#### Option A : Via GitHub (recommandé)

1. Créer un repository GitHub
2. Pusher les fichiers (index.html + vercel.json)
3. Aller sur [vercel.com](https://vercel.com/)
4. Cliquer sur "New Project"
5. Importer le repository GitHub
6. Déployer (automatique)

#### Option B : Via Vercel CLI

```bash
# Installer Vercel CLI
npm i -g vercel

# Se connecter
vercel login

# Déployer
vercel
```

#### Option C : Glisser-déposer

1. Aller sur [vercel.com](https://vercel.com/)
2. Cliquer sur "New Project"
3. Sélectionner "Deploy from template" ou uploader les fichiers

## 📁 Structure des fichiers

```
.
├── index.html       # Site complet
├── vercel.json      # Configuration Vercel
└── README.md        # Ce fichier
```

## ✨ Fonctionnalités

- ✅ Design moderne et responsive
- ✅ Formulaire de contact avec Formspree
- ✅ Galerie photos
- ✅ Section services
- ✅ Zone d'intervention
- ✅ Animations fluides
- ✅ Optimisé SEO

## 📧 Configuration email

Les emails du formulaire seront envoyés à : **louis.dumoulin56@gmail.com**

Pour changer l'email de réception :
1. Aller dans les paramètres Formspree
2. Modifier l'email de notification

## 🎨 Personnalisation

Les couleurs principales sont définies dans les variables CSS (ligne 12-20) :
- `--primary: #FF4D00` (Orange)
- `--secondary: #00F5FF` (Cyan)
- `--accent: #FFD700` (Or)

## 📱 Contact

- **Téléphone** : 07 83 93 21 20
- **Email** : louis.dumoulin56@gmail.com
- **Adresse** : 2 rue Claudie Haigneré, 56700 Hennebont

## 🔧 Support

Pour toute question sur le déploiement, consulter la [documentation Vercel](https://vercel.com/docs).
