# Patrón Observer para suscribirse a noticias

* Status: Rejected.
* Deciders: Diego Montoto, Guillermo Martín
* Date: 2019-11-12

## Context and Problem Statement
* Existe un problema de diseño: los diferentes usuarios deben poder subscribirse de manera distribuida a noticias generadas por sucesos en tiempo real y esta información debe estar permanentemente actualizada para los diferentes tipos de usuarios. 
* Se propone el patrón Observer para que los remitentes envíen mensajes no programados a los suscriptores.
* El patrón Observer es un patrón en el que un objeto llamado “sujeto” mantiene una lista con objetos dependientes a él, de forma que cuando un objeto cambie de estado se notifique y actualicen automáticamente todos los objetos que dependen de él.

## Decision Drivers

* RF017: Sistema de suscripción

## Decision Outcome

## Pros and Cons of the Options

### Pros
* Los suscriptores son notificados y actualizados automáticamente.
* Fácil implementación.

### Cons

* Con el patrón Observer, los componentes se acoplan estrechamente, al contrario de lo que sucede utilizando el patrón Publish-Subscribe.
* En el patrón Observer, los suscriptores conocen al sujeto, y viceversa, lo que dificulta la escalabilidad, pues habría que actualizar el registro de observadores cada vez que se añadiese un usuario al sistema.
* El patrón Observer se implementa principalmente de forma síncrona, es decir, el sujeto llama al método apropiado de todos sus observadores cuando ocurre algún evento. Esto puede ser perjudicial en el caso de que el usuario esté en medio de un proceso crítico.

## Links
[ADR-0026]-(0026-Publish Subscribe.md), alternativa seleccionada
