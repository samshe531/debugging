#  Bug Report – Conflit d'identifiants (`id`) et erreur de lien dans les données de films

##  1. Bug détecté : Identifiants (`id`) dupliqués

Un **conflit d'identifiants** a été détecté lors du rendu d'une liste de films avec `.map()` dans React.

###  Données concernées :
```js
{
  id: 2,
  title: "Her",
  ...
},
{
  id: 2, //  Identifiant dupliqué
  title: "The Lobster",
  ...
}
React exige que chaque élément enfant dans une liste ait une key unique. Ce doublon (id: 2) a provoqué un comportement incohérent dans le DOM virtuel.


React Developer Tools est un outil précieux pour inspecter les composants React, mais il ne détecte pas tous les types de bugs.



