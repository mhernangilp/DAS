# Selección-del-estilo

* Status: rejected
* Date: 2023-10-22

## Context and Problem Statement

Para desarrollar el software propuesto, consideramos que la mejor opción es adoptar un estilo basado en Modelo Vista Controlador.

## Decision Drivers

* RF1-Cambio de arquitectura
* RF2-Distintas conexiones de clientes
* RF4-Acceso vía HTTP/Rest

## Considered Options

* Modelo Vista Controlador
* REST
* Cliente-servidor

## Decision Outcome

Chosen option: "Modelo Vista Controlador", because consideramos que es el más acertado para este desarrollo según los argumentos previamente mencionados.

### Positive Consequences

* Permite un desarrollo eficaz de los requisitos propuestos

### Negative Consequences

* Puede ser más complejo que los otros estilos mencionados

## Pros and Cons of the Options

### Modelo Vista Controlador

Es un estilo versátil que nos permite cumplir con los requisitos de la aplicación.

* Good, because facilita la representación de los mismos datos en sistemas diferentes (Móvil y PC).
* Good, because ofrece mayor sencillez en el mantenimiento.
* Good, because permite una gran escalabilidad.
* Bad, because puede suponer una gran complejidad al principio del desarrollo
* Bad, because al distribuir más los componentes, provoca que haya que mantener más cantidad de ficheros.

### REST

Es un estilo que resuelve los problemas de la arquitectura, pero que no parece tan acertado como el Modelo Vista Controlador.

* Good, because permite la creación de la aplicación cumpliendo con los requisitos
* Bad, because obliga a desarrollar un servicio web

### Cliente-servidor

Un estilo muy parecido al rest, pero que nos parece menos adecuado para un sistema basado en microservicios

* Good, because permite el correcto desarrollo del software
* Bad, because puede no ser tan eficiente o acertado para los problemas que genera el desarrollo.
