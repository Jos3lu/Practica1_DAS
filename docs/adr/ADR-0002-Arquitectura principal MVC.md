# Arquitectura principal MVC.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: [YYYY-MM-DD when the decision was last updated]


## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real, por lo que vamos a utilizar una arquitectura MVC como principal.

## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.
* RF013: Priorización de eventos.
* RF017.1: Generación de noticias.


## Pros and Cons of the Options

### Pros
* La arquitectura MVC destaca por su bajo acoplamiento, que resulta fundamental para nuestro sistema al ser modular.
* Esta arquitectura soporta tratamiento de eventos.
* Es muy adecuada para la interacción de los usuarios con el sistema, al permitir separar la lógica de negocio de la interfaz con el usuario,
  por lo que los operarios de emergencias contarán con una interfaz adaptada a su trabajo al igual que los operarios de unidades de emergencias 
  y administradores del sistema aunque trabajen con el mismo sistema.


### Cons
* La arquitectura MVC responde de una manera menos eficiente al tratamento de eventos que el estilo por eventos.


## Links 

* [ADR-0000]-(0000-Arquitectura principal por eventos.md).
* [ADR-0007]-(0007-Sistema modular.md).
