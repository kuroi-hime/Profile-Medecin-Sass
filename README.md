# Profile-Medecin-Sass
Création d'une Page de Profil de Médecin en HTML et Sass

## Objectif du Projet

L’objectif de cet exercice est de recréer une page de profil de médecin inspirée du design fourni dont le but est de :
- Pratiquer la structuration d’une page de profil en HTML et Sass, avec une mise en page moderne.
- Se familiariser avec Flexbox et CSS Grid pour organiser le contenu de manière soignée et responsive.
- Appliquer des styles et effets visuels pour une présentation professionnelle.

## Mise en Page et Structure
Flexbox et Grid sont deux systèmes de mise en page CSS puissants : Flexbox gère les alignements en une seule dimension (ligne ou colonne), tandis que Grid permet des mises en page bidimensionnelles (lignes et colonnes).

### 🧱 Flexbox : Mise en page unidimensionnelle
Flexbox est idéal pour aligner les éléments dans une seule direction — soit horizontalement (ligne), soit verticalement (colonne).

#### 🔑 Concepts principaux
display: flex : active le mode Flexbox sur un conteneur. flex-direction : définit l’orientation (row, column, etc.). justify-content : aligne les éléments sur l’axe principal (ex. : center, space-between). align-items : aligne les éléments sur l’axe secondaire (ex. : stretch, center). flex-grow, flex-shrink, flex-basis : contrôlent la taille des éléments flexibles. order : change l’ordre visuel des éléments sans modifier le HTML.

#### ✅ Exemple d'utilisation dans le code
```CSS
footer {
    height: 10%;
    display: flex;/*choix d'affichage*/
    justify-content: center;/*centrer horizontalement*/
    align-items: end;/*pousser les éléments au dessous*/

    a {
        height: 70%;
        width: 100%;
        padding: 0 2%;

        button {
            height: 100%;
            width: 100%;
            border-radius: 10px;
            color: $secondary-color;
            background-color: $accent-color2;
        }
    }
}
```

### 🧮 Grid : Mise en page bidimensionnelle
Grid est conçu pour organiser les éléments en lignes et colonnes, parfait pour des mises en page complexes.

#### 🔑 Concepts principaux
display: grid : active le mode Grid sur un conteneur. grid-template-columns / grid-template-rows : définissent la structure du quadrillage. grid-gap ou gap : espace entre les lignes et colonnes. grid-column / grid-row : positionnent les éléments dans la grille. grid-area : nomme et place les zones de grille.

#### ✅ Exemple d'utilisation dans le code
```CSS
.statistiques {
                display: grid; /*choix d'affichage*/
                grid-template-columns: repeat(2, 1fr); /* diviser en deux colonnes*/
                justify-items: center; /*ajuster les éléments au centres*/
                height: fit-content;
                padding: 0 5%;
                row-gap: 5%;/*espace entre les lignes*/

                div {
                    /* du code ici */
                }
}
```