### Q & A

<br>
<br>

**1. how to find a limit, breaking up the logic, the code in order to simplify things?...**
=> it depends of the context! 
First the confort level as programmer but also
Working on a team it seems to be important to try to figuring out where the level of the abstraction is!...

**2. about reducing coupling code & logic as much as possible...**
=> it needs to move code in a way to increase cohesion (functional, feature..)

**3. about testing the specifics methods and the air traffic control methods?**
=> both needs to be tested on two different ways to improve the code coverage

**4. Does that make sense to each instance of service, in a case of multiples services's application, and then making them available via dependency injection?**
=> it seems to be a good thougth in this case.
Overriding injectors may be the case writing tests only.

<br>
<br>

**5.** Asking ourselves about, **if there's any reason we would need more than one instance of this thing to perform this function within the application?**

*There maybe are some particular cases which we potentially need it!? But it will be really rare to have more than one instance! And it will be recommended to keep it at the top level of the application and then make it available via dependency injection*

<br>
<br>

#### how to identify:

**what is the shared commonality or functionality that all the different components or parts that they need, and then placing that concerned part of the application at the level of the abstraction just above.**

<br>

### Quotes

- **About Cohesion:**
  
>"il n'y aurait pas de sens à ranger tout ses vêtements dans le même tiroir.
>de même qu'on peut tojours mieux faire et que si on range chaque type de 
>vêtements dans son propre tiroir, on pourrait tout à fait commencer à réfléchir 
>comment ranger ses pantalons ou bien ses Tee-shirts!!!?

>Ainsi, il y aurai une réflexion à mené autour de cette organisation afin
>de pouvoir s'y retrouver en toute situations, à tout moment...
>On y gagne en terme de "Cohésion"

>"Ranger ses livres par couleur n'a pas de sens autre que visuel. 
>Il déjà serait clairement évident, de réfléchir à
>les ranger par Thématique!! 
>C'est niveau approprié de cohésion.
>On prend du temps à le mettre en place mais on en gagne par la suite
>quand on en a besoin.
>
>Le "visuel" peux entrer en jeu, 
>mais il reste secondaire pour cette problématique."

- **About Organization & Mental Complexity:**
  
>"La question n'est pas d'attribuer un endroit pour chaque item!! 
>Ca n'a pas de sens, il s'agit de raisonner le problème et d'y 
>mettre en place une organisation cohérente pour réduire cette 
>forme de compléxité mentale."


>"Imagines une salle de réunion ou tu dois accueuillir tout les clients, 
>sous-traitants, collègues...
>On ne veut pas partager la même réunion dans la même salle avec les mêmes
>personnes!!!
>D'une réflexion sur la question de modéliser les choses, il arrive forcément 
>le moment ou en ressort le besoin de découper les choses, de les séparer.
>
>Mais si alors un seul principal service doit prendre en main ce problème,
>il parait logique qu'il n'y a pas besoin de duppliquer les choses"

>"Pour une Application avec 2 composants, cela peut être placé au niveau de 
>l'application.
>S'il ya deux applications séparées, il devrait être placé dans un dossier 
>`lib/` qu'il puisse être partagé à traves les applications.
>S'il y a plus d'un projet qui aurait besoin de cette fonctionnalité. 
>Il serait bon de penser à le publier peut être sur NPM
>
>Il s'agit de toujours le placer un niveau au dessus.

### Extracting methods

When comes the moment to extract a method from a class component, 
it's maybe a great thing to think if it can replace the `this.` by a 
parameter on this method extracted!!!

It's making a opportunity to switch that functionality inna pure function!