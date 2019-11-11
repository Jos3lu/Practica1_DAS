# Módulo de traducción: Microsoft Azure Translator Text API

* Status: Proposed.
* Deciders: Noelia Martínez (ASC), Óscar Rivas (ASC).
* Date: 2019-11-11

## Context and Problem Statement
El Sistema de Comunicaciones Internacionales necesita hacer uso de un Módulo de traducción simultánea. 
Se plantea como opción Microsoft Azure Translator Text API. 
Microsoft Translator es un servicio de traducción automática basado en la nube. En el centro de este servicio está Translator Text API, que da servicio a diversos productos y servicios de Microsoft y que utilizan miles de empresas en todo el mundo en sus aplicaciones y flujos de trabajo para que su contenido llegue a una audiencia mundial.
Fuente [https://docs.microsoft.com/es-es/azure/cognitive-services/translator/]

## Decision Drivers
* RF016.1: Módulo de traducción

## Decision Outcome

## Pros and Cons of the Options

### Pros
* Traduce 60 idiomas diferentes.
* Traducción automática neuronal de Microsoft Translator, con traducciones más fluidas y humanas, que pueden ajustarse más al texto original.
* Detección automática de idioma.
* Funcionalidad local (no necesita conexión a Internet), lo que resulta útil para no sobrecargar la red.
* Tarifas asequibles.
* Alta escalabilidad.
* Documentación completa disponible, así como servicio técnico.
* Custom Translator, una extensión del servicio Microsoft Translator, se puede usar en combinación con Translator Text API para ayudar a personalizar el sistema de traducción neuronal y mejorar la traducción para nuestra terminología y estilo específicos. 
Esto nos permitiría ajustar las traducciones a los términos técnicos específicos del Sistema Complejo de Emergencias.

### Cons
* Integración compleja.


## Links
* [ADR-0015]-(0015-Sistema de comunicaciones internacionales.md)
