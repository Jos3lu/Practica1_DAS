# Patrón Factory Method para tener una interfaz única

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín
* Date: 2019-11-12

## Context and Problem Statement
* Existe un problema de diseño: el sistema debe proporcionar una única interfaz para las posibles interfaces que gestionan diferentes usuarios de manera que el sistema sea más fácil de administrar y menos complejo. 
* Se propone el patrón Factory Pattern que nos permite centralizar en la clase Factoría la creación de los subtipos de interfaces. 

## Decision Drivers

* RF018: Interfaz genérica

## Decision Outcome
* Se soluciona el problema de diseño creando una única interfaz para la creación de interfaces de usuario denominada Interfaz de Usuario.
* Los diferentes usuarios harán uso de distintas interfaces (Interfaz de Usuario de Administrador, Interfaz de Usuario de Operario de Emergencias, Interfaz de Usuario de Asignador de Recursos, Interfaz de Usuario de Operario de Unidades Activas) que heredarán comportamiento de esta interfaz común pero también tendrán comportamiento exclusivo propio.
* Esto facilita la administración y reduce la complejidad del sistema.

## Pros and Cons of the Options

### Pros
* Los objetos creados de cada subtipo (Interfaz de Usuario de Administrador, Interfaz de Usuario de Operario de Emergencias, Interfaz de Usuario de Asignador de Recursos, Interfaz de Usuario de Operario de Unidades Activas) se enmascaran detrás de una interfaz común entre todos ellos (Interfaz de Usuario) con la finalidad de que estos puedan variar sin afectar la forma en que los usuarios interactúan con ellos y así simplificar el diseño.
* Los objetos concretos fabricados podrán hacer tareas similares pero con detalles de implementación diferentes, como es el caso.
* Se delega al Factory Method la responsabilidad de crear los objetos.
* Escalabilidad: se podrán añadir nuevos subtipos de Interfaz de Usuario.

### Cons
* No permite la creación de nuevas factorías para nuevos tipos de productos.

## Note
* Los ASC sugieren que se acepte esta decisión y se rechace la decisión 0027-Patrón Abstract Factory. Consideramos que se ajusta más a las necesidades del sistema, porque es un desperdicio de recursos utilizar un patrón Abstract Factory cuando solo se va a necesitar una factoría.

## Links
[ADR-0027]-(0027-Patrón Abstract Factory.md), alternativa contemplada

