# Arquitectura principal MVC.

* Status: Proposed.
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
* La arquitectura MVC destaca por su bajo acoplamiento.
* Esta arquitectura soporta tratamiento de eventos.
* Es muy adecuada para la interacción con usuarios.


### Cons
* La arquitectura MVC responde de una manera menos eficiente al tratamento de eventos que el estilo por eventos.


## Links 

* [ADR-0000]-(0000-Arquitectura principal por eventos.md).


