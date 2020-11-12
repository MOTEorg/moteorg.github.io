---
layout: post
title:  "Medidas de Información"
date:   2020-08-05 10:00:00 -0400
categories: Matematica Probabilidad 
---

### Probabilidad

Muchas veces expresado solo como un porcentaje se pierde todo lo que ese porcentaje informa.

Un porcentaje de probabilidad va del 0% al 100% o lo que es lo mismo de 0 a 1, si dividimos para cien.

Dar un dato en porcentaje es la forma más simple de informar. Qué oración te dice más:

"Quedan 10 helados en la nevera"

o

"Quedan el 50% de helados en la nevera" 

La segunda oración tiene más información. Si bien ese 50% puede ser 1, 2 o 100 helados, te dice algo sobre la nevera: que se puede llenar con más helados.

Claro, si lo que interesa es repartir los helados o calcular su precio, puede ser que falte la información de cuánto es el 100%. Asi que la primera oración es más útil.

Y quedemonos con estas dos características que puede tener un dato: Utilidad e informatividad.

#### Distribuciones de Probabilidad

Pero además de cuánto es el 100%, otra cosa que interesa es como se llega del 0 al 100%.

La forma más común de ir de 0% a 100% en la naturaleza es en forma de lo que se conoce como función error, que se parece a una S mayúscula alargada.

Esta curva es díficil de calcular, pero se puede usar una forma muy parecida que se llama sigmoide, mucho más fácil de calcular, o una intermedia pero más conocida como la arcotangente.

Otra forma muy común en la naturaleza es la curva logarítmica, que se parece a una L mayúscula invertida o también se le puede ver parecida a una r minúscula, que crece mucho al principio, pero luego empieza a crecer poquito a poquito mientras más cerca está de llegar al 100%.

La forma que nos facilita la vida para hacer cálculos es una línea recta inclinada.


Estas curvas de probabilidad, en realidad vienen de sumar cada partecita que suma. Por ejmplo: un helado llena la nevera lo mismo que otro helado, entonces sumar lo que llenan dos helados es multiplicar por dos el espacio que llena uno. Así si se necesitarán 100 helados, cada helado suma un 1% a la probabilidad de llenar la nevera.

A veces es más util usar ese 1% de cada helado.

Por ejemplo, un dado de juegos de mesa, tiene 6 posibles resultados, cada resultado tiene un 100/6=16.66% de salir al tirar el dado. Ese 16.66% es más útil, porque en cada tirada solo tendremos una cara arriba del dado.

Esta otra forma de ver cada partecita que suma el porcentaje se le llama masa de probabilidad. 

Pero similar a lo que ocurre entre saber el peso o masa de tomates y arroz: Para el primero podemos pesar cada tomate, pero para el arroz no vamos a pesar cada granito, sino que nos sirve tener una idea de cuantos granitos pesan un gramo. Por eso cuando las partes que hay que sumar para llegar al 100% son muchas, no hablamos de masa de probabilidad sino de densidad de probabilidad.


La forma de las curvas de la densidad de probabilidad, son la campana de Gauss o distribución normal para la curva función de error. Una exponencial negativa que se parece a una L mayúscula para la curva logarítmica. Y una línea recta horizontal, para la probabilidad que tiene una línea recta inclinada.

A la probabilidad como tal se le llama tambíen función acumulada de probabilidad, pues como se decía antes: es la suma de cada partecita. A la probabilidad se le representa con letras mayúsculas: $P(X)$.

La densidad de probabilidad tienen muchas más formas conocidas en la naturaleza y es a lo que en realidad se conoce como **distribuciones de probabilidad**. A la densidad de probabilidad se le representa con letras minúsculas: $p(x)$.

En la representación hay que tener siempre presente que las partecitas se identifican con la $x$ minúscula, llamada también variable aleatoria. Así que la probabilidad $P(X)$ no nos dice hasta que valor de $x$ estamos considerando, por eso debemos indicarle hasta donde estamos sumando y se expresa como $P(X\leq x)$.  

#### Laplace o Bayes

En nuestro ejemplos hemos dicho que para que una probabilidad tenga más utilidad se debe conocer cuánto es el 100%. Pero esto no siempre es posible.

Cuando una densidad o masa de probabilidad sale de dividir el 100% para las partes, como en el ejemplo del dado, se dice que es una probabilidad Laplaciana. Algo bastante usasdo en estadística, donde se busca información pero se tienen más datos conocidos.  

##### Cálculo de porcentajes: 

$ 100/6 = 1/6 * 100 = 16.66%$

Pero, ¿Cómo podríamos saber cuantos caras tiene un dado virtual, del cuál solo vemos el resultado?

Por ejmplo nos sale un 2 en la primera tirada. Sería básico suponer que tiene también la cara con el 1, así nuestra masa de probabilidad inicial sera $100/2=50%$ para cada cara.

Apretamos el botón de siguiente lanzamiento y nos sale un 4. ¿Será que realmente hay la cara con el 1, o el dado solo tiene números pares?.  



### Entropía de Shanon

### Información Mutua

### Divergencia Kullback–Leibler

### Complejidad de Kolmogorov

### Complejidad Lempel-Ziv

