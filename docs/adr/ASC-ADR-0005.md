# Gestion de incidencias.

* Status: Discused.
* Deciders: Noelia Martínez, Óscar Rivas
* Date: 2019-11-05


## Context and Problem Statement

Queremos diseñar un sistema de gestión de incidencias que permita a los operarios de emergencias almacenar las incidencias en una base de datos, crear incidencias al recibir llamadas entrantes y solicitar información o notificar mediante llamadas externas.

## Decision Drivers

* RF002: Sistema de comunicación.
* RF002.2: Gestión de incidencias internas del sistema.


## Considered Options


## Decision Outcome

Al generar las incidencias al recibir eventos el sistema reponderá de forma rápida y eficiente.


## Pros and Cons of the Options

### Pros

* Al emplear una arquitectura por eventos como la arquitectura principal de la aplicación, las llamadas entrantes y externas deben tratarse como evntos para que el sistema pueda generar las incidencias de 
  al detectar dichas llamadas 
* Dado que el sistema genera las incidencias al recibir el evento de llamada pueden dedicarse los recursos fisicos a otras funciones mientras no se reciben llamadas 

### Cons
* Los ASC consideramos que esta decisión no se ajusta a las necesidades del cliente. El sistema debe gestionar incidencias internas y emergencias.
Consideramos que las incidencias internas son contratiempos intrínsecos al propio sistema, por ejemplo, averías en los sistemas electrónicos (cámaras, monitores) o de los elementos activos de emergencias (ambulancias, camiones de bomberos...) y demás contrariedades que puedan surgir.
Por otra parte, las emergencias son aquellos eventos notificados por los usuarios externos a través de llamadas o por los propios sensores de emergencias.
Por tanto, sugerimos que se separe la gestión y tratamiento de estos diferentes eventos.  

## Links 

* [ADR-0003]-(0003-Eventos de llamadas entrantes.md).
* [ADR-0004]-(0004-Eventos de llamadas externas.md).
