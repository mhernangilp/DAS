# Reelección-del-estilo

* Status: accepted
* Date: 2023-10-25

## Context and Problem Statement

Hemos invalidado la decisión 0001-selección-del-estilo debido a que el estilo cliente servidor se adapta mejor a la arquitectura a diseñar, pues presenta una serie de ventajas respecto al MVC.

## Decision Drivers

* RF1-Cambio de arquitectura
* RF2-Distintas conexiones de clientes
* RF4-Acceso vía HTTP/Rest

## Considered Options

* Estilo cliente servidor
* Modelo vista controlador

## Decision Outcome

Chosen option: "Estilo cliente servidor", because es un estilo que se adapta mejor a los requisitos del software que queremos diseñar.

### Positive Consequences

* Ahora tenemos un estilo más acertado que nos va a permitir diseñar la arquitectura más adecuadamente.

## Pros and Cons of the Options

### Estilo cliente servidor

Es un estilo arquitectónico que nos permite cómodamente diseñar de manera separada la parte de los microservicios y la parte de interacción con el usuario.

* Good, because La parte cliente está separada de la parte servidor, por lo tanto es compatible con diferentes plataformas y sistemas operativos.
* Good, because Permite la distribución de tareas entre los servidores.

### Modelo vista controlador

Es el estilo que elegimos anteriormente.

* Good, because Al separar la parte vista y controlador del modelo, parecía la mejor opción para nuestro software.
* Bad, because Está pensado para sistemas altamente interactivos.
