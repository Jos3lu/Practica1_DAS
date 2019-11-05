# Arquitectura principal Cliente-Servidor.

* Status: Rejected.
* Deciders: Diego Montoto, Guillermo Martín.


## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real, por lo que vamos a utilizar una arquitectura Cliente-Servidor como principal.

## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.
* RF013: Priorización de eventos.
* RF017.1: Generación de noticias.


## Pros and Cons of the Options

### Pros
* La arquitectura cliente-servidor soporta respuesta por eventos, mediante peticiones al servidor.
* Esta arquitectura funciona mediante peticiones asincronas, permitiendo que tanto los operarios del sistema como los operarios de unidades de emergencias y administradores del sistema puedan
  solicitar y enviar información al sistema.


### Cons
* Para que esta arquitectura nos ofrezca el rendimiento necesario y un servicio venticuatro horas incluso al realizar actualizaciones grandes del sistema se requieren una bran cantidad de recursos físicos.
* Es menos adaptable que el estilo por eventos.


## Links 

* [ADR-0000]-(0000-Arquitectura principal por eventos.md).
* [ADR-0007]-(0007-Sistema modular.md).

