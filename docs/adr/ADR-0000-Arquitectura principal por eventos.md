# Arquitectura principal por eventos.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-10-29


## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real, por lo que vamos a utilizar una arquitectura por eventos como principal.

## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.
* RF013: Priorización de eventos.
* RF017.1: Generación de noticias.


## Considered Options

* [ADR-0001]-(0001-Arquitectura principal Cliente-Servidor.md).
* [ADR-0002]-(0002-Arquitectura principal MVC.md).


## Decision Outcome

Al emplear un estilo por eventos el sistema podrá responder a los cambios de forma eficiente y adaptarse a estos.

## Pros and Cons of the Options

### Pros
* La arquitectura por eventos permite al sistema detectar, adaptarse y gestionar de forma muy rápida las situaciones de emergencia, la información recibida de los sensores, 
  llamadas entrantes y comunicaciones internacionales.
* Al ser un sistema modular el bajo acoplamiento que proporciona la arquitectura por eventos es fundamental.


### Cons


## Links 
* [ADR-0007]-(0007-Sistema modular.md).