# Princípios Design e Arquitetura
Segue abaixo alguns princípios que são amplamente recomendado pela comunidade de desenvolvimento Orintado a Objetos.

## S O L I D
##### Single Responsibility (SRP)
> *A CLASS SHOULD HAVE ONLY ONE REASON TO CHANGE.*
>
If a class has more than one responsibility, then the responsibilities become coupled.
Changes to one responsibility may impair or inhibit the class’ ability to meet the others.
This kind of coupling leads to fragile designs that break in unexpected ways when changed.

> *[Uncle Bob - SRP](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod)*

##### Open and Closed (OCP)
> *SOFTWARE ENTITIES (CLASSES, MODULES, FUNCTIONS, ETC.) SHOULD BE OPEN FOR EXTENSION, BUT CLOSED FOR MODIFICATION.*
>
> When a single change to a program results in a cascade of changes to dependent modules, that program exhibits the undesirable attributes that we have come to associate with “bad” design. The program becomes fragile, rigid, unpredictable and unreusable. The open-closed principle attacks this in a very straightforward way. It says that you should design modules that never change. When requirements change, you extend the behavior of such modules by adding new code, not by changing old code that already works.

> *[Uncle Bob -OCP](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod)*

##### Liskov substitution principle (LSP)

> *FUNCTIONS THAT USE POINTERS OR REFERENCES TO BASE
CLASSES MUST BE ABLE TO USE OBJECTS OF DERIVED CLASSES WITHOUT KNOWING IT.*
The above is a paraphrase of the Liskov Substitution Principle (LSP). Barbara Liskov first wrote it as follows nearly 8 years ago¹

>> ***" What is wanted here is something like the following substitution property: If for each object o1 of type S there is an object o2 of type T such that for all programs P defined in terms of T, the behavior of P is unchanged when o1 is substituted for o2 then S is a subtype of T."***
>
The importance of this principle becomes obvious when you consider the conse-quences of violating it. If there is a function which does not conform to the LSP, then that function uses a pointer or reference to a base class, but must know about all the derivatives
of that base class. Such a function violates the Open-Closed principle because it must be modified whenever a new derivative of the base class is created.
>

##### Interface segregation (ISP)

##### Dependency inversion principle (DIP)

## Principles of Package Architecture
##### The Release Reuse Equivalency Principle (REP)

##### The Common Closure Principle (CCP)

##### The Common Reuse Principle (CRP)

## Arquitetura Hexagonal

## Domain Driven Design
