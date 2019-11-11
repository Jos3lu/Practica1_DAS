# Funcionamiento de la asignación de recursos disponibles

* Status: Discused.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11


## Context and Problem Statement
* El subsistema de asignación de recursos necesita disponer de medios para pre-asignar unidades activas disponibles a una emergencia.
* Las emergencias necesitan ser priorizadas (el cliente no ha especificado cómo), pudiendo haber como máximo 20 activas de manera simultánea.
* Los asignadores de recursos pueden asignar operarios de unidades activas para atender una emergencia.
* Se necesita un algoritmo de optimización de ruta que puede ser utilizado al pre-asignar y por los operarios de emergencias al asignar recursos a una emergencia.

## Decision Drivers
* RF003: Monitorizar recursos
* RF005.3: Operarios de unidades activas.
* RF005.4: Asignadores de recursos.
* RF013: Priorización de eventos.
* RF014: Pre-asignar unidades activas

## Decision Outcome
* El Subsistema de Asignación de Recursos contará con un módulo que guarde el ID de las emergencias activas registradas junto a una lista de sus recursos asignados.
* Habrá un mecanismo para pre-asignar recursos a una emergencia que pase a estar activa, pero no se ha explicitado por el cliente cuáles son los criterios para hacer esta asignación.
* Los asignadores de recursos pueden cambiar la asignación de recursos a una emergencia en cualquier momento.
* Se utiliza un algoritmo de optimización de rutas para seleccionar qué operarios de unidades activas se asignan a una emergencia.

Ejemplo de funcionamiento: un incendio pasa a ser una de las 20 emergencias activas, por lo que se le pre-asigna una determinada cantidad de recursos (por ejemplo, 2 camiones de bomberos y un coche de policía). Utilizando el algoritmo de optimización, se manda a los operarios de unidades activas más cercanos al incendio para que vayan a atenderlo. Más tarde, un asignador de recursos decide destinar un camión de bomberos más a esa emergencia, por lo que se vuelve a seleccionar al operario más cercano al lugar de la emergencia.

## Pros and Cons of the Options

### Pros
* El SCE contará con un sistema de asignación de recursos eficaz.
* La selección de unidades activas se realiza de manera automática y óptima (se eligen automáticamente las unidades activas disponibles más cercanas al foco de la emergencia).

### Cons
* Se necesita un algoritmo de optimización eficiente.

## Note
* Los ASC sugieren que se acepte esta propuesta, aunque han notado que falta explicitar cómo se va a gestionar el sistema las emergencias a la espera de ser atendidas.

## Links

* [ADR-0013]-(0013-Subsistema de asignación de recursos.md)
* [ADR-0014]-(0014-Usuarios del sistema.md)

