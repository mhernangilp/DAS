# Selección-de-algoritmos

* Status: accepted
* Date: 2023-11-02

## Context and Problem Statement

El sistema debe contar con dos algoritmos de optimización que se seleccionan en función de la demora del camión. Para ello, se debe utilizar un patrón de diseño que facilite su implementación.

## Decision Drivers

* RF5-Selección de algoritmo

## Considered Options

* Patrón de diseño Strategy
* Patrón de diseño State

## Decision Outcome

Chosen option: "Patrón de diseño Strategy", because se adapta mejor a nuestro problema de diseño.

### Positive Consequences

* Queda solucionado el problema de diseño.

## Pros and Cons of the Options

### Patrón de diseño Strategy

Es un patrón de comportamiento que permite encapsular varios métodos o algoritmos y hacerlos intercambiables.

* Good, because Permite intercambiar los algoritmos en tiempo de ejecución, por lo tanto podría cambiar según la demora del camión en nuestro caso.
* Bad, because Puede aumentar la complejidad del código.
* Bad, because Puede provocar duplicidad de código

### Patrón de diseño State

Permite que un objeto modifique su comportamiento dependiendo de su estado interno

* Good, because Es parecido al patrón strategy, permite modificar el comportamiento de una clase, lo cual puede ser útil para nuestro sistema.
* Bad, because Está pensado para que cambie el comportamiento cuando cambia el estado interno del objeto.
