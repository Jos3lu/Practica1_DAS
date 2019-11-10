# Subsistema de llamadas externas (salientes)

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-09

## Context and Problem Statement

El Sistema de Emergencias (SE) necesita hacer uso de llamadas externas, nacionales e internacionales, para monitorizar y actualizar el estado de sus emergencias.
Es decir, los operarios de emergencias podrán hacer uso de estas llamadas para comprobar el estado de la emergencia y sus características o solicitar datos y otras cuestiones.


## Decision Drivers

* RF002.1: Gestión de llamadas externas.
* RF003: Monitorizar recursos.
* RF005.2: Operarios de emergencias.
* RF016: Comunicaciones internacionales.

## Decision Outcome

* El sistema contará con un Subsistema de Llamadas Externas, que será utilizado por los usuarios operarios de emergencias para monitorizar y gestionar las emergencias en curso.
* Las comunicaciones pueden ser internacionales.

## Pros and Cons of the Options

### Pros

* Este subsistema permite a los operarios del centro de emergencias poder llamar para monitorizar las emergencias en curso con la información recogida en la llamada.

### Cons

## Links 
* [ADR-0009] - (0009-Sistema de gestión de Emergencias.md)
* [ADR-0004] - (0004-Eventos de llamadas externas.md)
