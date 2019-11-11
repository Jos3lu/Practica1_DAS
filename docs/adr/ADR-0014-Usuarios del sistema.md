# Usuarios del sistema

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11


## Context and Problem Statement

Existen distintos tipos de usuarios que gestionan y utilizan el sistema, que son: administrador del sistema, operarios de emergencias, operarios de unidades activas y asignadores de recursos.
Se necesita definir qué funciones y permisos tiene cada usuario.

## Decision Drivers
* RF005: Tipos de usuario
* RF005.1: Administrador del sistema.
* RF005.2: Operarios de emergencias.
* RF005.3: Operarios de unidades activas.
* RF005.4: Asignadores de recursos.

## Decision Outcome
* Todos los usuarios tienen acceso a una interfaz del sistema.
* Las funciones y permisos del Administrador del Sistema no han sido definidas por el cliente.
* Los Operarios de Emergencias disponen de una interfaz para recibir y contestar llamadas entrantes, y registrar eventos a partir de ellas.
* Los Operarios de Unidades Activas disponen de una interfaz donde reciben información en tiempo real de las asignaciones correspondientes.
* Los Asignadores de Recursos disponen de una interfaz para monitorizar emergencias y asignar recursos.

## Pros and Cons of the Options

### Pros
* Todos los usuarios disponen de una interfaz que les permite cumplir sus funciones.

### Cons
* Que existan distintos tipos de usuario obliga a crear una interfaz diferente para cada uno y dificulta la escalabilidad.

## Note
* Los ASC sugieren que se apruebe esta decisión.

## Links

* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ADR-0012]-(0012-Subsistema de llamadas externas.md)
* [ADR-0013]-(0013-Subsistema de asignación de recursos.md)
