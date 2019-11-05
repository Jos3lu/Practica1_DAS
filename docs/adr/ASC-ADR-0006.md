# Almacenamiento de incidencias mediante una base de datos Oracle Database.

* Status: Discused.
* Deciders: Noelia Martínez, Óscar Rivas.
* Date: 2019-11-05


## Context and Problem Statement

Se quieren alamacenar las incidencias en el sistema de forma segura por lo que se plantea el uso de la tecnología de base de datos de oracle.
Para mas información sobre el funcionamiento y las tarifas ir a : 

https://www.oracle.com/es/database/


## Decision Drivers

* RF002: Sistema de comunicación.
* RF002.2: Gestión de incidencias internas del sistema.


## Considered Options


## Decision Outcome

Al almacenar las incidencias en una base de datos de oracle contaremos con un sistema autogestionado y autorreparable con un servicio técnico de 
calidad.


## Pros and Cons of the Options

### Pros
* Dado que nuestro sistema gestiona situaciones de emergencia, desde incendios hasta delitos, es fundamental que la base de datos este operativa siempre 
  por lo que el soporte técnico y la función de autorrepación ofrecida por oracle es vital para evitar fallos y podernos recuperar de ellos.

* Como la base datos proporciona un servicio autogestión por lo que elimina la gestión manual de los datos permitiendo que sea usada por usuarios con poco 
  conocimientos informáticos. 

### Cons

* Coste elevado del servicio.

* Los ASC consideramos dos grandes inconvenientes de tener un sistema que almacene las incidencias en una base de datos de oracle.
El elevado coste de las licencias y la necesidad de contratar a un especialista certificado en sistemas oracle, ya que si no se hace una buena instalación del software, este mismo puede llegar a ser notablemente lento.
El coste de contratación de dicho especialista puede llegar a ascender hasta $5000 mensuales.

## Links 

* [ADR-0003]-(0003-Eventos de llamadas entrantes.md).
* [ADR-0004]-(0004-Eventos de llamadas externas.md).
* [ADR-0005]-(0005-Gestión de incidencias.md).
