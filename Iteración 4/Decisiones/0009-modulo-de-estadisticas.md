# Modulo-de-estadisticas

* Status: accepted
* Date: 2023-11-09

## Context and Problem Statement

El sistema cuenta con un módulo de estadísticas que proporciona información valiosa sobre el estado de los pedidos y la situación en tiempo real de los camiones.

## Decision Drivers

* RF8-Módulos de estadísticas

## Considered Options

* Patrón Observer

## Decision Outcome

Chosen option: "Patrón Observer", because permite resolver el problema de diseño de forma adecuada, notificando a los módulos de estadísticas cuando cambia algo en los objetos observados.

## Pros and Cons of the Options

### Patrón Observer

Es un patrón de comportamiento que notifica a un objeto cuando ocurre un evento en el objeto que está observando.

* Good, because permite actualizar los módulos de estadísticas cuando ocurre un evento en los pedidos o repartos.
* Bad, because avisa a los objetos suscriptores en un orden aleatorio una vez que sucede un evento.
