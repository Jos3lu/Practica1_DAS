# Sensores
* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-12


## Context and Problem Statement
* El Subsistema de Detección necesita disponer de sensores situados en diferentes puntos de la geografía que transmitan información constantemente al Centro de Control Remoto vía radio.
* Existirán diferentes sensores en función de las emergencias que se quieran tratar. En un principio, el cliente ha expresado que necesita sensores para detectar incendios, robos y gases tóxicos.
* Cada sensor es un componente hardware con su driver correspondiente que emite información en tiempo real.

## Decision Drivers
* RF011: Transmisión de información al centro de control remoto.

## Decision Outcome
* Habrá sensores de humo y de temperatura para detectar incendios.
* Habrá sensores de CO2 y otros gases tóxicos para detectar escapes de gas.
* Habrá Detectores de Control de Acceso, que sirven para detectar robos.
* Habrá pulsadores manuales, que sirven para notificar robos.
* Habrá sensores de vibración para identificar robos.
* Cada sensor tendrá un driver y emitirá información en tiempo real vía radio.

## Pros and Cons of the Options

### Pros
* Que cada sensor herede de una clase genérica facilita la escalabilidad: se podrán añadir más sensores y de más tipos, cada uno con su driver.

### Cons
* Los sensores son componentes hardware que tienen que someterse a un constante mantenimiento.

## Links

* [ADR-0011]-(0011-Subsistema de detección de emergencias.md)
* [ADR-0022]-(0022-Centro de control remoto.md)

