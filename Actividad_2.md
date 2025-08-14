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
Nota final = 3.0 - (Promedio * 0.7) / 0.3
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
Costo = Cantidad_Lapices * Valor_Unidad
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

Variable de salida: Descuento, Valor Final

### Pseudocodigo

```
Inicio
Leer Valor_Compra
Si Valor_Compra > 250000
    Descuento = Valor_Compra * 0.15
Si no
    Descuento = Valor_Compra * 0.08
Fin si
Valor_Total = Valor_Compra - Descuento
Escribir "Valor a pagar:", Valor_Total
Fin
```

### Diagrama de flujo

![Ejercicio5](/images/Ejercicio5.png)

# Ejercicio 6

El director de una escuela esta organizndo un viaje de estudios, y requiere determinar cuanto debe cobrar a cada alumno y cuanto debe pagar a la compañia de viajes por el servivio. La forma de cobrar es la siguiente: Si son 100 alumnos o mas, el costo de cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de renta del autobus es de $4000.00, sin importar el numero de alumnos.

## Solucion

### Analisis

Variables de entrada: Alumnos

Proceso: Aplicar el costo de cada alumno segun la cantidad

Variable de salida: Costo de Alumno, Costo Total

### Pseudocodigo

```
Inicio
Leer Alumnos
Si Alumnos >= 100
    Costo_Alumno = 65
Si no 
    Si Alumnos >= 50
        Costo_Alumno = 70
    Si no
        Costo_Alumno = 90
    Fin si
Fin si 

```

### Diagrama de flujo

![Ejercicio6](/images/Ejercicio6.png)

# Ejercicio de Tarea

### Pseudocodigo

```
Inicio
Leer dia_nacimiento, mes_nacimiento, año_nacimiento, dia_actual, mes_actual, año_actual
Si dia_actual < dia_nacimiento
    dia_actual = dia_actual + 30
    mes_actual = mes_actual - 1
Fin Si
dias = dia_actual - dia_nacimiento
Si mes_actual < mes_nacimiento
    mes_actual = mes_actual + 12
    año_actual = año_actual - 1
Fin Si
meses = mes_actual - mes_nacimiento
años = año_actual - año_nacimiento
dias_vividos = (años * 365) + (meses * 30) + dias
Escribir "Edad: ", años, " años, ", meses, " meses, ", dias, " días"
Escribir "Has vivido: ", dias_vividos, " días"
Si dia_nacimiento = dia_actual Y mes_nacimiento = mes_actual Entonces
    Escribir "¡Feliz cumpleaños!"
Fin Si
Fin
```

# Bucles y ciclos

Un **bucle** en programación es una estructura de control que permite **ejecutar repetidamente** un bloque de código mientras se cumple una condición específica o durante un número determinado de iteraciones. Son fundamentales para **automatizar** tareas repetitivas, realizar cálculos iterativos y procesar grandes conjuntos de datos.

En **Python** existe **for** y **while**, mientras que en otros lenguajes, como **C++** puede existir tambien un **do-while**.

# Ejercicio 1

Se requiere un algoritmo para determinar, de N cantidades, cuantas son cero, cuantas son menores a cero y cuantas son mayores a cero.
Realice el diagrama de flujo y el pseudocodigo, representarlo, usando el flujo apropiado.

## Solución

### Analisis

Variable de entrada: N, Cantidad

Variables de salida: Ceros, Mayores, Menores (contador)

Control: N

### Pseudocodigo

```
Inicio
Leer N
Ceros = 0
Mayores = 0
Menores = 0
Mientras N > 0:
    Leer Cantidad
    Si Cantidad > 0:
        Mayores = Mayores + 1
    Si no
        Si Cantidad = 0:
            Ceros = Ceros + 1
        Si no
            Menores = Menores + 1
        Fin Si
    Fin Si
    N = N - 1
Fin Mientras
Mostrar Ceros, Mayores, Menores
Fin
```
### Diagrama de Flujo

![EjercicioBucle1](/images/EjercicioBucle1.png)

# Ejercicio 2

Calcular el factorial de un numero entero ingresado por el usuario.

## Solución (propia)

### Analisis

Variables de entrada: N

Variables de salida: Resultado

Variables de control: i, Factorial

### Pseudocodigo

```
Inicio
Leer N
Si N <= 0
    Escribir "No definido"
Fin si
Factorial = 1
i = 1
Mientras i <= N
    Factorial = Factorial * i
    i = i + 1
Fin Mientras
Mostrar Resultado
Fin
```
## Solución (profesor)

Variables de entrada: N

Variables de salida: Factorial

Variables de control: i / N

# Tarea

Consultar como funcionan las tarjetas de credito. Asumir una tasa de interes fija (2%). Preguntar al usuario el valor de la compra y el numero de cuotas. Calcular y mostrar en pantalla el valor de cada una de las cuotas que debe pagar hasta saldar la deuda.

## Solucion

### Analisis

Variables de entrada: ValorCompra, NumeroCuotas, Tasa

Variables de salida: CuotaMensual

Variables de control: i

### Pseudocodigo

```
Inicio
Tasa = 0.02
Leer ValorCompra
Leer NumeroCuotas
InteresTotal = ValorCompra * Tasa * NumeroCuotas
MontoTotal = ValorCompra + InteresTotal
CuotaMensual = MontoTotal / NumeroCuotas
Para i desde 1 hasta NumeroCuotas
    Mostrar "Cuota", i, ": $", CuotaMensual
Fin Para
Mostrar "Valor inicial: $", ValorCompra
Mostrar "Interés total: $", InteresTotal
Mostrar "Total a pagar: $", MontoTotal
Fin
```
