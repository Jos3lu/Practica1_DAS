# Sistema de video-vigilancia

* Status: Accepted.
* Deciders: Diego Montoto, Guillermo Martín
* Date: 2019-11-12

## Context and Problem Statement
* Se cuenta con cámaras remotas que se necesita que transmitan vídeo al sistema de emergencias. 
* El sistema de emergencias puede detectar emergencias a partir de las imágenes capturadas por las cámaras, una vez procesadas.

## Decision Drivers

* RF010: Sistema de detección de emergencias
* RF011: Transmisión de información al centro de control.

## Decision Outcome
* Dentro del Subsistema de detección de emergencias, habrá una clase "Procesador de vídeo" que recibe información en vídeo procedente de las cámaras de diferentes lugares.
* Esta clase procesa esta información y si es el caso, detecta una emergencia que se pueda estar produciendo.

## Pros and Cons of the Options

### Pros
* Este sistema de video-vigilancia permite detectar emergencias a partir de imágenes que se capturan por las cámaras repartidas en diferentes localizaciones geográficas, lo que puede ser muy útil.

### Cons
* El mantenimiento del sistema se dificulta.
* El coste del servicio se incrementa.

## Note
* Los ASC consideramos que la decisión debería ser aceptada.

## Links
* [ADR-0011]-(0011-Subsistema de detección de emergencias.md).
* [ADR-0023]-(0023-Sensores.md).
