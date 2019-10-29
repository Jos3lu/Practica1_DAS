# Almacenamiento de incidencias mediante una base de datos Oracle Database.

* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-10-29


## Context and Problem Statement

Se quieren alamacenar las incidencias en el sistema de forma segura por lo que se plantea el uso de la tecnología de base de datos de oracle.
Para mas información sobre el funcionamiento y las tarifas ir a : 

https://www.oracle.com/es/database/


## Decision Drivers

* RF002: Sistema de comunicación.
* RF002.2: Gestión de incidencias internas del sistema.


## Considered Options


## Decision Outcome

Al generar las incidencias al recibir eventos el sistema reponderá de forma rápida y eficiente.


## Pros and Cons of the Options

### Pros
* Dado que nuestro sistema gestiona situaciones de emergencia, desde incendios hasta delitos, es fundamental que la base de datos este operativa siempre 
  por lo que el soporte técnico y la función de autorrepación ofrecida por oracle es vital para evitar fallos y podernos recuperar de ellos.

* Como la base datos proporciona un servicio autogestión por lo que elimina la gestión manual de los datos permitiendo que sea usada por usuarios con poco 
  conocimientos informáticos. 

### Cons

* Coste elevado del servicio.

## Links 

* [ADR-0003]-(0003-Eventos de llamadas entrantes.md).
* [ADR-0004]-(0004-Eventos de llamadas externas.md).
* [ADR-0005]-(0005-Gestión de incidencias.md).