# Gestor de llamadas entrantes

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11

## Context and Problem Statement
El Subsistema de Detección de Emergencias necesita un gestor de llamadas entrantes que al recibir una nueva llamada, la distribuya entre los operarios de emergencias disponibles y permita detectar y crear eventos de emergencias si así es necesario.

## Decision Drivers
* RF002.3: Gestión de llamadas entrantes.
* RF009: Distribución de las llamadas entrantes.


## Decision Outcome
* Se dispone de un Distribuidor de Llamadas, un módulo que distribuye llamadas entrantes entre los Operarios de Emergencias disponibles.
* A partir de la llamada, el operario puede decidir registrar una nueva emergencia.
* Mientras la llamada esté activa, el operario estará ocupado. Cuando la llamada termine, el operario volverá a estar disponible.
* Los operarios del Centro de Emergencias pueden gestionar hasta 20 llamadas simultáneas, las demás llamadas entran en una cola de llamadas pendientes.

## Pros and Cons of the Options

### Pros
* Este módulo gestiona de manera eficiente las llamadas al Centro de Emergencias.
* Se distribuirán las llamadas entrantes entre los operarios disponibles y nunca más de 20 a la vez, y con ello se consigue un reparto de trabajo adecuado.
* Se pueden registrar emergencias a partir de llamadas que se reciban.

### Cons
* Se necesita tener disponibles a 20 operarios que respondan las llamadas.
* Se necesita una cola de llamadas.

## Note
* Los ASC consideran que la decisión debería ser aprobada.

## Links
* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ADR-0014]-(0014-Usuarios del sistema.md)
