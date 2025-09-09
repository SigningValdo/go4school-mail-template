# Go4School - Template Email

<div align="center">
  <h3>📧 Template d'emails transactionnels pour Go4School</h3>
  <p>L'école connectée entre vos mains</p>
</div>

## 📋 Description du projet

Ce projet contient un template d'email transactionnel pour l'application Go4School, développé avec le framework Maizzle et Tailwind CSS. Il permet de créer des emails HTML responsives et compatibles avec tous les clients de messagerie.

## 🏗️ Structure du projet

```
go4school-template/
├── components/           # Composants réutilisables
│   ├── button.html      # Composant bouton personnalisé
│   ├── divider.html     # Composant séparateur
│   ├── spacer.html      # Composant espacement
│   └── v-fill.html      # Composant de remplissage vertical
├── emails/              # Templates d'emails
│   └── transactional.html  # Template principal
├── images/              # Assets visuels
│   ├── logo.png         # Logo Go4School
│   ├── app.png          # Image de l'application
│   ├── appstore.svg     # Badge App Store
│   ├── playstore.svg    # Badge Google Play
│   └── *.svg            # Icônes réseaux sociaux
├── layouts/             # Layouts de base
│   └── main.html        # Layout principal
├── config.js            # Configuration de développement
├── config.production.js # Configuration de production
└── package.json         # Dépendances et scripts
```

## 🚀 Installation et exécution

### Prérequis

- Node.js (version 14 ou supérieure)
- npm ou yarn

### Installation des dépendances

```bash
npm install
```

### Commandes disponibles

#### Développement

```bash
npm run dev
```

Lance le serveur de développement Maizzle avec rechargement automatique. L'email sera accessible à l'adresse `http://localhost:3000`.

#### Production

```bash
npm run build
```

Compile et optimise l'email pour la production. Les fichiers finaux sont générés dans le dossier `build_production/`.

## 🎨 Personnalisation

### Modifier le contenu de l'email

Le contenu principal se trouve dans `emails/transactional.html`. Vous pouvez :

- Modifier les textes directement dans le fichier
- Ajuster les couleurs via les classes Tailwind CSS
- Personnaliser les liens et boutons

### Ajouter des composants

Les composants réutilisables sont dans le dossier `components/`. Chaque composant peut être utilisé avec des props personnalisables.

Exemple d'utilisation :

```html
<x-button href="https://example.com" class="bg-blue-500 text-white">
  Mon bouton
</x-button>
```

### Modifier les images

1. Ajoutez vos images dans le dossier `images/`
2. Mettez à jour les références dans `emails/transactional.html`
3. Les images sont automatiquement optimisées lors du build

## 🛠️ Configuration

### Configuration de développement (`config.js`)

- Définit les paramètres de base pour le développement
- Configure le contenu à traiter et les assets statiques

### Configuration de production (`config.production.js`)

- Optimise l'email pour la production
- Minifie le CSS et le HTML
- Inline les styles pour une meilleure compatibilité

## 📱 Fonctionnalités

- ✅ **Responsive** : S'adapte à tous les écrans
- ✅ **Compatible** : Fonctionne sur tous les clients email
- ✅ **Composants** : Système de composants réutilisables
- ✅ **Tailwind CSS** : Styling moderne et maintenable
- ✅ **Optimisé** : Images et CSS optimisés pour la production

## 🎯 Utilisation

1. **Développement** : Utilisez `npm run dev` pour voir vos modifications en temps réel
2. **Personnalisation** : Modifiez le contenu dans `emails/transactional.html`
3. **Build** : Exécutez `npm run build` pour générer la version finale
4. **Déploiement** : Utilisez les fichiers du dossier `build_production/`

## 📞 Support

Pour toute question ou problème :

- Email : hello@go4school.net
- Téléphone : +237 696 271 223 / +33 753952024
- Site web : www.go4school.net

## 📄 Licence

Ce projet utilise le framework Maizzle sous licence MIT.
