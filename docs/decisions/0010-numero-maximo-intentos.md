# Numero-maximo-intentos

* Status: accepted
* Date: 2023-11-09

## Context and Problem Statement

El usuario debe tener un número limitado de intentos a la hora de realizar un pedido.

## Decision Drivers

* RF9-Limitación de intentos de pedido

## Considered Options

* Patrón circuit breaker

## Decision Outcome

Chosen option: "Patrón circuit breaker", because permite establecer un número máximo de intentos a la hora de realizar un pedido, solucionando el problema de diseño.

### Positive Consequences

* Evita saturaciones del servidor.

## Pros and Cons of the Options

### Patrón circuit breaker

Este patrón evita que un objeto intente reiteradamente una operación o solicitud que tiene alta probabilidad de fallo.

* Good, because previene fallos de conexión.
* Good, because almacena las peticiones fallidas para que las pueda revisar un administrador
* Bad, because puede generar falsas alarmas y provocar que el sistema falle.
