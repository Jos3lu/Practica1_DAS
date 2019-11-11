# Distribuidor de llamadas

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11


## Context and Problem Statement
El Gestor de Llamadas Entrantes necesita un sistema que distribuya las llamadas entrantes entre los Operarios de Emergencias disponibles en el momento de la llamada.

## Decision Drivers
* RF009: Distribución de las llamadas entrantes.

## Decision Outcome
* Se dispone de un Distribuidor de Llamadas, un módulo que distribuye llamadas entrantes a los Operarios de Emergencias disponibles.
* Este módulo guarda los ID de las llamadas activas y los ID de los operarios. También guarda qué llamada hay asignada a cada operario.
* Cuando el módulo recibe una nueva llamada, la asigna a un operario teniendo en cuenta los que hay disponibles.
* Cuando una llamada termina, el operario vuelve a estar disponible.

## Pros and Cons of the Options

### Pros
* Se distribuirán las llamadas entrantes entre los operarios disponibles de manera eficiente.

### Cons

## Note
* Los ASC sugieren que se apruebe esta decisión.

## Links

* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ADR-0014]-(0014-Usuarios del sistema.md)
* [ADR-0016]-(0016-Gestor de llamadas entrantes.md)

