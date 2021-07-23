<div align="center">

  <img src="../assets/managing-complexity-hero.png" alt="managing-complexity-hero-pic">

</div>

<br>
<br>
<br>
<br>

## A propos de cette compléxité...

- gérer les états et la mécanique qui en découle
- analyser ces systèmes
- manipuler un volume de code 
- manipuler le flux de données de ces systèmes

<br> 

## Les 3 Points Clés

**Comment gérer la compléxité en développement & maintenance web de projets de logiciels à grande échelle?**
**Les grands projets de logiciles peuvent être difficile à comprendre!**

1. Gestion des **"States"**
1. Gestion de la **communication des "Data"**
1. Gestion du **volume de Code**

<br> 

           STATES MANAGEMENT 
                  / \   => abilité de faire passer & communiquer les données
                 /   \
                /     \
               /       \
              /         \
              ----------- 
       CONTROL FLOW       CODE VOLUME => gestion des "States", des données
            => implique l'abilité à gérer son code

<br> 

### Quelle "compléxité" ?

*Comment **raisonner un système selon un besoin d'entreprise** qui souvent est 
amené à grandir et se compléxifier.*

Faire ressortir de cette refléxion un sens très abstrait de notre métier, 
qui nous amènerait à prendre les bonnes décisions au bon moment ainsi qu'à
approcher les problématiques de la bonne manière selon la difficulté.

> Cette compléxité "mentale" comme une abilité mentale d'analyser ce qui se passe
> dans une application à grande échelle, d'analyser le système dès lors qu'il
> a vocation à grandir, de comprendre les enjeux des choix d'implémentation qui 
> sont devant nous...

## Compléxité & Routine

<img src="../assets/quote2.png" alt="quote about testing bad code">

<br> 


#### L'abilité à gérer cette compléxité

- **l'approche du "Code Legacy"**
- **la confrontation au "spaghetti code"**
- **l'assurance d'un code solide à 200%**
- **la compréhension d'un projet à grande échelle**
- **les principes clés de mise en pratique**
- **le micro, le mezzo & le macro**

#### Différentes problématiques du quotidien

1. un code même testé, d'apparence propre n'apporte t-il pas sa part de problème, ou bien sa propre compléxité a t-elle bien été prise en compte?
   => à quel point sommes nous sur qu'un code ne cassera pas?

1. le partage d'états "mutable" apporte une certaine dangerosité...
  => notion de "Separate Concerns" et SRP (Single Responsability Principle)
  => précautions sur l'implémentation de logiques imbriquées

1. gérer la compléxité sur différents niveaux de l'application
  => le composant, la librairie et l'application 

1. l'approche d'un code "sale", incompréhensible et / ou cassé
  => les limites du refactoring
  => le travail de prise en main du problème
  => comment et quand tester le code

<br> 

## Control Flow & Communication

**Comment communiquer un état en évènements selon son context et son propre niveau d'implémentation dans l'appication...**




### Communication des données
 
- des composants entre eux
- de l'injection de librairies
- au niveau globale de l'application

### Applications

- communication de/des aplications
- maintenir de la consistence dans le système
- rendre le data flow prévisible & cohérent
- séparer son code en de simples actions 
- limiter la taille de son code
- éviter la mutation de données par le choix de nos méthodes
- écrire du code réutilisable
  