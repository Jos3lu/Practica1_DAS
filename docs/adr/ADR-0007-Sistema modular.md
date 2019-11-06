# Sistema modular.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-5


## Context and Problem Statement

Queremos diseñar un sistema de emergencias que permita gestionar diferentes alertas y situaciones en tiempo real detectadas por diferentes fuentes: cámaras de seguridad, llamadas entrantes y salientes y comunicaciones internacionales.
 
## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.
* Decisión modificada en Tiempo de Refinamiento a partir de las críticas de los ASC.

## Decision Outcome

Al ser un sistema modular, se podrán realizar cambios y reparaciones en los diferentes múdulos de forma independiente permitiendo que el resto del sistema funcione sin verse afectado.
   
## Pros and Cons of the Options

### Pros

* Al dividirse el sistema en diferentes modulos (gestión de llamadas, sistema de vigilancia, comunicaciones internacionales) en caso de fallo en un módulo el resto del sistema seguirá funcionando lo que resulta vital en un sistema de emergencias.
* Se pueden realizar reparaciones y actualizaciones de los módulos sin afectar al resto del sistema.

### Cons

* Los sistemas modulares resultan más complejos de gestionar y requieren mayor grado de especialización de los trabajadores responsables de mantener el sistema. 

## Links

* [ASC-ADR-0000.md] - Problemas encontrados por los ASC en el Reflection Time de la Iteración 1.
* [ASC-ADR-0002.md] - Problemas encontrados por los ASC en el Reflection Time de la Iteración 1.
