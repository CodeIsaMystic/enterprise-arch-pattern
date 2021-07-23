<div align="center">

  <img src="../assets/local-complexity.png" alt="local-complexity-hero-pic">

</div>

<br>
<br>

#  Les Niveaux de Compléxité [Micro-Mezzo-Macro]

***Réfléchir en terme de niveau de compléxité Micro/Mezzo/Macro***



### Le Niveau Local du code & de sa compléxité: MICRO

La compléxité locale du programme, **au niveau des composants**
- gérer les *"input & output"* au niveau du composant (dans une fonction, un objet...)

### Le Niveau Intermédiaire de compléxité: MEZZO

La communication **des composants & librairies dans l'application**:
- réfléchir en terme de composant ou des librairies injectées
- une sorte d' "intra-composant" communication 
- la possibilité de monter dans l'application

### Le Niveau Supérieur de compléxité: MACRO

La compléxité **au niveau de ou des application(s)**
- les applications ou au niveau de l'application.

<br>
<br>
<br>

## DEPENDENCY INJECTION & EXTRACT METHOD

<img src="../assets/dependency-injection.png" alt="dependency injection title">
<img src="../assets/extract-method.png" alt="extract method title">



**2 Options:**
- **Extraire une méthode et/ou bien un paramètre**
- **Injecter des dépendances**


#### Air Traffic Control ou Sequencing Methods

Des méthodes au niveau supérieur qui vont aider à la gestion des flux de données.
Généralement vont recevoir le résultat d'autres méthodes plus spécifiques.

Suivant le principe de "single responsability", ces fonctions vont aider au 
séquençage du programme et doivent souvent être séparées à nouveau pour 
permettre une bonne coordination de la séquence ou bien une forme de délégation 
des autres méthodes plus spécifiques ("separate concerns").


#### Specifics Methods

Des méthodes donc plus spécifiques, qui vont avoir une tâches bien particulière.
Généralement ce sont des méthodes qui reçoivent un "input" et retourne un "output",
et vont établir la même logique à chaque fois.

=> ce sont des blocs de code facilement réutilisable et testable
 
 <br>
 <br>

## Testing those


<img src="../assets/quote1.png" alt="quote about doing good practice in code">

The **specifics Methods are easy to tests**, put in an "input" and expecting the "output"
result.

The **Air Traffic Methods needs only & simply to check if the specifics methods are
been called**. No need to "input" / "output" system, just passing the parameter we
are expecting to check if the right specific or delegated methods have been called.
