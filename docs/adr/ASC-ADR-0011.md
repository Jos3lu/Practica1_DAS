# Subsistema de detección de emergencias

* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-09

## Context and Problem Statement

* El Sistema de Emergencias (SE) necesita detectar emergencias mediante sensores que recojan los eventos inesperados que puedan surgir. Estos sensores están repartidos en diferentes puntos de la geografía.
* Además, se registran emergencias a partir de las llamadas que entran al Centro de Emergencias y son respondidas por los operarios de emergencias.

## Decision Drivers

* RF002.3: Gestión de llamadas entrantes.
* RF005.2: Operarios de emergencias.
* RF007: Registro de emergencias.
* RF010: Sistema de detección de emergencias.
* RF011: Transmisión de información al centro de control.
* RF012: Alertas al sistema de emergencias.

## Decision Outcome

* El sistema contará con un Subsistema de Detección de Emergencias, que será el encargado de detectar una emergencia y generar el evento correspondiente.
* Por una parte, se detecta una emergencia cuando un operario, a partir de una llamada que ha recibido en el Centro de Emergencias, así lo registra.
* Por otra parte, se detecta una emergencia cuando alguno de los sensores distribuidos geográficamente, lo identifica automáticamente.

## Pros and Cons of the Options

### Pros

* Este subsistema permitirá al SCE detectar y registrar de manera eficaz las emergencias que se notifiquen a través de una llamada o de un sensor.

### Cons

* Los ASC consideramos que dado que se permiten conexiones internacionales con otros países cercanos, se debería especificar cómo se van a detectar las emergencias en ellos. 
Nosotros proponemos que se detecten de igual manera que en el propio país: con llamadas al Centro de Emergencias procedentes de aquellos países, si bien no se dispondrá de sensores en esos territorios.

## Links 
* [ADR-0009] - (0009-Sistema de gestión de Emergencias.md)
* [ADR-0003] - (0003-Eventos de llamadas entrantes.md)
