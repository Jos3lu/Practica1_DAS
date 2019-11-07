# Sistema de gestión de Incidencias Internas (SI)

* Status: Discused.
* Deciders: Noelia Martínez, Óscar Rivas
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
* Una descripción textual de la emergencia.
* La localización.
* La fecha en la que se detectó.

El Sistema de Incidencias se encargará de registrar, gestionar y monitorizar estas incidencias hasta que sean solucionadas.

## Pros and Cons of the Options

### Pros

* Este registro permite identificar claramente qué tipo de incidencias se producen y cómo y cuándo se detectan.
* El registro es simple pero eficaz, lo que permite rapidez en su gestión.


### Cons

* Como las Incidencias se registran automáticamente gracias a mecanismos automatizados, como lo puede ser un sensor de incendios, nos parece que la información almacenada de la incidencia debería ser más simple. 
Por ello, los ASC consideramos que la descripción textual de la emergencia debería sustituirse por un indicador del estado actual de la emergencia (si sigue activa, si se acaba de detectar o si está resuelta) y de su nivel de gravedad.
Por lo demás, nos parece que la decisión se ajusta a las necesidades del cliente.

## Links

* [ADR-0008]-(0008-Gestión de incidencias internas y gestión de emergencias.md).
* [ADR-0010]-(0010-Sistema de Incidencias Internas.md).

