# actividad 2
![link de ayudas](./image/Captura%20de%20pantalla%202025-07-31%20104545.png)

# ejercicio 2

Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.

## solucion

```
Inicio
Leer ID, S1, S2, S3, S4, S5, S6
Total = S1 + S2 + S3 + S4 + S5 + S6
Promedio = Total / 6
Escribir ID, Total, Promedio
Fin
```
![link imagen de diagrama](./image/Diagrama%20sueldos%20julian.drawio.png)



# tarea

```
leer N1, N2, N3, N4, N5, N6, N7

```

# CLASE MARTES 5 DE AGOSTO
# ejercicio 3

Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

| variables | tipo | comentario|
|-----------|------| -------|
| lapices   | entrada| cantidad de lapices|
|valor unidad | intermedia| valor intermedio de cada lapiz|
| precio    | salida|precio total de los lapices|
|85 , 90 | constantes|no cambian|
## pseudocodigo
```
inicio 
leer lapices 
si lapices >= 1000:
    valor_unidad = 85
Si no 
    valor_unidad = 90
Fin si 
Precio = lapices * valor_unidad
Escribir "el valor total es:", precio
Fin
```
![link imagen de diagrama de flujo](./image/ejercicio%203.png)


# ejercicio 4
Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

| variables | tipo | comentario|
|-----------|------| -------|
| total_compra| entrada| valor de la compra |
|descuento |salida | valor a pagar|
|precio final | salida | valor a pagar |
| 15% , 8% , $250000| constante | descuento y valor limite|
## peseudocodigo
```
inicio 
leer total_compra 
si total_compra > 250000:
    descuento = total_compra * 0.15
si no 
    descuento = total_compra * 0.08
fin si 
precio_final = total_compra - descuento 
escribir "valor a pagar:" , precio_final 
fin
```


# ejercicio 5 
El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

| variables | tipo | comentario|
|-----------|------| -------|
| alumnos | entrada | numero de alumnos que van al viaje |
|costo_alumno , Precio_total| salida | precio por alumno que va y la suma todal de ellos |
|$65.00 , $70.00 , $95.00 , $4000.00 | constante | valor dependiendo del numero de alumnos |
|alumnos >=100 ,50 a 99 alumnos , 30 a 49 alumnos , alumnos < 30 | rango ||
## pseudocodigo
```
inicio 
leer alumnos 
si alumnos >= 100:
    costo_alumnos = 65
si no 
    si alumnos >= 50 
        costo_alumnos = 70
    si no 
        si alumnos >= 30 
            costo_alumnos = 95
        si no 
            costo_total = 4000
            costo_alumnos = costo_total/alumnos 
        fin si 
    fin si 
fin si 
costo_total = costo_alumnos * alumnos 
escribir: costo_total , costo_alumnos
fin 
``` 


# TAREA
averiguar cunatos años tiene una persona con su dia mes y año a la fecha actual 

| variables | tipo | comentario|
|-----------|------| -------|
|fecha_nacimiento, fecha_actual|entrada| dia mes y año|
|12 meses= un año, 1~31 dias= mes | rango| tener en cuenta para saber si esta adecuadamente los años|
|años| salida | resta de la fecha_nacimiento y fecha_atual|
## peseudocodigo

```
inicio 
leer año_nacimiento, mes_nacimiento, dia_nacimiento
leer año_actual, mes_actual, dia_actual
años = año_actual - año_nacimiento
si mes_nacimiento < mes_actual
    años
si no 
    si mes_nacimiento = mes_actual
        si dia_nacimiento <= dia_actual
            años 
        si no 
            años = años - 1
        fin si
    si no 
        años = años - 1
    fin si 
fin si 
escrbir: "su edad es", años
fin
```

![link a tarea](./image/tarea%202.drawio.png)

# ejercicios de bucles 

## ejercicio 1

se requiere un algotitmo para determinar, N cantidades cuantas son cero, cuantas son menores a cero, cuantas son iguales a cero y uantas son mayores a cero 
realice un diagrama de flujo y pseudocodigo representarlo y utilizando el coclo apropiado.

```
inicio 
leer N
ceros = 0
mayores = 0
menores = 0

mientras N > 0 :
    leer cant
    si cant > 0 : 
        mayores = mayores + 1 
    si no 
        si cant = 0:
            ceros = ceros + 1
        si no 
            menores = menores + 1
        fin si 
    fin si 
    N = N - 1
fin mientras
mostras ceros, mayores, menores 
fin
```

## ejercicio 2
calcular el factorialde un numero entero ingresado por el usuario.

```
inicio 
leer N 
fact = 1 
mientras N > 0 
    fact = fact * N
    N = N - 1 
fin mientras 
mostrar fact
fin
```



