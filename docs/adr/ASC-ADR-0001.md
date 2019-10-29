# Arquitectura principal Cliente-Servidor.

* Status: Discused.
* Deciders: Noelia Martínez, Óscar Rivas
* Date: 2019-10-29

## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real, por lo que vamos a utilizar una arquitectura Cliente-Servidor como principal.

## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.
* RF013: Priorización de eventos.
* RF017.1: Generación de noticias.


## Pros and Cons of the Options

### Pros


### Cons
* No se concreta por qué al sistema le favorece funcionar mediante peticiones asíncronas.
* No entendemos qué eventos gestionaría en concreto la arquitectura cliente-servidor.
* Un problema que encontramos a esta arquitectura es el hecho de que se depende mucho de los recursos físicos disponibles (capacidad de los servidores del sistema).

## Links 

* [ADR-0000]-(0000-Arquitectura principal por eventos.md).


