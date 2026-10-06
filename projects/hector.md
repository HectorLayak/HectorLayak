# HECTOR

**Décrire le besoin. Construire la mécanique.**

[Tous les projets](../README.md#tout-latelier) · [English](hector.en.md)

HECTOR part d’une idée : l’auteur doit pouvoir exprimer le comportement attendu, ses contraintes et les transformations autorisées. Types, unités, effets et contrats donnent une forme explicite à cette intention. Le langage vise aussi les agents : leurs propositions deviennent examinables par le compilateur.

Le projet réunit un langage, un compilateur natif écrit en Hector et des bibliothèques consommables en natif ou en WebAssembly. Collections, registres et calculs constituent des applications concrètes. Une même règle de recherche peut, par exemple, conduire à un parcours ou à un index selon les libertés déclarées et le profil de charge.

L’ambition est de comparer plusieurs réalisations d’un même comportement selon le temps, la mémoire ou la simplicité. Le compilateur et ses contrats existent ; la recherche sur l’équivalence comportementale et le choix des réalisations continue.

## Parcours

1. Décrire les données, le comportement et ses contraintes.
2. Déclarer les transformations admissibles.
3. Examiner types, effets et contrats avec le compilateur natif.
4. Intégrer et mesurer le noyau compilé dans son application.

## Décisions de conception

### Le comportement avant la mécanique

Déclarer les valeurs, les résultats et les obligations. L’auteur précise aussi les libertés : représentation, fusion ou ordre indépendant.

### Un langage pour humains et agents

Les types, effets et contrats rendent les propositions analysables. L’agent propose un changement ; le compilateur expose les contradictions qu’il sait détecter.

### Un noyau réutilisable

Les mêmes sources produisent des bibliothèques natives et WebAssembly. Les interfaces et les identités de compilation accompagnent leur intégration dans les applications.

**État :** Recherche appliquée · compilateur natif et noyaux WebAssembly.

[Studio & services ↗](https://floriansola.fr/projects/hector)
