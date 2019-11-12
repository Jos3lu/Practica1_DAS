# Patrón Publish-Subscribe para suscribirse a noticias

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo 
* Date: 2019-11-12

## Context and Problem Statement
* Existe un problema de diseño: los diferentes usuarios deben poder subscribirse de manera distribuida a noticias generadas por sucesos en tiempo real y esta información debe estar permanentemente actualizada para los diferentes tipos de usuarios. 
* Se propone el patrón Publish-Subscribe para que los remitentes envíen mensajes no programados a los suscriptores.

## Decision Drivers

* RF017: Sistema de suscripción

## Decision Outcome
* Este patrón serviría para notificar a los usuarios de una actualización relacionada con noticias.

## Pros and Cons of the Options

### Pros

* Componentes del sistema podrán proporcionar información (noticias) a otros componentes (usuarios) a medida que ocurren los eventos.
* La mensajería asincrónica es una forma efectiva de desacoplar los remitentes de los consumidores y evitar bloquear al remitente para que espere una respuesta.
* Aumenta la escalabilidad y mejora la capacidad de respuesta del remitente. El remitente puede enviar rápidamente un solo mensaje al canal de entrada y luego volver a sus responsabilidades principales de procesamiento. La infraestructura de mensajería es responsable de garantizar que los mensajes se entreguen a los suscriptores interesados.
* Permite el procesamiento diferido o programado. Los suscriptores pueden esperar para recoger los mensajes hasta las horas de menor actividad, o los mensajes se pueden enrutar o procesar de acuerdo con un horario específico. Esto viene bien para que las noticias se procesan cuando el usuario no esté ocupado atendiendo una emergencia o algún proceso crítico.

### Cons

* Manejo de suscripciones. La infraestructura de mensajería debe proporcionar mecanismos que los consumidores puedan usar para suscribirse o darse de baja de los canales disponibles.
* Seguridad. La conexión a cualquier canal de mensajes debe estar restringida por la política de seguridad para evitar escuchas de usuarios o aplicaciones no autorizados.

## Note
* Los ASC sugieren que se acepte esta decisión y se rechace la decisión 0026-Patrón Observer. Consideramos que se ajusta más a los requerimientos del sistema principalmente porque que el sistema necesita ser escalable y con bajo acoplamiento entre componentes.

## Links
[ADR-0026]-(0026-Patrón Observer.md), alternativa contemplada.
