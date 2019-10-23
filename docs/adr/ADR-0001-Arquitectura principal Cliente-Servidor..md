# Arquitectura principal Cliente-Servidor.

* Status: proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: [YYYY-MM-DD when the decision was last updated]


## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real, por lo que vamos a utilizar una arquitectura Cliente-Servidor como principal.

## Decision Drivers

* RF006: Informacion en tiempo real.
* RF002: Sistema de comunicacion.
* RF013: Priorizacion de eventos.
* RF017.1: Generacion de noticias.


## Pros and Cons of the Options

### Pros
* La arquitectura cliente-servidor soporta respuesta por eventos.
* Esta arquitectura funciona mediante peticiones asincronas.


### Cons
* Es menos adaptable que la estilo por eventos


## Links 

* [ADR-0000]-(0000-Arquitectura principal por eventos.md).


