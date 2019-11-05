# Sistema modular.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-5


## Context and Problem Statement

Queremos diseñar un sistema de emergencias, que permita gestionar diferentes alertas y situaciones en tiempo real detectadas por diferentes fuentes, camaras de seguridad, llamadas entrante y salientes y comunicaciones internacionales.
 
## Decision Drivers

* RF006: Información en tiempo real.
* RF002: Sistema de comunicación.

## Decision Outcome

Al establecerse un sistema modular, se podrán realizar cambios y reparaciones en los diferentes modulos de forma independiente permitiendo que el resto del sistema funcione sin 
verse afectado.
   
## Pros and Cons of the Options

### Pros
* Al dividirse en sistema en diferentes modulos (gestión de llamadas, sistema de vigilancia, comunicaciones internacionales) en caso de fallo en un módulo el resto del sistema seguirá 
  funcionando lo que resulta vital en un sistema de emergencias.
* Se pueden realizar reparaciones y actualizaciones de los módulos sin afectar al resto del sistema.


### Cons

* Los sistemas modulares resultan más complejos de gestionar y requieren mayor grado especialización de los trabajadores responsables de mantener el sistema. 

#Link
Respuesta a lo discutido en el reflexión time de la primera iteración 
ASC-ADR-0002.md
