# Coordinación con UME y Policía

* Status: Discused.
* Deciders: Diego Montoto, Guillermo Martín
* Date: 2019-11-12

## Context and Problem Statement
* El sistema necesita una solución para coordinarse con las unidades de policía y Unidad Militar de Emergencias (UME). 
* El cliente no ha especificado el funcionamiento de esta coordinación ni cómo afecta al sistema.
* Las comunicaciones deben estar cifradas por radio. Para conseguir esto, se utilizará DSP 9000. (Más información: https://www.tccsecure.com/Products/radio-encryption/DSP9000-detail-es.aspx)

## Decision Drivers
* RF015: Coordinación con policía y UME.

## Decision Outcome
* Se dispondrá de un sistema de coordinación con la policía y UME con un módulo encargado de recibir mensajes y otro encargado de enviarlos.
* Ambos módulos utilizan el cifrado de radios militares DSP 9000.

## Pros and Cons of the Options

### Pros
* La coordinación con la policía y UME puede facilitar la gestión de emergencias.
* La solución de cifrado de radio universal DSP 9000 funciona con la mayoría de las marcas y modelos, y se superpone imperceptiblemente con las redes preexistentes para brindar seguridad punto a punto rentable y de primera calidad.

### Cons
* El sistema es más complejo y se necesitarán recursos para realizar de manera efectiva esta coordinación.
* Se depende de un sistema de cifrado externo.

## Note
* Los ASC consideramos que la decisión debería ser aprobada.

## Links
