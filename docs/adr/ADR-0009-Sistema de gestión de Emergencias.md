# ADR-0009 - Sistema de gestión de emergencias (SE)

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-07

## Context and Problem Statement

El sistema contará con un sistema de gestión de emergencias (SE) independiente del sistema de gestión de incidencias, que deberá detectar situaciones imprevistas, priorizar los eventos, asignar recursos a las diferentes emergencias y realizar llamadas entrantes y salientes (incluyendo llamadas internacionales).


## Decision Drivers

* RF002: Sistema de comunicación.
* RF003: Monitorizar recursos.
* RF008: Identificación de llamadas entrantes.
* RF010: Sistema de detección de emergencias.
* RF013: Priorización de eventos.
* RF014: Pre-asignar unidades activas.
* RF016: Comunicaciones internacionales.

## Decision Outcome

Este sistema de gestión de emergencias contará con los siguientes subsistemas:
* Subsistema de detección: encargado de detectar las situaciones inesperadas y llamadas entrantes y generar la emergencia correspondiente.
* Subsistema de asignación de recursos: asignará los recursos pertinentes para cada emergencia (ambulancias, helicópteros, etc)
* Subsistema de llamadas salientes (incluidas llamadas internacionales).

## Pros and Cons of the Options

### Pros

* Al tener un sistema dedicado a la gestión de emergencias, que a su vez se divide en diferentes subsistemas, se favorece la modularidad y el bajo acoplamiento.
* La priorización de eventos de emergencia facilita la asignación de recursos, de forma que las emergencias con mayor prioridad reciben antes los recursos necesarios.
* El tener un subsistema dedicado a la detección de emergencias permite detectar diferentes situaciones y llamadas y convertirlas en eventos de emergencia que el sistema pueda gestionar.

### Cons

### Note

* A los ASC nos parece adecuada esta división del Sistema de Emergencias y creemos que se debe aceptar la decisión, aunque no se especifica dónde se integran las llamadas internacionales.

## Links 
* [ADR-0008] - (0008-Gestión de incidencias internas y gestión de emergencias.md)
* [ADR-0007] - (0007-Sistema Modular.md).
