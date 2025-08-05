# Simbolos usados en Diagramas de Flujo

1) **Ovalado**: Representa el inicio o el fin de un algoritmo
2) **Rectangulo**: Indica una tarea o proceso especifico dentro del proceso
3) **Diamante**: Indica un punto de decision, normalmente con opciones si/no
4) **Paralelogramo**: Muestra los datos que entran o salen del sistema
5) **Flecha**: Indica la direccion del flujo entre simbolos
6) **Simbolo de documento**: Para ilustrar como se crean. revisan o utilizan los documentos del proceso
7) **Simbolo de bases de datos**: Indica los procesos que implican la recuperación o almacenamiento de datos
8) **Simbolo de entrada manual**: Resalta las interacciones del usuario que requieren introduccion de datos

[Link a la pagina usada](https://clickup.com/es-ES/blog/214499/simbolos-del-diagrama-de-flujo)

![Imagen descriptiva](/images/diagrama-de-flujo.png)

# Ejercicio 2

Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.

## Solución

### Pseudocodigo

```
Inicio
Leer ID, S1, S2, S3, S4, S5, S6
Total = S1 + S2 + S3 + S4 + S5 + S6
Promedio = Total / 6
Escribir ID, Total, Promedio
Fin
```

### Diagrama de Flujo

![Ejercicio2](/images/Ejercicio2.png)

# Ejercicio 3

Un curso se evalua con 7 notas, conoce 6 notas, las cuales valen el 70% del curso. Se le pide al usuario las primeras 6 notas, y se calcula cuanto debe sacar en la evaluación final para aprobar, minimo, con 3.0.

## Solución

### Analisis

Variables de entrada: N1, N2, N3, N4, N5, N6
Proceso: Calcular Promedio de N1 a N6, restar 3.0 del Promedio x 0.7 y dividirlo por 0.3
Variables de Salida: Promedio de N1 a N6 y Nota Final

### Pseudocodigo

```
Inicio
Leer N1, N2, N3, N4, N5, N6
Promedio = (S1 + S2 + S3 + S4 + S5 + S6) / 6
Nota final = 3.0 - (Promedio x 0.7) / 0.3
Si Promedio > 3.0, Aprobar
Sino, Reprobar
Escribir Promedio, Nota Final, Aprueba o no Aprueba
Fin
```

### Diagrama de Flujo

![Ejercicio3](/images/Ejercicio3.png)

# Ejercicio 4

Realice un algoritmo para determinar cuanto se debe pagar por equis cantidad de lapices considerando que si son 1000 o mas el costo es de $85 cada uno; de lo contrario, el precio es de $90.

## Solucion

### Analisis

Variables de entrada: Cantidad de Lapices

Variable intermedia: Valor unidad

Proceso: Contar cantidad y aplicar precio

Variables de Salida: Cantidad de Lapices, Precio

### Pseudocodigo

```
Inicio
Leer Cantidad_Lapices
Si Cantidad_Lapices >= 1000
    Valor_Unidad = 85
Si no
    Valor_Unidad = 90
Fin si
Costo = Cantidad_Lapices x Valor_Unidad
Escribir "El valor total es:", Costo
Fin
```

### Diagrama de Flujo

![Ejercicio4](/images/Ejercicio4.png)

# Ejercicio 5

Un almacen de compra tiene una promocion: por compras superiores a $250000 se les aplicará un descuento del 15%, de caso contrario, solo se aplicará un 8%. Realice un algoritmo para determinar el precio final que debe pagar una personapor comprar en dicho almacén y de cuanto es el decuento que obtendrá.

## Solucion

### Analisis

Variables de entrada: Valor de compra

Proceso: Aplicar descuento segun aplica

Variable de salida: Valor con descuento

### Pseudocodigo

```
Inicio
Leer Valor_Compra
Si Valor_Compra > 250000
Valor_final = Valor_Compra x 0.85
Sino, Valor_Final = Valor_Compra x 0.92
Escribir Valor_Final
Fin
```

### Diagrama de flujo

![Ejercicio5](/images/Ejercicio5.png)

# Ejercicio 6

El director de una escuela esta organizndo un viaje de estudios, y requiere determinar cuanto debe cobrar a cada alumno y cuanto debe pagar a la compañia de viajes por el servivio. La forma de cobrar es la siguiente: Si son 100 alumnos o mas, el costo de cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de renta del autobus es de $4000.00, sin importar el numero de alumnos.

## Solucion

### Analisis

Variables de entrada: Cantidad de Alumnos

Proceso: Aplicar el costo de cada alumno segun la cantidad

Variable de salida: Costo de renta

### Pseudocodigo

```
Inicio
Leer Cantidad_Alumnos
Si Cantidad_Alumnos >= 100
Costo_Renta = Cantidad_Alumnos x 65
O, Si Cantidad_Alumnos 50-99
Costo_Renta = Cantidad_Alumnos x 70
O, Si Cantidad_Alumnos 30-49
Costo_Renta = Cantidad_Alumnos x 95
Sino, Costo_Renta = 4000
Escribir Costo_Renta
Fin
```

### Diagrama de flujo

![Ejercicio6](/images/Ejercicio6.png)
