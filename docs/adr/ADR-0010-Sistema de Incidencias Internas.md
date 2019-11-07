# Sistema de gestión de Incidencias Internas (SI)

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-7


## Context and Problem Statement

Queremos diseñar un sistema que detecte y gestione incidencias que puedan ocurrir en nuestro Sistema Complejo de Emergencias, como lo puede ser un incendio o una avería en alguna de nuestras unidades activas.


## Decision Drivers

* RF019: Registro de incidencias.
* RF002.2: Gestión de incidencias internas del sistema.

## Decision Outcome

Las Incidencias internas que sucedan, se registrarán con:
* Un identificador.
* Una categoría (incendio, avería, inundación, otro).
* Estado (detected, in progress, solved).
* Nivel de gravedad de la incidencia.
* La localización.
* La fecha en la que se detectó.

El Sistema de Incidencias se encargará de registrar, gestionar y monitorizar estas incidencias hasta que sean solucionadas.

## Pros and Cons of the Options

### Pros

* Este registro permite identificar claramente qué tipo de incidencias se producen y cómo y cuándo se detectan.
* El registro es simple pero eficaz, lo que permite rapidez en su gestión.


### Cons

### Note

* Se ha cambiando la información que se registrará de cada incidencia teniendo en cuenta las consideraciones realizadas por los ASC.

## Links

* [ADR-0008]-(0008-Gestión de incidencias internas y gestión de emergencias.md).
* [ASC-ADR-0010] - Consideraciones realizadas por los ASC en Time in refined de la Iteración 3.
