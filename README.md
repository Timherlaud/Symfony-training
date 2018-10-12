# Symfony Training

## Conception


### Law of demeter
un objet doit éviter d'invoquer des méthodes d'un membre objet retourné par une autre méthode.

### Value object
In computer science, a value object is a small object that represents a simple entity whose equality is not based on identity: i.e. two value objects are equal when they have the same value,


### Idempotent
signifie qu'une opération a le même effet qu'on l'applique une ou plusieurs fois.

YAGNI = acronyme anglais de you ain't gonna need it,

### Gang of four
Erich Gamma, Richard Helm,
Ralph Johnson et John Vlissides

### SOLID
![alt text](https://cdn-images-1.medium.com/max/1200/1*yO6YGExWLJl5VOUL61xXvQ.jpeg "SOLID")
Responsabilité unique (single responsibility principle)
une classe, une fonction ou une méthode doit avoir une et une seule responsabilité
Ouvert/fermé (open/closed principle)
une classe doit être ouverte à l'extension, mais fermée à la modification
Substitution de Liskov (Liskov substitution principle)
une instance de type T doit pouvoir être remplacée par une instance de type G, tel que G sous-type de T, sans que cela ne modifie la cohérence du programme
Ségrégation des interfaces (interface segregation principle)
préférer plusieurs interfaces spécifiques pour chaque client plutôt qu'une seule interface générale
Inversion des dépendances (dependency inversion principle)
il faut dépendre des abstractions, pas des implémentations

## Design Pattern
###Creational Patterns
####Abstract factory
Ce DP permet de créer des instances pour des groupes, des familles de classes différents sans que le code qui les utilise n’ait à se soucier de ces groupes ou familles.
####Builder
Ce DP décrit comment séparer la construction d’un objet complexe de sa représentation.
####Factory method
Cet DP ressemble à l’abstract factory en permettant à une méthode de créer des instances dérivées d’une classe mère.
####Prototype
Le prototype est une instance correctement initialisée servant de modèle à la création d’un clone. Cet DP permet par exemple d’implémenter une collection d’objets décrivant des formes géométriques.
####Singleton
Il permet de s’assurer qu’une seule instance d’une classe ne peut exister à un moment donné et fournit un point d’accès vers cette instance.
####Adapter
L’adapter (adaptateur) est un procédé permettant d’habiller en quelque sorte une classe en la faisant ressembler, du point de vue de son interface, à une autre.
####Bridge
Ce DP créé un pont entre une classe et l’implémentation de tout ou partie de son code.
####Composite
Le composite est un DP permettant de créer des structures arborescentes d’objets ayant une relation tout/partie tout en autorisant les clients de traiter les objets individuels et les compositions de façon uniforme.
####Decorator
Avec ce pattern on dispose d’un moyen efficace pour accrocher de nouvelles fonctions à un objet dynamiquement lors de l’exécution.
####Façade
Il s’agit ici de proposer une .. façade masquant la complexité de tout un système.
####Flyweight
Cette DP autorise le partage de très nombreux objets de petite granularité de façon efficace.
####Proxy
ce DP définit comment un objet permet d’en contrôler un autre. On l’utilise très fréquemment pour manipuler localement la représentation d’un objet distant
###Behavioral patterns
####Chain of responsability
Ce DP définit une structure permettant de découpler un objet émettant des requêtes des objets chargés de les traiter.
####Command
Lorsqu’un système doit gérer de nombreuses commandes qui peuvent être mises en attente et être éventuellement annulée il est intéressant de transformer chaque commande en un objet placé dans une liste.
####Interpreter
Ce DP propose une structure de classes permettant, à partir d’un langage et d’une représentation de sa grammaire, de pouvoir interpréter des phrases écrites dans ce langage.
####Iterator
Ce DP propose un moyen d’accéder à tous les objets d’une liste séquentiellement sans avoir besoin d’exposer la structure interne qui maintient cette liste.
####Mediator
Cet DP définit le fonctionnement d’un objet qui gère les interactions entre d’autres objets. C’est un médiateur.
####Memento
Ce DP met en place un mécanisme permettant de capturer l’état interne d’un objet pour le stocker et restaurer ultérieurement l’objet dans le même état.
####Observer
Lorsque plusieurs objets doivent être averti d’une notification il faut trouver un moyen pour distribuer le message.
####State
Ce DP décrit comment un objet peut modifier son comportement quand son état change.
####Strategy
Pourvoir modifier un algorithme de façon transparente peut être très utile.
####Template method
Ce DP définit comment mettre en place un algorithme dont les étapes sont figées mais dont la réalisation de ces dernières peut être déléguée à d’autres objets offrant des variations de traitement.
####Visitor
Le visiteur peut être vu comme l’opération complémentaire à l’itérateur. Le visiteur est une classe définissant une opération sur une autre classe.

###PHP
5.4 => trait



##Algorithmique
##Base de données
##Conception logicielle
##HTTP
https://fr.wikipedia.org/wiki/Liste_des_codes_HTTP
##La POO avec PHP
##SYMFONY
DEBUG: https://symfony.com/doc/current/components/debug.html
### command line
https://symfony.com/doc/2.5/cookbook/console/usage.html
### Dependency Injection
 what is the correct way to override a service class  using ContainerBuilder class?
$container->getDefinition('my.service')->setClass('My\Service\Class')

https://symfony.com/doc/current/service_container/compiler_passes.html
### Routing
https://symfony.com/doc/current/routing/scheme.html
### Twig
https://twig.symfony.com/doc/2.x/internals.html
https://symfony.com/doc/current/templating/twig_extension.html
https://symfony.com/doc/current/reference/twig_reference.html#humanize
### Automated tests
### Form
https://symfony.com/doc/current/security/csrf.html
https://symfony.com/doc/current/forms.html
https://symfony.com/doc/current/form/disabling_validation.html
https://symfony.com/doc/current/form/use_empty_data.html

### PHP Standards Recommendations
- PSR 1 & PSR 2 => codding style
- PSR 3  => logger interface
- PSR 4 + PSR 0  => autoloader
- PSR 6  => Caching Interface
- PSR 16 => SimpleCaching Interface
- PSR 7  => HTTP Message Interface
- PSR 11 => ContainerInterface
- PSR 13 => Link Interface

### Events
https://symfony.com/doc/current/reference/events.html

### Other
https://symfony.com/doc/current/templating/hinclude.html

##Securité
https://symfony.com/doc/current/security/custom_provider.html
https://symfony.com/doc/current/security/voters.html

#Other
0xFF = 255

# links

- [Override error templates](https://symfony.com/doc/current/controller/error_pages.html)

- [Associations] (https://www.doctrine-project.org/projects/doctrine-orm/en/latest/reference/unitofwork-associations.html#bidirectional-associations)

- [Component Filesystem] (https://symfony.com/doc/current/components/filesystem.html#isabsolutepath)

- https://www.w3.org/International/questions/qa-lang-priorities
- https://tools.ietf.org/html/rfc2616#page-79
- https://symfony.com/doc/4.0/email.html
- https://symfony.com/doc/current/components/debug.html#enabling-the-exception-handler
- https://symfony.com/doc/current/reference/configuration/framework.html#logging
- https://symfony.com/doc/current/security/security_checker.html
- https://symfony.com/doc/current/contributing/code/bc.html

https://fr.wikipedia.org/wiki/Liste_des_codes_HTTP

https://github.com/jmolivas/symfony-certification-guide

https://symfony.com/doc/current/quick_tour/the_architecture.html
