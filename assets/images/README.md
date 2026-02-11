# Images du Portfolio

Ce dossier contient les images utilisées dans le portfolio.

## 📸 Images requises

### Images principales
- `profile.jpg` - Photo de profil pour la page d'accueil (200x200px recommandé, format carré)
- `about-photo.jpg` - Photo professionnelle pour la page À propos (optionnel)
- `favicon-32x32.png` - Favicon du site 32x32px
- `favicon-16x16.png` - Favicon du site 16x16px

### Images de projets
Créez un sous-dossier `projects/` pour les captures d'écran de vos projets :
- `ecommerce.jpg` - Capture du projet e-commerce
- `dashboard.jpg` - Capture du projet dashboard
- `api.jpg` - Capture du projet API
- etc.

## 🎨 Recommandations

### Format
- **Photos** : JPEG (.jpg) pour les photos
- **Graphiques/Screenshots** : PNG (.png) pour les captures d'écran
- **Icons** : SVG pour les icônes (intégrés directement dans le HTML)

### Taille
- Compressez vos images pour de meilleures performances
- Utilisez des outils comme [TinyPNG](https://tinypng.com/) ou [Squoosh](https://squoosh.app/)
- Photo de profil : max 200KB
- Screenshots de projets : max 500KB chacun

### Dimensions recommandées
- Photo de profil : 200x200px (carré)
- Photo À propos : 250-400px de largeur
- Screenshots projets : 1200px de largeur max

### Accessibilité
- Assurez-vous que vos images ont un bon contraste
- Les textes sur images doivent être lisibles
- Toujours ajouter un attribut `alt` descriptif dans votre HTML/Markdown

## 📝 Droits d'auteur

Assurez-vous que toutes les images que vous utilisez sont :
- Vos propres photos/créations
- Libres de droits
- Ou correctement créditées si provenant de sources externes

## 🔗 Sources d'images libres de droits

Si vous avez besoin de placeholder ou d'images temporaires :
- [Unsplash](https://unsplash.com/) - Photos haute qualité
- [Pexels](https://www.pexels.com/) - Photos et vidéos gratuites
- [Pixabay](https://pixabay.com/) - Images et illustrations
- [UI Faces](https://www.uifaces.co/) - Avatars pour prototypes

## 📦 Structure suggérée

```
images/
├── profile.jpg               # Photo de profil
├── about-photo.jpg          # Photo page À propos
├── favicon-32x32.png        # Favicon 32x32
├── favicon-16x16.png        # Favicon 16x16
└── projects/                # Screenshots de projets
    ├── ecommerce.jpg
    ├── dashboard.jpg
    ├── api.jpg
    └── autre-projet.jpg
```

## ⚠️ Note importante

Les images ne sont **pas incluses** dans ce template pour des raisons de taille de fichier et de personnalisation. Vous devez ajouter vos propres images avant de déployer votre portfolio.

En attendant, les pages utilisent des placeholders qui seront automatiquement masqués si les images ne sont pas trouvées (grâce à `onerror="this.style.display='none'"` dans le code).
