---
layout: post
title:  "Permutaciones, combinaciones y variaciones"
date:   2020-08-04 08:00:00 -0400
categories: Matematica Probabilidad 
---

## Combinatoria
Conocer la cantidad de formas de ordenar las cosas es importante para conocer las probabilidades de encontrarlas en ese orden o de lograr colocarlas en ese orden.

Y a las personas nos gusta ordenar las cosas porque así obtenemos información útil de ellas. 


### Permutaciones
Si hay una sola cosa, ya esta ordenada. No puede estar ni adelante, ni atrás, ni arriba, ni abajo, ni a la izquierda ni a la derecha de nada más.

Si hay dos cosas, si podemos colocar una a la izquierda de otra o a la derecha. Olvidemos por un momento que puede estar también arriba, abajo, adelante o atrás, para pder verlas solo con etiquetas de texto.

Asignemos el nombre o etiqueta "A" a una de las cosas y la etiqueta "B" a la otra cosa.

Tenemos entonces las probables formas de ordenar:

**AB**

**BA**

Bien, hasta ahora: una cosa, una forma de ordenar. Dos cosas, dos formas de ordenar. 

Si añadimos una tercera cosa con etiqueta "C" tenemos las probables formas de ordenar:

**ABC**

**ACB**

**BAC**

**BCA**

**CAB**

**CBA**

Ahora con tres cosas, tenemos seis formas de ordenar.

Si añadimos una cuarta cosa con etiqueta "D" tenemos:

**ABCD** **BACD** **CABD** **DABC**

**ABDC** **BADC** **CADB** **DACB**

**ACBD** **BCAD** **CBAD** **DBAC**

**ACDB** **BCDA** **CBDA** **DBCA**

**ADBC** **BDAC** **CDAB** **DCAB**

**ADCB** **BDCA** **CDBA** **DCBA**

Esto es 24 formas de ordenar.

Asi si vamos añadiendo una cosa en el orden: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, ...

Se va formando una sequencia de maneras de ordenar: 1,2, 6, 24, 120, 720, 5040, 40320, 362880, 3628800, ...

O lo que es lo mismo: 1, 1x2, 1x2x3, 1x2x3x4, 1x2x3x4x5, 1x2x3x4x5x6, ... , 1x2x3x4x5x6x7x8x9x10, ...

Así que la formas de ordenar cosas es igual a multiplicar todo hasta llegar al numero de cosas, operación matemática también conocida como factorial deun número,y para un número **n** se se escribe **n!** , yeah! un número que sorprende por lo rápido que pasamos de 1 a más de 3 millones en solo diez pasos.


### Combinaciones

Muchas de veces de todas las formas posibles de ordenar muchas cosas, solo necesitamos las que incluyen unas pocas. Por ejemplo, si tenemos en le bolsillo cuatro monedas: una de 5 centavos, una de 10 centavos, una de 50 centavos y otra de 1 dólar. ¿Cuánto podemos juntar sacando solo dos monedas del bolsillo?

Las formas de ordenar las cuatro monedas, si les pusieramos los nombres "A", "B","c" y "D" es fácil ver que son las 24 formas de antes.

Si sacamos dos, y no nos importa el orden entre las dos, tenemos como opciones:

**AB**, **BC**, **CD**, **AC**, **BD** y **AD**

Que vendrían siendo: 15 centavos, 60 centavos, 1.50 dólares, 55 centavos, 1.10 dólares, y 1.05 dólares.

En términos matemáticos existe una fórmula para obtener las combinaciones de **k** elementos de un conjunto de **n** elementos

${n}\choose{k}=\frac{n!}{k!(n-k)!} $

Si usamos con k igual 2 y n igual 4 nos da $\frac{24}{(2)(2)}=6$, que es lo que esperabamos.

#### Combinaciones, permutaciones y probabilidades.

Las combinaciones y permutaciones nos sirven bastante para obtener probabilidades. 

Por ejemplo: Si con nuestras cuatro monedas de antes, lo que queremos es sacar 60 centavos del bolsillo.

Entonces solo nos sirven la moneda de 10 centavos o moneda "B" y la de 50 centavos o moneda "C". Usemos de nuevo el concepto de orden, sacar dos monedas es similar a que sean las dos primeras en alguna de las formas de ordenar las cuatro. 

Así las formas que nos sirven son **BCAD**, **BCDA**, **CBAD** y **BCAD**. 

Solo 4 de las 24 formas nos sirven para sacar dos monedas antes o el esto es $4/24 \times 100= 16.66\%$ de probabilidades de obtener 60 centavos en un intento. 

Y de las combinaciones, 60 centavos es una de la 6 posibles, esto es $1/6 \time 100= 16.66\%$ de probabilidades.

Las permutaciones consideran el orden de los elementos, las combinaciones no, por eso existen más permutaciones que combinaciones. 

### Variaciones

Hasta ahora considerabamos que teníamos solo uno de cada uno de los elementos a los que dimos una etiqueta.

Pero cuando las etiquetas son números es muy común que tengamos un 1 o un 11. Que encontremos un 2, un 22 o un 222 en un grupo de números.

¿De cuántas formas se pueden ordenar el "0" y el "1", si se pueden repetir?

Tenemos:
**00**
**01**
**10**
**11**

Esto es cuatro formas de ordenarlos.

Si añadimos el 2 y permitimos que se repita tenemos;
**000** **001** **002** **010** **020** **011** **012** **021** **022**
**100** **101** **102** **110** **111** **112** **120** **121** **122**
**200** **201** **202** **210** **211** **212** **220** **221** **222**

Esto es 27 formas de ordenarlos.

Así, si tenemos esta cantidad de elementos: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10...

La cantidad de variaciones son: 1, 4, 27, 256, 3125, 46656, 823543, 16777216, 387420489, 10000000000

Esta secuencia en matemática se represnta como $n^n$ Wow! Si la serie anterior superaba en diez pasos los 3 millones, está llega a los  10 mil millones en los mismos diez paso.

Si 10 mil millones con solo 9 etiquetas, por eso los humanos nos pusimos de acuerdo en usar esta forma de asignar números a las cosas. Para ponerlo en otra perspectiva: Si contaramos un número cada segundo para llegar a 10 mil millones necesitamos casi 317 años (gracias a los años bisiestos o si no es más de 317 años).

¿La cantidad total de humanos cada vez se aproxima a esta cantidad, si dedicamos medio segundo para decir ¡Hola! a cada persona, necesitaríamos pasar toda nuestra vida saludando, incluso antes de aprender a hablar :o  

