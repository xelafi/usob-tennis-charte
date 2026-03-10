# 📘 Guide d'Utilisation - Charte Graphique U.S.O.Bezons Tennis

## 🎨 Utilisation des Couleurs

### Couleur Principale - Bleu Foncé (#0D2B5B)

**✅ À UTILISER POUR :**
- Logo principal
- En-têtes et headers
- Fonds principaux
- Titres importants
- Maillots et textiles officiels
- Éléments de navigation principaux

**❌ À ÉVITER :**
- Texte sur fond sombre
- Petits éléments (manque de lisibilité)
- Fonds de formulaires

**Exemple d'utilisation :**
```css
.header {
    background: var(--color-primary);
    color: var(--color-neutral);
}
```

### Couleur Secondaire - Bleu Clair (#3366B8)

**✅ À UTILISER POUR :**
- Boutons secondaires
- Liens cliquables
- Pictogrammes et icônes
- Éléments graphiques décoratifs
- Dégradés avec le bleu foncé
- Hover states

**❌ À ÉVITER :**
- Texte de paragraphe
- Fonds étendus (trop présent)

**Exemple d'utilisation :**
```css
.btn-secondary {
    background: var(--color-secondary);
    color: var(--color-neutral);
}

.btn-secondary:hover {
    background: var(--color-secondary-dark);
}
```

### Couleur Accent - Jaune Tennis (#FEE02E)

**✅ À UTILISER POUR :**
- Boutons d'action principale (CTA)
- Rappel de la balle de tennis
- Mise en avant d'informations importantes
- Détails du logo
- Highlights et surlignages
- Éléments interactifs

**❌ À ÉVITER :**
- Texte sur fond blanc (utiliser #E6C200)
- Fonds étendus
- Trop présent (perd son impact)

**Exemple d'utilisation :**
```css
/* Pour fond */
.highlight {
    background: var(--color-accent);
    color: var(--color-primary);
}

/* Pour texte sur fond clair */
.text-accent {
    color: var(--color-accent-dark); /* Meilleur contraste */
}
```

### Couleur Neutre - Blanc (#FFFFFF)

**✅ À UTILISER POUR :**
- Texte sur fond bleu
- Respirations visuelles
- Fonds de cartes
- Espaces entre sections

---

## ✍️ Utilisation de la Typographie

### Montserrat Bold - Police de Titres

**✅ À UTILISER POUR :**
```css
/* Nom du club */
.club-name {
    font-family: var(--font-title);
    font-weight: var(--font-weight-bold);
    font-size: var(--font-size-h1);
    text-transform: uppercase;
    letter-spacing: 2px;
}

/* Titres de sections */
h2 {
    font-family: var(--font-title);
    font-size: var(--font-size-h2);
}

/* Affiches et visuels */
.poster-title {
    font-family: var(--font-title);
    font-weight: var(--font-weight-bold);
}
```

**❌ À ÉVITER :**
- Textes longs (difficile à lire)
- Corps de texte
- Texte en minuscules (perd son impact)

### Open Sans - Police de Texte

**✅ À UTILISER POUR :**
```css
/* Texte courant */
p, body {
    font-family: var(--font-text);
    font-size: var(--font-size-body);
    line-height: 1.6;
}

/* Navigation */
.nav-link {
    font-family: var(--font-text);
    font-weight: var(--font-weight-medium);
}

/* Formulaires */
input, textarea {
    font-family: var(--font-text);
}
```

---

## 📏 Système d'Espacement

### Règles générales

```css
/* Espacement interne des cartes */
.card {
    padding: var(--space-lg); /* 32px */
}

/* Marges entre sections */
section + section {
    margin-top: var(--space-3xl); /* 96px */
}

/* Espacement des éléments de liste */
.list-item {
    margin-bottom: var(--space-md); /* 24px */
}

/* Petit espacement (éléments liés) */
.form-label {
    margin-bottom: var(--space-xs); /* 8px */
}
```

### Guide d'utilisation

| Taille | Valeur | Usage recommandé |
|--------|--------|------------------|
| XS | 8px | Entre étiquette et champ, petits gaps |
| SM | 16px | Entre paragraphes, petites marges |
| MD | 24px | Entre groupes d'éléments |
| LG | 32px | Padding de cartes, entre blocs |
| XL | 48px | Entre sections liées |
| 2XL | 64px | Entre grandes sections |
| 3XL | 96px | Entre sections majeures |

---

## 🎯 Boutons

### Bouton Principal
```html
<button class="btn btn-primary">Inscription</button>
```
```css
.btn-primary {
    background: var(--color-primary);
    color: var(--color-neutral);
    padding: 18px 50px;
    border-radius: var(--radius-xl);
    font-family: var(--font-title);
    font-size: 1.2em;
    text-transform: uppercase;
    letter-spacing: 2px;
    box-shadow: var(--shadow-md);
}
```

### Bouton Accent (Call-to-Action)
```html
<button class="btn btn-accent">Réserver un court</button>
```
```css
.btn-accent {
    background: var(--color-accent);
    color: var(--color-primary);
    /* Même style que btn-primary */
}
```

### Tailles minimales
- **Desktop** : 44×44px minimum
- **Mobile** : 48×48px minimum (zones tactiles)

---

## ♿ Règles d'Accessibilité

### Contraste de Couleurs

#### ✅ CONFORMES WCAG AA

| Combinaison | Ratio | Usage |
|-------------|-------|-------|
| Bleu foncé + Blanc | 12.6:1 | ✅ Parfait pour texte |
| Bleu clair + Blanc | 4.8:1 | ✅ OK pour titres (> 18px) |
| Jaune foncé + Blanc | 4.5:1 | ✅ OK pour texte |

#### ❌ NON CONFORMES

| Combinaison | Problème |
|-------------|----------|
| Jaune clair (#FEE02E) + Blanc | Ratio insuffisant |
| Bleu clair + Bleu foncé | Trop faible pour petit texte |

**Solution :** Utiliser `var(--color-accent-dark)` pour texte jaune sur fond clair

### Tailles de Texte

```css
/* ✅ Tailles minimales recommandées */
body { font-size: 16px; } /* Minimum absolu */
p { font-size: 18px; }    /* Recommandé pour confort */
h3 { font-size: 24px; }   /* Minimum pour titres */

/* ❌ À éviter */
.small-text { font-size: 12px; } /* Trop petit */
```

---

## 📱 Applications Pratiques

### Site Web

```css
/* Header */
.site-header {
    background: var(--color-primary);
    padding: var(--space-lg) var(--space-2xl);
}

/* Navigation */
.nav-link {
    color: var(--color-neutral);
    font-family: var(--font-title);
    padding: var(--space-sm);
}

.nav-link:hover {
    color: var(--color-accent);
}

/* Section principale */
.hero-section {
    background: linear-gradient(135deg, 
                var(--color-primary) 0%, 
                var(--color-secondary) 100%);
    padding: var(--space-3xl) var(--space-2xl);
}

/* Cartes */
.card {
    background: var(--color-neutral);
    padding: var(--space-lg);
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-md);
    border-left: 4px solid var(--color-accent);
}
```

### Réseaux Sociaux

**Format : 1080×1080px (Instagram) ou 1200×630px (Facebook)**

```css
.social-post {
    background: var(--color-primary);
    /* Logo en haut à gauche */
    /* Titre en Montserrat Bold */
    /* Accent jaune pour élément clé */
    /* Balle de tennis stylisée en décoration */
}
```

### Affiches / Flyers

**Hiérarchie visuelle :**
1. Titre principal : Montserrat Bold, 72pt+, Blanc
2. Sous-titre : Montserrat Bold, 36pt, Jaune
3. Informations : Open Sans, 18-24pt, Blanc
4. Call-to-action : Bouton jaune avec texte bleu foncé

---

## 🚫 Erreurs à Éviter

### ❌ Ne JAMAIS faire

1. **Déformer le logo** (étirer, comprimer)
2. **Changer les couleurs** sans respecter la charte
3. **Utiliser d'autres polices** que celles définies
4. **Texte jaune clair sur blanc** (mauvais contraste)
5. **Espacements aléatoires** (toujours multiples de 8px)
6. **Trop de couleurs accent** (le jaune perd son impact)
7. **Texte trop petit** (< 16px)

### ✅ Bonnes Pratiques

1. **Préserver les espaces** autour du logo (minimum = hauteur du logo)
2. **Utiliser le système d'espacement** (multiples de 8px)
3. **Vérifier les contrastes** avant publication
4. **Tester sur mobile** (lisibilité et zones tactiles)
5. **Rester cohérent** avec les exemples fournis
6. **Privilégier la simplicité** (moins c'est plus)

---

## 📞 Questions ?

Pour toute question sur l'utilisation de la charte graphique, référez-vous :
- À la présentation complète (index.html)
- Au fichier README.md
- Aux exemples dans ce document

**U.S.O.Bezons Tennis** - Respectons notre identité visuelle ! 🎾
