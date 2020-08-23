<!-- omit in toc -->
# CSS Advanced

Voyons ensemble encore quelques techniques qui nous seront utiles en CSS.

- [Variables ou custom properties](#variables-ou-custom-properties)
- [Import](#import)
- [Contexte de Formatage de Blocs](#contexte-de-formatage-de-blocs)

## Variables ou custom properties

Depuis CSS3 il est possible de créer des variables. Il s'agit d'informations que vous voulez réutilisez dans toutes votre feuille de style. Vous pouvez stocker des couleurs, des polices ou n'importe quelle autre propriété CSS.

Un des avantages des variables est la lisibilité. En effet il sera plus facile de lire `primary-color`que le code hexadécimal de cette couleur `#FF4000`. 

Un autre avantage, évident, c'est la facilité d'éffectuer des modifications sur l'ensemble de sa feuille de style. Il ne faut en effet modifier qu'une fois la valeur de sa variable et le changement se ferra partout où vous avez indiqué cette variable.

<!-- omit in toc -->
### Utilisation simple

On déclare une variable en indiquant deux tirets devant son nom. Ensuite il faut utiliser la valeur `var(nom-de-variable)`.

```css
:root {
  --main-bg-color: red;
}
element {
  background-color: var(--main-bg-color);
}
```

[:book:En savoir plus](https://developer.mozilla.org/fr/docs/Web/CSS/Using_CSS_custom_properties)

[:arrow_up:Revenir au top](#CSS-advanced)

## Import

Vous commencez sans doute à avoir une feuille de style à rallonge et vous ne vous y retrouvez plus? Et bien la solution réside dans les `import`. En effet la règle `@import`permet d'inclure une feuille de style dans une autre. Ainsi vous pouvez diviser votre travail en plusieurs feuilles en fonction des différentes sections que vous devez styliser.

Il est également possible d'utiliser les mediaqueries pour utiliser une feuille de style particulière si la règle est respectée.

**Exemple**: main.css, header.css, footer.css, nav.css, card.css, print.css...

<!-- omit in toc -->
### Utilisation

Il suffit de placer **au dessus de toute autre règle/sélecteur** votre `@import`, lui indiquer la feuille qu'il doit importer et préciser éventuellement les règles qu'il doit respecter pour utiliser cette feuille de style.

```css
@import "header.css";
@import url("nav.css");
@import "printstyle.css" print; /* use it only on print */
@import "mobile.css" screen and {max-width: 768px}; /* use it only if media is screen and viewport is max 768px */
```

[:arrow_up:Revenir au top](#CSS-advanced)

## Contexte de Formatage de Blocs

> Un contexte de formatage de blocs (block formatting context) est une partie du rendu visuel par le CSS, d'une page web. C'est la région qui délimite la mise en page des blocs et dans laquelle les éléments flottant interagissent les uns avec les autres.
>
> *- MDN Web Docs*

En d'autre termes, il s'agit de définir comments les éléments interagissent entre eux. Quand on a une élément en `float`, l'élément qui vient se placer à côté de lui se place aussi en dessous de celui-ci car il fait partie du même contexte, du même environnement. Si vous voulez "casser" cela, il faut par exemple utiliser une propriété telle que `overflow:hidden`. Consultez l'exemple suivante pour mieux comprendre ce dont je vous parles:

[Un exemple](https://codepen.io/scalajeremy/pen/ExKNwZp) vaut plus qu'une longue théorie.

> :book: Plus d'infos: [MDN :us:](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context) | [MDN :fr:](https://developer.mozilla.org/fr/docs/Web/CSS/Block_formatting_context) | [Video :us:](https://youtu.be/h3XH3yTWiK8)
>
> [:video_camera: Une vidéo](https://youtu.be/x_i2gga-sYg) qui reprend le principe du contexte de formatage des blocs en parlant des inline, block et inline-block 

[:arrow_up:Revenir au top](#CSS-advanced)
