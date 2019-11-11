# Módulo de traducción: Google Cloud Translation

* Status: Proposed.
* Deciders: Diego Montoto, Guillermo Martín.
* Date: 2019-11-11

## Context and Problem Statement
El Sistema de Comunicaciones Internacionales necesita hacer uso de un Módulo de traducción simultánea. 
Se plantea como opción Google Cloud Translation. 
La API de Cloud Translation puede traducir dinámicamente texto entre miles de pares de idiomas. 
Cloud Translation forma parte de la familia más amplia de la API de Cloud Machine Learning. 
Fuente [https://cloud.google.com/translate/]

## Decision Drivers
* RF016.1: Módulo de traducción

## Decision Outcome

## Pros and Cons of the Options

### Pros
* Traduce un gran número de idiomas.
* Detección automática de idioma.
* Compatibilidad con glosarios
* Alta escalabilidad
* Integración sencilla
* Tarifas simples y asequibles

### Cons
* Traducciones no siempre fieles, especialmente en ámbitos técnicos, por lo que se podrían traducir incorrectamente ciertos términos relacionados con las emergencias.

## Links
* [ADR-0015]-(0015-Sistema de comunicaciones internacionales.md)
