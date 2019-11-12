# Patrón Abstract Factory para tener una interfaz única

* Status: Rejected.
* Deciders: Diego Montoto, Guillermo 
* Date: 2019-11-12

## Context and Problem Statement
* Existe un problema de diseño: el sistema debe proporcionar una única interfaz para las posibles interfaces que gestionan diferentes usuarios de manera que el sistema sea más fácil de administrar y menos complejo. 
* Se propone el patrón Abstract Factory para encapsular un grupo de fábricas individuales bajo un tema común y utilizar interfaces para crear objetos concretos.

## Decision Drivers

* RF018: Interfaz genérica

## Decision Outcome

## Pros and Cons of the Options

### Pros
* Los objetos creados de cada subtipo (Interfaz de Usuario de Administrador, Interfaz de Usuario de Operario de Emergencias, Interfaz de Usuario de Asignador de Recursos, Interfaz de Usuario de Operario de Unidades Activas) se enmascaran detrás de una interfaz común entre todos ellos (Interfaz de Usuario) con la finalidad de que estos puedan variar sin afectar la forma en que los usuarios interactúan con ellos y así simplificar el diseño.
* Los objetos concretos fabricados (en nuestro caso, interfaces de usuario) podrán hacer tareas similares pero con detalles de implementación diferentes.
* Se facilita la administración del sistema.
* Se delega la responsabilidad de crear los objetos.
* Escalabilidad: se pueden crear nuevas factorías.

### Cons
* El sistema solo necesitaría una factoría de interfaces de usuario, por lo que se desaprovecha la capacidad de este patrón.

## Links


