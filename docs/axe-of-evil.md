<div align="center">

  <img src="assets/the-axe-of-evil.png" alt="the-axe-of-evil-pic">

</div>

<br>
<br>
<br>
<br>

## Se poser les bonnes questions

<img src="assets/know-this-code.png" alt="can-I-know-this-code">

<img src="assets/reuse-this-code.png" alt="can-I-reuse-this-code">

<img src="assets/test-this-code.png" alt="can-I-test-this-code">

## Les 3 classiques causes de conflit

<img src="assets/the-3-classics-issues.png" alt="can-I-test-this-code">

*Imaginons un programme implémenté de façon assez complexe avec un test coverage médiocre, nous imaginons également que tout fonctionne, qu'il n'y aurait donc pas de souci à se faire. Cependant, si nous supposons que dans 95% des cas d'utilisations de ce programmes tout fonctionnerai à merveille, cela ne veut surtout pas dire que sur une exception, le programme ne puisse pas casser. 
Les principales causes dans cette situation est qu'un programme se doit d'adapter certaines pratiques...*

<br>

#### Hidden State

Une structure de controle imbriquée gérant différents "états", différents cas de figure ou bien l'utilisation de méthode faisant "muter" les données et changer ce même état peut engendrer un disfonctionnement dans le programme.

**Suivre les bonnes pratiques ainsi que se fier aux méthodes de la programmation fonctionnelle** telles que `map()`, `filter()`, `reduce()` par exemple, doit être un objectif afin que le données ne mutent pas notemment.


<img src="assets/hidden-state.png" alt="block-code hidden state">

<br>
<br>

#### Violating the single responsability principle

Une des principes fondamentale de la méthode S.O.L.I.D entrant en résonnance avec le principe de "separate concerns", séparant le code de manière organisée, divisant le code en petits programmes ayant chacun qu'**une seule responsabilité**. 
Cela aura pour but d'éviter et de retirer tout type de conflit dans la logique du programme.

<img src="assets/srp.png" alt="block-code hidden state">

<br>
<br>

#### Nested Logic

Implémenter de **la logique de façon imbriquée, compléxifie le code et sa compréhension**.
Cela rend le code plus difficile à tester et augmente les chance que dans certains cas particulier, le code "casse". 
Dans certains cas de figure, des parties du programme peuvent entrer en conflit, il est alors tout à fait logique que de **séparer les block de code et simplifier les choses**.

<img src="assets/nested-logic.png" alt="block-code hidden state">

<br>
<br>

#### Quotes

<img src="assets/quote2.png" alt="quote about testing bad code">

<img src="assets/quote1.png" alt="quote about doing good practice in code">