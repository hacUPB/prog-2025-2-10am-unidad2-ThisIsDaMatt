```
Desde i = 0 hasta 4
    Mostrar Edades [i]

Desde i = 0 hasta i = 9
    Leer Dato
    Edades[1] = Dato
Fin Desde
```
# Taller de Algoritmos

## Ejercicios con Condicionales

### Verificación de peso de despegue

En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.

### Analisis

Variables de entrada: CantidadCombustible, CantidadCarga
Variables de control: MTOW, PesoVacio
Variables de salida: PesoTotal

### Pseudocodigo

```
Inicio
MTOW = 78000
PesoVacio = 42600
Leer CantidadCombustible
Leer CantidadCarga
PesoTotal = PesoVacio + CantidadCombustible + CantidadCarga
Si PesoTotal <= MTOW
    Mostrar "La aeronave es apta para despegar"
Si no
    Mostrar "La aeronave excede el peso maximo de despegue"
Fin Si
Fin
```

## Ejercicios con Bucles

### Registro de altitudes de vuelo

Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.

### Analisis

Variables de entrada: Altitud
Variables de control: i
Variables de salida: Mediciones

### Pseudocodigo

```
Inicio
i = 0
Mientras i < 6
    Leer Altitud
    Mediciones[i] = Altitud
    i = i + 1
Fin Mientras
Mostrar Mediciones
Fin
```

## Ejercicios con Bucles y Condicionales

### Planificación de misión satelital

Desarrollar un algoritmo que reciba datos de consumo de energía por hora de un satélite durante un día completo. Si en cualquier hora el consumo excede un límite crítico, debe registrarse como una alerta. Al final, mostrar el consumo total y el número de alertas generadas.

### Analisis

Variables de entrada: ConsumoEnergia
Variables de control: i, LimiteCritico
Variables de salida: ConsumoTotal, NumeroAlertas

### Pseudocodigo

```
Inicio
i = 0
ConsumoTotal = 0
NumeroAlertas = 0
LimiteCritico = 50
Mientras i < 24
    Leer ConsumoEnergia
    ConsumoTotal = ConsumoTotal + ConsumoEnergia
    Si ConsumoEnergia > LimiteCritico
        NumeroAlertas = NumeroAlertas + 1
    Fin si
    i = i + 1
Fin Mientras
Mostrar ConsumoTotal
Mostrar NumeroAlertas
Fin



        




    

