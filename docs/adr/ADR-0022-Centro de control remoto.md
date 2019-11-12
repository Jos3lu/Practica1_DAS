# Centro de Control Remoto
* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-12


## Context and Problem Statement
* El Subsistema de Detección necesita disponer de un Centro de Control Remoto que reciba información de sensores repartidos geográficamente, la analice y alerte al SCE cuando corresponda.

## Decision Drivers
* RF011: Transmisión de información al centro de control remoto.
* RF012: Alerta al sistema de emergencias.

## Decision Outcome
* El Centro de Control Remoto recibe y analiza la información que le llega vía radio de los sensores repartidos en diferentes puntos de la geografía.
* El Centro de Control lleva un registro de cada sensor del sistema.
* El Centro de Control dispone de un mecanismo de monitorización del estado de cada sensor.
* A partir del anális de esta información, detecta problemas, notificando al Sistema Complejo de Emergencias con una alerta y un SMS. El cliente no ha concretado cuáles son las condiciones exactas ante las que se debería alertar de una situación peligrosa.

## Pros and Cons of the Options

### Pros
* Se implementaría un Sistema de Detección que de manera efectiva y automática detectase las emergencias que pudiesen acontecer en un determinado territorio.

### Cons
* El Subsistema de Detección se vuelve más complejo y difícil de gestionar.

## Links

* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ASC-ADR-0022]- Problemas encontrados por los ASC durante el Reflection Time de la Iteración 7
