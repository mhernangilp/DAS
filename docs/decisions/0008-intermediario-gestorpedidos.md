# Intermediario-gestorpedidos

* Status: accepted
* Date: 2023-11-04

## Context and Problem Statement

Existe un componente denominado GestorPedidos que hace de intermediario entre los clientes, pedidos, el reparto y las incidencias comunicando dichas funcionalidades. Se debe encontrar un patrón que solucione este problema de diseño.

## Decision Drivers

* RF7-Intermediario GestorPedidos

## Considered Options

* Patrón Mediator
* Patrón Chain of Respoinsibility

## Decision Outcome

Chosen option: "Patrón Mediator", because se adecúa más al requisito.

### Positive Consequences

* Permite centralizar las relaciones entre las clases.

### Negative Consequences

* No permite la comunicación secuencial entre las clases pertinentes.

## Pros and Cons of the Options

### Patrón Mediator

Elimina las conexiones directas entre emisores y receptores, forzándolos a comunicarse a través de un objeto intermediario.

* Good, because Permite reducir las dependencias caóticas entre objetos.
* Good, because Restringe las comunicaciones entre objetos.
* Bad, because Puede ser complicado definir sus responsabilidades y las de las clases que maneja.
* Bad, because Si no se diseña correctamente, puede acabar siendo un módulo demasiado grande.

### Patrón Chain of Respoinsibility

Permite pasar solicitudes a lo largo de una cadena de manejadores.

* Good, because Permitiría la comunicación secuencial entre las clases cliente, pedido, reparto e incidencias.
* Bad, because No haría de intermediario entre las clases.
