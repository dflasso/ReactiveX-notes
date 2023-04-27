# Introducción

## ¿Por qué usar extensciones reactivas?
todos queremos manejar información en tiempo real

## ¿Cuando usar RX?
- Manejar cualquier evento de la interfaz de usuario
- Cuando es necesario notificar sobre cambios en un objeto(s)
- Comunicaciones por sockets.
- Cuando necesitamos trabajar con flujos de información (Streams)

## Piezas

### Observables
- Son la fuente de información
- Pueden emitir multiples valores, sólo uno o ninguno.
- Pueden emitir errores
- Pueden ser infinitos, finitos (completarse)
- Pueden ser síncronos o asíncronos

### Subscribers
- Se subscriben a un observable, es decir, estar pendiente de lo que realiza el observable.
- Consumen / observan la data del observable.
- Pueden recibir los errores y eventos del observable
- Desconocen todo lo que se encuentra detrás del observable


### Operatorss
- Usados para transformar Observables (map, group, scan, ...)
- Usados para filtrar observables (filter, distinct, skip, debounce, ...)
- Usados para combinar observables
- Usados para crear nuevos observables 

## Beneficios
1. Evitar el Callback hell
2. Trabajar de forma simple tareas sincrónicas y asíncronas.
3. Uso de operadores para reducir y simplificar el trabajo.
4. Es fácil transformar los flujos (streams) de información
5. Código más limpio y fácil de leer.
6. Fácil de implementar
7. Fácil anexar procedimientos sin alterar el producto final.  

# ¿Qué es ReactiveX?

Según el sitio oficial, es la mejor combinación del patrón observer, iterador y la programación funcional.

## Patrón observer

Es un patrón de diseño de software que define una dependencia del tipo uno a muchos entre objetos, de manera que cuando uno de los objetos cambia su estado, notifica este cambio a todos los dependientes.

- primero() -> first()
- siguiente() -> next()
- hayMas() 
- elementoActual() -> currentElement()

## Patrón iterador

Implementar todas las funciones para ejecutar operaciones secuenciales

## Programación funcional
 

# Diagramas de canicas

- un observable debe terminar con símbolo $ (buena práctica),  de la siguiente manera: clicks$
- Cada circulo representa un valor emitido por el observable