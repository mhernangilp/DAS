# Acceso-diferentes-plataformas

* Status: accepted
* Date: 2023-10-29

## Context and Problem Statement

El sistema requiere que los usuarios puedan acceder desde el ordenador o desde el móvil, por lo tanto, se ha de encontrar un patrón de diseño que nos lo permita.

## Decision Drivers

* RF2-Distintas conexiones de clientes
* RF4-Acceso vía HTTP/Rest

## Considered Options

* Patrón Facade
* Patrón API Gateway

## Decision Outcome

Chosen option: "Patrón API Gateway", because es una mejor solución para nuestro problema.

### Positive Consequences

* permite el acceso a clientes desde diferentes plataformas.

### Negative Consequences

* debe estar implementado correctamente debido a que afecta a directamente al funcionamiento del sistema.

## Pros and Cons of the Options

### Patrón Facade

Provee de una interfaz unificada para acceder a una interfaz de un subsistema.

* Good, because podría solucionar el problema de diseño.
* Bad, because se adapta más a un sistema monolítico.

### Patrón API Gateway

Proporciona un punto de entrada único a una estructura de microservicios, ocultando la complejidad y las interacciones entre ellos.

* Good, because todas las solicitudas, incluidas las que usan el protocolo HTTP/Rest pasan por el gateway antes de ser dirigidas al microservicio correspondiente.
* Good, because nos permite separar el acceso de los clientes, sin aumentar la complejidad.
* Bad, because si no se diseña de forma adecuada, todas las solicitudes desde, y hacia los microservicios pueden verse afectadas
