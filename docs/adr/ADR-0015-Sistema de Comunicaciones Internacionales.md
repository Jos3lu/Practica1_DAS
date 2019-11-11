# Sistema de Comunicaciones Internacionales

* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11


## Context and Problem Statement
El Sistema Complejo de Emergencias requiere de conexiones internacionales con otros países colindantes o cercanos. Para ello, se dispondrá de un módulo de traducción textual simultánea en tiempo real.
A partir de estas comunicaciones se crean y actualizan emergencias.

## Decision Drivers
* RF016: Conexiones internacionales

## Decision Outcome
* Se dispondrá de un Sistema de Conexiones Internacionales que permite que países cercanos se comuniquen textualmente entre sí, comunicándose emergencias y otras cuestiones.
* A partir de estas comunicaciones, el SCE puede crear y modificar emergencias. Por ejemplo, si el SCE está implementado en España y mantiene comunicaciones con Francia en las que se le notifica de un incendio cercano en Francia, el SCE creará un evento de emergencia y podrá monitorizarlo y asignar recursos si así es necesario.
* Se crea un Subsistema de Monitorización de Emergencias Internacionales, que a partir de mensajes textuales monitoriza emergencias que haya en otros países.
* Se crea un Subsistema de Detección de Emergencias Internacionales, que a partir de mensajes textuales entrantes genera eventos de emergencias.
* Los asignadores de recursos podrán asignar recursos a las emergencias internacionales porque se tratarán de manera idéntica que las nacionales.
* Se dispondrá de un módulo de traducción textual simultánea en tiempo real que traduzca los mensajes entre países.

## Pros and Cons of the Options

### Pros
* Se pueden crear y monitorizar emergencias internacionales a partir de comunicaciones entre países.
* Se pueden destinar recursos a emergencias internacionales que puedan afectarnos.
* El sistema funciona con traducción textual simultánea.

### Cons
* El SCE se vuelve más complejo y habría que destinar recursos a atender emergencias internacionales que puedan surgir.

## Links

* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ADR-0013]-(0013-Subsistema de asignación de recursos.md)
* [ADR-0014]-(0014-Usuarios del sistema.md)
