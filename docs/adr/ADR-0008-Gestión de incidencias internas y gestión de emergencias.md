# Gestión de incidencias internas y gestión de emergencias.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-06


## Context and Problem Statement

Queremos diseñar un sistema complejo de emergencias que gestione llamadas externas (las que realiza nuestro sistema), llamadas entrantes (las que se reciben) e incidencias internas.
Las incidencias internas son contratiempos intrínsecos al propio sistema, por ejemplo, averías en los sistemas electrónicos (cámaras, monitores) o de los elementos activos de emergencias (ambulancias, camiones de bomberos...) y demás contrariedades que puedan surgir (como, por ejemplo, incendios).
Por otra parte, las emergencias son aquellos eventos notificados por los usuarios externos a través de llamadas o por los propios sensores de emergencias. 

Se necesita gestionar estos dos elementos de la mejor manera posible.

## Decision Drivers

* RF002: Sistema de comunicación.
* RF007: Registro de emergencias.
* RF019: Registro de incidencias internas.

## Considered Options


## Decision Outcome

El Sistema Complejo de Emergencias contiene dos subsistemas a su vez, el Sistema de Incidencias Internas y el Sistema de Emergencias, que se encargan, respectivamente, de gestionar las incidencias internas y las emergencias mencionadas anteriormente.

## Pros and Cons of the Options

### Pros

* La separación de estos dos subsistemas nos permitirá gestionar de manera más eficiente los problemas que puedan surgir al sistema, a través de una asignación de recursos más rápida y clara.

### Cons

## Links 

* [ADR-0005] - Gestión de incidencias, decisión tomada en Time in ADD de la Iteración 2.
* [ASC-ADR-0005]- Problemas encontrados por los ASC durante el Reflection Time de la Iteración 2
