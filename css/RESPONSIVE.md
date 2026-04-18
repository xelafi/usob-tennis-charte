# 📱 Guide Responsive - U.S.O.Bezons Tennis

## Breakpoints définis

### 🖥️ Desktop (> 1024px)
- Affichage par défaut
- Toutes les grilles en 2 ou 4 colonnes
- Tailles de police normales

### 💻 Tablette (≤ 1024px)
- `--font-size-h1: 3em`
- `--font-size-h2: 2em`
- Réduction des espacements
- Balle de tennis décorative réduite à 120px

### 📱 Mobile (≤ 768px)
- **Grilles en 1 colonne** (sauf couleurs tertiaires en 2 colonnes)
- `--font-size-h1: 2em`
- `--font-size-h2: 1.5em`
- `--font-size-body: 0.85em`
- Boutons ajustés
- Balle de tennis décorative à 80px
- Variations de couleurs avec wrap

### 📱 Petit Mobile (≤ 480px)
- `--font-size-h1: 1.75em`
- `--font-size-h2: 1.3em`
- `--font-size-body: 0.8em`
- Grille couleurs tertiaires en 1 colonne
- Balle de tennis décorative à 60px
- Boutons en largeur 90% (max 300px)
- Système d'espacement en colonne
- **Tous les espacements minimisés**

## Configuration Reveal.js

```javascript
width: 1920,
height: 1080,
margin: 0.1,
minScale: 0.1,  // Permet une réduction jusqu'à 10%
maxScale: 2.0,
touch: true     // Gestes tactiles activés
```

## Éléments adaptés

✅ Typographie (tous les niveaux)
✅ Grilles de couleurs
✅ Variations de couleurs
✅ Boutons
✅ Applications
✅ Hiérarchie typographique
✅ Système d'espacement
✅ Accessibilité
✅ Décorations (balles de tennis)
✅ Espacements (padding, margin, gap)
✅ Images (max-width: 100%, object-fit: contain)
✅ Overflow prevention (overflow: hidden)

## Correction du débordement mobile

### Problèmes résolus:
1. **Dimensions Reveal.js**: Utilisation de valeurs fixes (1920x1080) au lieu de pourcentages
2. **minScale réduit**: De 0.2 à 0.1 pour permettre plus de réduction
3. **Overflow**: `overflow: hidden` sur html, body et sections
4. **Box-sizing**: Appliqué globalement à tous les éléments
5. **Tailles de police réduites**: Sur mobile et petits mobiles
6. **Espacements minimisés**: Padding et gaps réduits sur mobile
7. **Images**: `max-width: 100%` et `object-fit: contain`

## Test

Pour tester le responsive :
1. Ouvrir `index.html` dans un navigateur
2. Ouvrir les DevTools (F12)
3. Activer le mode responsive (Ctrl+Shift+M / Cmd+Shift+M)
4. Tester aux breakpoints : 
   - 1920px (Desktop)
   - 1024px (Tablette)
   - 768px (Mobile)
   - 480px (Petit mobile)
   - 375px (iPhone SE)
   - 360px (Samsung Galaxy)

## Résolution des problèmes

Si les slides débordent encore:
- Vérifier que `minScale` est bien à 0.1
- Réduire `margin` dans Reveal.initialize() si nécessaire
- Utiliser les DevTools pour identifier les éléments qui débordent
- Ajuster les media queries en conséquence
