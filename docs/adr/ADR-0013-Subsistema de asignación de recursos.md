# Subsistema de asignación de recursos
* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-09

## Context and Problem Statement

* El Sistema de Emergencias (SE) necesita disponer de un mecanismo de asignación y monitorización de recursos para tratar las emergencias activas. 

* Los asignadores de recursos, que se encuentran en el Centro de Emergencias, son los que reciben la información en tiempo real, y monitorizan y asignan recursos (elementos activos de emergencia como ambulancias, bomberos, policías…). 

* Los operarios de unidades activas reciben esta información en sus smartphones y tablets en tiempo real. 

## Decision Drivers

* RF002.3: Gestión de llamadas entrantes.
* RF003: Monitorizar recursos.
* RF005.3: Operarios de unidades activas.
* RF005.4: Asignadores de recursos.
* RF014: Pre-asignar unidades activas.

## Decision Outcome

* El sistema contará con un Subsistema de Asignación de Recursos, que dispondrá de mecanismos para asignar y monitorizar recursos para tratar las posibles emergencias. 

* Las emergencias que se monitorizan son las que se registran previamente por el Subsistema de Detección. 

* Los asignadores de recursos pueden asignar y monitorizar el estado de la emergencia y sus recursos asignados. 

* Los operarios de unidades activas reciben la asignación de recursos.

* Toda la información se transmite en tiempo real en la interfaz. 

## Pros and Cons of the Options

### Pros

* Este subsistema permitirá al SCE gestionar, controlar y monitorizar los recursos disponibles para hacer frente a las emergencias.
* Este subsistema está correctamente coordinado con el Subsistema de Detección.

### Cons


## Links 
* [ADR-0009] - (0009-Sistema de gestión de Emergencias.md)
* [ADR-0011] - (0011-Subsistema de detección de emergencias.md)
* [ADR-0012] - (0012-Subsistema de llamadas externas (salientes).md)
* [ASC-ADR-0013] - Problemas encontrados por los ASC en Reflection Time Iteración 4
