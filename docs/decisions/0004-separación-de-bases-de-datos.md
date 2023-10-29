# Separación-de-bases-de-datos

* Status: proposed
* Date: 2023-10-29

## Context and Problem Statement

El sistema debe tener los datos separados en dos bases de datos diferentes, una de "Clientes" y otra de "Pedidos".

## Decision Drivers

* RF3-Acceso a clientes y pedidos

## Considered Options

* Patrón Base de datos por servicio
* Diseñar un modelo propio

## Decision Outcome

Chosen option: "Patrón Base de datos por servicio", because se debe mantener una separación de las bases de datos.

### Positive Consequences

* descentraliza las bases de datos.

### Negative Consequences

* se deben tener en cuenta los errores

## Pros and Cons of the Options

### Patrón Base de datos por servicio

Este patrón permite que los distintos microservicios tengan su propio almacenamiento de datos.

* Good, because permite solucionar el problema de diseño, teniendo dos bases de datos independnientes.
* Bad, because necesita protección ante los fallos en caso de que haya algún problema en la comunicación.

### Diseñar un modelo propio

Diseñar una interfaz propia para el uso de estas dos bases de datos.

* Good, because permite personalizar sus funciones con respecto a las necesidades.
* Bad, because es más correcto utilizar un patrón de diseño que ya está probado.
