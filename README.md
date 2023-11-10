# Estructura de Datos y Algoritmos I 23-24

### Repositorio de Juan René Ixcopal San José - Ingeniería Informática

## Temas vistos durante el curso

<<<<<<< HEAD
- [Estructuras de datos & conceptos fundamentales](001-intro/primitivasMatricesClasesObjetos.md)
- [Listas](002-listas/README.md)
  - Pilas
  - Colas
=======
- [Temario](temario/README.md)
- Evaluaciones
  - Evaluación continua: [Retos!](retos/README.md)
  - Examen parcial
  - Proyecto final 
>>>>>>> d11ae3393e7633c4c10230901d4df28f7c423781

## Temas extras

- [Programación genérica](/temario/999-otrosTemas/programacionGenerica.md)
- [Pruebas & manejo de errores](/temario/999-otrosTemas/pruebas.md)

# Retos realizados durante el curso

<details>
  <summary>Hoja de cálculo</summary>

<<<<<<< HEAD
  ### Hoja de cálculo

El reto consiste en desarrollar una hoja de cálculo en consola.

### Requisitos
| |
|-|
La hoja de cálculo debe ser de 15 filas por 10 columnas.
La navegación mediante **w**/**a**/**s**/**d**
Para ingresar un valor, se debe utilizar el comando **e**
Para terminar, utilizar el comando **q**
Las celdas deben tener un ancho de 7 caracteres. 
En caso que el usuario ingrese contenido de más de 7 caracteres, se deben mostrar los 7 primeros caracteres (ver presentación, estado intermedio.)

### Reglas de entrega

- Guardar el trabajo en la carpeta entregas, dentro una carpeta que siga el formato *nombreApellido*. Ejemplo: **/entregas/fernandezIbuprofeno**
- El envío debe hacerse al repositorio de la asignatura, a la rama ***Reto-001***

### Presentación
<div align="center">

| |
|:-:|
![](/imagenes/HojaDeCalculo000.png)
Estado inicial
![](/imagenes/HojaDeCalculo001.png)
Estado intermedio

</div>
</details>








<details>
  <summary>Hoja de cálculo orientado a objetos</summary>

  ### Hoja de cálculo en OOP

Partiendo de lo desarrollado en el reto anterior (esto es muy importante): reescribir el código siguiendo el paradigma orientado a objetos.

El reto consiste en reescribir el código, no en agregarle funcionalidad.

Se pueden hacer ajustes menores, pero la esencia debe mantenerse.

### Reglas de entrega

- Tener terminado el reto 001.
- Guardar el trabajo en la carpeta entregas, dentro una carpeta que siga el formato *apellidoNombre*. Ejemplo: **/entregas/fernandezIbuprofeno**
- El envío debe hacerse al repositorio de la asignatura, a la rama ***Reto-002***
</details>









<details>
  <summary>Variaciones sobre una lista simple</summary>

  ### Variaciones sobre una lista simple

  Partiendo del código de listas básicas revisado en clase, y publicado [aquí](/src/listas/basica/)

El reto consiste en agregar funcionalidad sin alterar la esencia del código.

||
|-|
Optimizar el proceso de saber cuántos elementos tiene la lista.
Para este caso concreto, hacer más descriptivo el proceso de entrada y salida de elementos (*entró xxx*, *salió yyy*).
Verificar que los cambios en las clases Node y List funcionan ejecutandolas a través de la clase Ejemplo.

## Reglas de entrega

- Tener resueltos ambos retos.
- Se exige código limpio.
- Se reciben entregas a la rama Reto-003 hasta las 23:59:59 del jueves 19 de octubre de 2023.

### Sugerencia de presentación

#### Presentación actual

```
LA FILA------------------
-------------------------
Esta vacia? true
Esta vacia? false
LA FILA------------------
Juanito
Pepito
Anita
-------------------------
Tamaño: 4
Tamaño: 3
LA FILA------------------
Juanito
Pepito
Anita
-------------------------
```

#### Presentación deseada

```
LA FILA------------------
-------------------------
Esta vacia? true
 > Llegó Juanito
 > Llegó Pepito
 > Llegó Anita
Esta vacia? false
LA FILA------------------
Juanito
Pepito
Anita
-------------------------
 > Llegó Luisito
Tamaño: 4
Se fue Luisito
Tamaño: 3
LA FILA------------------
Juanito
Pepito
Anita
-------------------------
┏[manuel]--[main ≡ ● ]
┖[~/misRepos/23-24-eda1]
```

</details>




<details>
  <summary>Variaciones sobre una lista simple V2</summary>

  ### Variaciones sobre una lista simple - Versión 2

Partiendo del código de listas básicas revisado en clase, publicado [aquí](/src/listas/basica/) y extendido en su último reto.

El reto consiste en agregar funcionalidad sin alterar la esencia del código.

||
|-|
Extender los métodos para agregar elementos, permitiendo agregar al inicio y al final.
Extender los métodos para eliminar elementos, permitiendo eliminar desde el inicio y desde el final.
Extender los métodos para agregar un i-ésimo elemento.
Extender los métodos para eliminar un i-ésimo elemento.
Verificar que los cambios en las clases Node y List funcionan ejecutandolas a través de la clase Ejemplo.

### Reglas de entrega

- Tener resueltos ambos retos.
- Se exige código limpio.
- Se reciben entregas a la rama Reto-004.
</details>




<details>
  <summary>Variaciones sobre una lista simple V2</summary>

  ### Reto CCCF

El centro comercial CF de El Alisal trabaja de 9 de la mañana a 9 de la noche vendiendo diversos artículos.

Un estudio previo determinó que la probabilidad de llegada de un cliente nuevo a la cola se estima en un 60% por minuto.

Para la gestión de la venta dispone de 4 cajas que van atendiendo a los clientes, que a su vez van situándose en fila conforme concluyen sus compras esperando una caja vacía que les atienda.

Cuando una caja está libre (es decir, no está atendiendo a ningún cliente), puede recibir a un nuevo cliente de la cola. Este cliente llevará su compra, la cual el estudio anteriormente citado midió en **packs de items**.

El usuario puede llevar un mínimo de 5 y un máximo de 15 pack de items para su atención.

Se tiene calculado que las cajas tardan 1 minuto en atender un pack de items.

|Escenario
|-|
|![](/imagenes/retoCCCF.png)

Desarrolle un programa que modele y simule el sistema explicado líneas arriba, teniendo en cuenta las condiciones indicadas.

### Reto base

Este programa debe ir mostrando los siguientes datos conforme avance el tiempo:

* Llegada de las personas
* Número de personas en cola
* El estado de atención de las cajas.

### Reto extendido

Extienda el programa anterior para que, al finalizar la jornada, presente un resumen con los siguientes datos:

* Número de minutos en que no hubo nadie en cola.
* Número de personas que estaban en cola al finalizar el día.
* Número de personas atendidas durante el día.
* Número de items vendidos en el día.

### Reto ampliado

Extienda el programa anterior para que soporte los siguientes supuestos:

* En caso que haya más de 15 personas en cola, agregue una persona más en caja, que atienda como mínimo a 5 personas (o mientras hayan más de 15 personas en cola).
* Agregue el rol de superadministrador del sistema, que permita encender o apagar cajas (suponga que puede gestionar hasta 6 cajas).

> Nota: Debido a su complejidad, se sugiere que los retos ampliados se resuelvan uno a la vez y que, dominados los conceptos, se integren en una única solución.

### Sugerencia de presentación

```bash
manuel@manuel-OptiPlex-7020:~/Documentos/miJava$ java TestParcial
MINUTO 1 - Llega 1 persona - En Cola: 0
Caja1:[13] | Caja2:[0] | Caja3:[0] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 2 - No llega nadie  - En Cola: 0
Caja1:[12] | Caja2:[0] | Caja3:[0] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 3 - Llega 1 persona - En Cola: 0
Caja1:[11] | Caja2:[6] | Caja3:[0] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 4 - Llega 1 persona - En Cola: 0
Caja1:[10] | Caja2:[5] | Caja3:[4] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 5 - No llega nadie  - En Cola: 0
Caja1:[9] | Caja2:[4] | Caja3:[3] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 6 - Llega 1 persona - En Cola: 0
Caja1:[8] | Caja2:[3] | Caja3:[2] | Caja4:[4]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 7 - Llega 1 persona - En Cola: 1
Caja1:[7] | Caja2:[2] | Caja3:[1] | Caja4:[3]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 8 - No llega nadie  - En Cola: 1
Caja1:[6] | Caja2:[1] | Caja3:[0] | Caja4:[2]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 9 - Llega 1 persona - En Cola: 1
Caja1:[5] | Caja2:[0] | Caja3:[7] | Caja4:[1]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 10 - No llega nadie  - En Cola: 0
Caja1:[4] | Caja2:[6] | Caja3:[6] | Caja4:[0]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 11 - Llega 1 persona - En Cola: 0
Caja1:[3] | Caja2:[5] | Caja3:[5] | Caja4:[4]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 12 - Llega 1 persona - En Cola: 1
Caja1:[2] | Caja2:[4] | Caja3:[4] | Caja4:[3]
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
MINUTO 720 - No llega nadie  - En Cola: 7
Caja1:[1] | Caja2:[4] | Caja3:[4] | Caja4:[2]
- - - - - - - - - - - - - - - - - - - - - - - - - - - -
RESUMEN
============================================================
Minutos con cola en cero  	  : 216
Personas en la cola al cierre : 7
Personas atendidas en el dia  : 295
Articulos vendidos en el dia  : 2684
============================================================
```


### Reglas

- Puede reutilizar el código que hizo en su momento. O no...
- El lenguaje de programación para desarrollarlo es libre. Lo mismo con el paradigma (estructurado u orientado a objetos).
- Se **exige** código limpio.
- Se reciben entregas a la rama Reto-005.
- Entregas hasta el lunes 6 a las 23:59:59
</details>

# Solucion a los retos

- Reto 1 [SOLUCIÓN](https://github.com/juanixcopal/23-24-eda1/tree/main/entregas/juanIxcopal/Reto-001)
- Reto 2 [SOLUCIÓN](https://github.com/juanixcopal/23-24-eda1/tree/main/entregas/juanIxcopal/Reto-002)
- Reto 3 [SOLUCION](https://github.com/juanixcopal/23-24-eda1/tree/main/entregas/juanIxcopal/Reto-003)
- Reto 4 [SOLUCIÓN](https://github.com/juanixcopal/23-24-eda1/tree/main/entregas/juanIxcopal/Reto-004)
- Reto 5 [SOLUCIÓN](https://github.com/juanixcopal/23-24-eda1/tree/main/entregas/juanIxcopal/Reto-005)
=======
- [Hoja de asistencia de la asignatura](https://docs.google.com/spreadsheets/d/18jzNDeHckYg1bWRV4mEz9wdfirxPORikC-jv-pcYt2U/edit?usp=sharing)
- [Libro de la asignatura](https://campus.uneatlantico.es/pluginfile.php/81026/mod_folder/content/0/Estructuras%20de%20datos%20y%20algoritmos%20I.pdf?forcedownload=1)
- [Diferencia entre ciencias de la computación e ingenieria de software](https://interestingengineering.com/culture/computer-science-vs-software-engineering-how-are-they-different)

### En mi máquina funciona...

#### Mac OS
```bash
┏[manuel]
┖[~/misRepos]
   java --version
java 20.0.2 2023-07-18
Java(TM) SE Runtime Environment (build 20.0.2+9-78)
Java HotSpot(TM) 64-Bit Server VM (build 20.0.2+9-78, mixed mode, sharing)
```

#### KUbuntu
```bash
┏[manuel]
┖[~/misRepos]
   java --version
openjdk 17.0.8.1 2023-08-24
OpenJDK Runtime Environment (build 17.0.8.1+1-Ubuntu-0ubuntu123.04)
OpenJDK 64-Bit Server VM (build 17.0.8.1+1-Ubuntu-0ubuntu123.04, mixed mode, sharing)
```
>>>>>>> d11ae3393e7633c4c10230901d4df28f7c423781
