# 🎾 U.S.O.Bezons Tennis - Charte Graphique

Présentation Reveal.js de la charte graphique du club U.S.O.Bezons Tennis.

## 📋 Contenu de la présentation

### 1. **Couleurs principales** 🎨
- **Bleu foncé** (#0D2B5B) - Couleur principale du club
- **Bleu clair** (#3366B8) - Couleur secondaire
- **Jaune tennis** (#FEE02E) - Couleur accent (rappel de la balle)
- **Blanc** (#FFFFFF) - Couleur neutre

### 2. **Couleurs enrichies** ✨
- **Variations de luminosité** pour chaque couleur principale (light/dark)
- **Couleurs tertiaires** : Gris anthracite (#4A5568) pour textes secondaires
- **Couleurs d'état** : Succès, Erreur, Avertissement, Info

### 3. **Typographies**
- **Titres** : Montserrat Bold / Bebas Neue
- **Texte** : Open Sans / Roboto
- **Hiérarchie définie** : H1 (56px), H2 (40px), H3 (28px), Body (19px)
- **Graisses** : Regular 400, Medium 500, Bold 700

### 4. **Système d'espacement** 📏
Basé sur des multiples de 8px pour une cohérence parfaite :
- XS: 8px, SM: 16px, MD: 24px, LG: 32px, XL: 48px, 2XL: 64px, 3XL: 96px

### 5. **Accessibilité** ♿
- Conformité WCAG AA
- Ratios de contraste validés
- Tailles minimales définies

### 6. **Style graphique**
- Éléments visuels : balle de tennis, lignes de court, motifs dynamiques
- Style : moderne, dynamique, sport club

## 🚀 Installation et utilisation

### Visualiser la présentation Reveal.js

1. Ouvrez le fichier `index.html` dans votre navigateur
2. Utilisez les touches fléchées ou cliquez sur les flèches pour naviguer

### Voir les exemples de composants

Ouvrez `exemples.html` pour voir tous les composants en action :
- Boutons (toutes tailles et styles)
- Cartes et containers
- Formulaires
- Badges et alertes
- Navigation et footer
- Éléments décoratifs

### Consulter la documentation

- **README.md** : Vue d'ensemble et démarrage rapide
- **GUIDELINES.md** : Guide détaillé d'utilisation de la charte
- **css/components.css** : Tous les snippets CSS réutilisables

### Servir localement (optionnel)

Si vous préférez utiliser un serveur local :

```powershell
# Avec Python
python -m http.server 8000

# Avec Node.js (http-server)
npx http-server

# Avec PHP
php -S localhost:8000
```

Puis ouvrez `http://localhost:8000` dans votre navigateur.

## 🎮 Navigation

- **← →** : Naviguer entre les slides
- **Espace** : Slide suivante
- **Échap** : Vue d'ensemble des slides
- **F** : Mode plein écran
- **S** : Mode présentateur avec notes

## 📁 Structure du projet

```
USOB Tennis/
│
├── index.html              # Présentation Reveal.js principale
├── exemples.html           # Page d'exemples de composants
├── css/
│   ├── theme.css          # Styles de la charte graphique
│   └── components.css     # Composants réutilisables
├── README.md              # Documentation principale
└── GUIDELINES.md          # Guide d'utilisation détaillé
```

## 🎨 Utilisation de la charte graphique

### Variables CSS disponibles

#### Couleurs principales
```css
--color-primary: #0D2B5B;          /* Bleu foncé */
--color-primary-light: #1a4080;
--color-primary-dark: #081b3a;

--color-secondary: #3366B8;        /* Bleu clair */
--color-secondary-light: #5c8ad4;
--color-secondary-dark: #2952a3;

--color-accent: #FEE02E;           /* Jaune tennis */
--color-accent-dark: #E6C200;      /* Meilleur contraste */
--color-accent-light: #FFF176;

--color-neutral: #FFFFFF;          /* Blanc */
--color-neutral-light: #F8F9FA;
--color-neutral-dark: #E9ECEF;
```

#### Couleurs tertiaires & d'état
```css
--color-gray: #4A5568;             /* Gris anthracite */
--color-gray-light: #718096;
--color-gray-dark: #2D3748;

--color-success: #10B981;          /* Vert succès */
--color-error: #EF4444;            /* Rouge erreur */
--color-warning: #F59E0B;          /* Orange avertissement */
--color-info: #3366B8;             /* Bleu information */
```

#### Typographie
```css
--font-title: 'Montserrat', sans-serif;
--font-text: 'Open Sans', sans-serif;

--font-size-h1: 3.5em;             /* 56px */
--font-size-h2: 2.5em;             /* 40px */
--font-size-h3: 1.75em;            /* 28px */
--font-size-body: 1.2em;           /* 19px */

--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-bold: 700;
```

#### Espacement
```css
--space-xs: 8px;
--space-sm: 16px;
--space-md: 24px;
--space-lg: 32px;
--space-xl: 48px;
--space-2xl: 64px;
--space-3xl: 96px;
```

#### Bordures & Ombres
```css
--radius-sm: 5px;
--radius-md: 10px;
--radius-lg: 15px;
--radius-xl: 50px;

--shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.1);
--shadow-md: 0 4px 15px rgba(0, 0, 0, 0.15);
--shadow-lg: 0 6px 20px rgba(0, 0, 0, 0.25);
```

### Classes de boutons

```html
<button class="btn btn-primary">Bouton Principal</button>
<button class="btn btn-secondary">Bouton Secondaire</button>
<button class="btn btn-accent">Action Importante</button>
<button class="btn btn-outline">Bouton Outline</button>
```

## 📱 Applications de la charte

- **Digital** : Site web, réseaux sociaux, newsletter
- **Textile** : Maillots, vêtements, accessoires
- **Print** : Affiches, flyers, documents
- **Événements** : Banderoles, signalétique, trophées

## 🛠️ Personnalisation

Pour modifier les couleurs ou les styles, éditez le fichier `css/theme.css`.

Les polices sont chargées depuis Google Fonts et sont déjà intégrées dans le fichier HTML.

## 📖 Documentation Reveal.js

Pour plus d'options de personnalisation, consultez la [documentation officielle de Reveal.js](https://revealjs.com/).

## 🎯 Points clés de la charte

- **Identité forte** : Couleurs franches et reconnaissables
- **Modernité** : Design épuré et contemporain
- **Dynamisme** : Éléments graphiques sportifs
- **Cohérence** : Application uniforme sur tous les supports

## ✨ Améliorations de la charte

### Système de couleurs enrichi
- ✅ Variations de luminosité (light/dark) pour chaque couleur
- ✅ Couleurs tertiaires (gris anthracite) pour plus de nuances
- ✅ Couleurs d'état (succès, erreur, avertissement) pour les interfaces

### Hiérarchie typographique claire
- ✅ Tailles définies pour tous les niveaux (H1, H2, H3, body)
- ✅ Graisses standardisées (Regular, Medium, Bold)
- ✅ Line-height optimisés pour la lisibilité

### Système d'espacement cohérent
- ✅ Basé sur des multiples de 8px
- ✅ 7 niveaux d'espacement (XS à 3XL)
- ✅ Facilite l'alignement et la cohérence visuelle

### Accessibilité WCAG AA
- ✅ Ratios de contraste validés
- ✅ Jaune foncé (#E6C200) pour texte sur fond clair
- ✅ Tailles minimales définies
- ✅ Zones de clic optimisées

### Design System complet
- ✅ Variables CSS pour tous les éléments
- ✅ Bordures et ombres standardisées
- ✅ Système responsive intégré
- ✅ Documentation complète

---

**U.S.O.Bezons Tennis** - Une identité forte pour un club d'exception
