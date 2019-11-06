# Almacenamiento de datos mediante una base de datos Oracle Database.

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-10-29


## Context and Problem Statement

Se quieren almacenar los datos necesarios para registrar las emergencias y las incidencias que será pertinente que el sistema monitorice. Se plantea para el almacenamiento y tratamiento de datos el sistema de gestión de base de datos Oracle Database.
Para más información sobre el funcionamiento y las tarifas ir a la página web: 

https://www.oracle.com/es/database/


## Decision Drivers

* RF002: Sistema de comunicación.
* RF003: Monitorizar recursos.
* RF007: Registro de emergencias.
* RF019: Registro de incidencias internas.


## Considered Options


## Decision Outcome

Al almacenar las incidencias en una base de datos de Oracle contaremos con un gestor seguro y eficiente adecuado para la complejidad del sistema que estamos diseñando. 


## Pros and Cons of the Options

### Pros
* Dado que nuestro sistema gestiona situaciones de emergencia es fundamental que la base de datos esté operativa siempre, por lo que el soporte técnico y la función de autorreparación ofrecida por oracle es vital para evitar fallos y podernos recuperar de ellos.

* Protección de datos: seguridad completa en el entorno de producción y de pruebas y gestión de copias de seguridad, indispensable teniendo en cuenta que manejamos datos críticos.

* Alta disponibilidad: escalabilidad, protección y alto rendimiento para la actividad empresarial, punto relevante pues nuestro sistema es complejo y escalable y necesita ser eficiente para gestionar los procesos con la mayor rapidez posible.


### Cons

* Coste elevado del servicio.

## Links 

* [ADR-0003]-(0003-Eventos de llamadas entrantes.md).
* [ADR-0004]-(0004-Eventos de llamadas externas.md).
* [ADR-0005]-(0005-Gestión de incidencias.md).
* [ASC-ADR-006] - Contras propuestos por los ASC en Reflection Time
