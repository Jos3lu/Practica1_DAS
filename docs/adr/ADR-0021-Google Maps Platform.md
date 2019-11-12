# Algoritmo de planificación de rutas: Google Maps Platform

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-12


## Context and Problem Statement
* El subsistema de asignación de recursos necesita disponer de un algoritmo de optimización de rutas para calcular la ruta más corta entre dos puntos.
* Se propone utilizar Google Maps Platform, un set de APIs que permite obtener la mejor forma de ir de un sitio a otro con datos exhaustivos e información del tráfico en tiempo real.


## Decision Drivers
* RF004: Optimización de rutas

## Decision Outcome
* Se contará con un algoritmo de optimización de rutas que calculará la ruta más corta entre dos puntos de manera rápida y eficiente.

## Pros and Cons of the Options

### Pros
* Información de 64 millones de kilómetros de carreteras disponible.
* Actualización constante y datos de ubicación precisos en tiempo real.
* La infraestructura de Google es de gran calidad y segura.
* Información del estado del tráfico en tiempo real.
* Mucha documentación disponible, plataforma ampliamente conocida.


### Cons
* El plan "Premium" es caro.

## Links

* [ADR-0019]-(0019-Asignación de recursos disponibles.md)

