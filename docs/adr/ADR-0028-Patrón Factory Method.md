# Patrón Factory Method para tener una interfaz única

* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín
* Date: 2019-11-12

## Context and Problem Statement
* Existe un problema de diseño: el sistema debe proporcionar una única interfaz para las posibles interfaces que gestionan diferentes usuarios de manera que el sistema sea más fácil de administrar y menos complejo. 
* Se propone el patrón Factory Pattern que nos permite centralizar en la clase Factoría la creación de los subtipos de interfaces. 

## Decision Drivers

* RF018: Interfaz genérica

## Decision Outcome

## Pros and Cons of the Options

### Pros
* Los objetos creados de cada subtipo (Interfaz de Usuario de Administrador, Interfaz de Usuario de Operario de Emergencias, Interfaz de Usuario de Asignador de Recursos, Interfaz de Usuario de Operario de Unidades Activas) se enmascaran detrás de una interfaz común entre todos ellos (Interfaz de Usuario) con la finalidad de que estos puedan variar sin afectar la forma en que los usuarios interactúan con ellos y así simplificar el diseño.
* Los objetos concretos fabricados podrán hacer tareas similares pero con detalles de implementación diferentes, como es el caso.
* Se delega al Factory Method la responsabilidad de crear los objetos.
* Escalabilidad: se podrán añadir nuevos subtipos de Interfaz de Usuario

### Cons
* No permite la creación de nuevas factorías para nuevos tipos de productos.

## Links


