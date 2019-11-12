# Uso de patrón Facade

* Status: Proposed.
* Deciders: Noelia Martínez (ASC), Óscar Rivas (ASC).
* Date: 2019-11-12

## Context and Problem Statement
* Se necesita acceder a las diferentes interfaces específicas de los usuarios (Interfaz de Usuario de Administrador, Interfaz de Usuario de Operario de Emergencias, Interfaz de Usuario de Asignador de Recursos, Interfaz de Usuario de Operario de Unidades Activas)
de manera unificada para simplificar el sistema y el uso de estas interfaces.
* El patrón Facade provee de una interfaz unificada simple para acceder a una interfaz o grupo de interfaces de un subsistema.

## Decision Drivers

* RF018: Interfaz genérica

## Decision Outcome

* Al emplear el patrón Facade se accede a dichas interfaces de usuario de una manera unificada y simple y se reduce la complejidad del uso de las mismas.

## Pros and Cons of the Options

### Pros
* Se estructura el sistema y se reduce la complejidad con la división en subsistemas.
* Se minimizan las comunicaciones y dependencias entre subsistemas (en este caso, las diferentes Interfaces de Usuario).
* Se consigue un punto de entrada al sistema.

### Cons

## Links
* [ADR-0028]-(0028-Patrón Factory Method.md)
