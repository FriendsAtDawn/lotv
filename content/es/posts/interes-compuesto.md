---
title: "Interés compuesto"
description: "Introducción a la siguiente entrada"
draft: false
tags: ["interés", "compuesto", "interés compuesto contínuo", "ICC", "matemáticas"]
date: 2023-03-07
---

## Interés compuesto

Una definición bastante precisa de lo que es interés compuesto lo da Llambías cuando dice:

> 695. ANATOCISMO: NOCIÓN.- ES la capitalización de los intereses, o interés compuesto, de modo que agregándose tales intereses al capital originario pasan a redituar nuevos intereses.

Esto es notable desde la misma notación de la fórmula. La del interés simple es:

$$
I = C \times \Delta t \times ratio
$$

Casi intuitivamente que esos valores constantes ---salvo el tiempo que pasa--- van a dibujar una recta en las coordenadas cartesianas, merced justamente a que el tiempo sucede instante tras instante:

Así si partimos desde un 

$$
C = 100
$$

y

$$
ratio = 33%
$$

![IntSimple](/posts/img/iss.png)

Una ecuación de primera grado siempre genera rectas.

La del interés compuesto es:

$$
V_f  = V_n (1 + i/f)^{(f n)}
$$

Nótese que en la fórmula no se trata de hallar el interés de cierto período de tiempo porque aunque la ratio del mismo  se mantiene constante, el _principal_ crece de momento a momento ---por lo tanto el valor del interés crece de momento a momento, sino de hallar el **valor final** del principal a partir del **valor inicial**.

|         |             |                                   |
| ------  | ----------- |---------------------------------- |
| $$V_f$$ | ;           |	es el valor final.                |
| $$V_n$$	| ;           | es el valor de un periodo determinado |
| $$i$$	  | ;           | es la ratio del interés           |
| $$n$$	  | ;           | son los periodos                  |
| $$f$$	  | ;           | es la frecuencia de actualización |

Ello asumiendo que la frecuencia es un número finito. _Tout court:_ es decir que la frecuencia es un numero que podemos computar mediante una aritmética sencilla: enseguida se verá el caso en que ya no es así.

No hace falta estimar valor alguno para darse cuenta de que esa ecuación ---la del interés compuesto--- es una exponencial. En el plano no nos dibujará una recta: Veamos.

$$
V_f  = V_n (1 + i/f)^{(f n)}
$$

$$
V_f = 100 \cdot \left(1 + \dfrac{0.36}{{1}}\right)^{6 \times 1}
$$

$$
V_f = 100 \times 1.36 ^ {6 \times 1}
$$

$$
V_f = 100 \times 6.32 = 632
$$

![Interes](/posts/img/compuesto.png)

¿Es legal esto? Sí, claro. Siempre y cuando la llamada *tasa efectiva* no supere los límites usurarios. En el caso, lo hace. Así que para el mismo, no.

Y siempre y cuando la persona a cuyo favor se generan tales intereses no sea un banco o financiera. 

La orgánica del BCP decía antes:

> El interés a partir de la mora, denominado interés moratorio, será la misma tasa pactada originalmente. No podrán capitalizarse intereses moratorios por períodos inferiores a 30 (treinta) días.

Pero una modificación posterior borró toda posibilidad de que se capitalicen intereses.

Ahora bien, la frecuencia por supuesto que impacta en el valor final, es por eso que la ley anterior decía que no podía hacerse sino cada 30 días... pero ¿significaba un cambio sustancial en el monto que tenía que pagarse por intereses? La verdad no. Si uno hace los cálculos ---que no mostraré ahora pero que prometo hacerlo de manera detallada más tarde--- una capitalización trimestral es apenas _mejor_ que una diaria.

¿Y que tal si la capitalización se realiza en frecuencias cada vez más cortas? Digamos cada hora, digamos cada minuto, digamos cada segundo... Menos, cada instante. Asumamos que el tiempo se puede dividir por siempre: es cuando la frecuencia _tiende_ a cero.

Entonces tenemos lo que los libros de matemáticas llaman capitalización compuesta contínua. Su fórmula es  ---prometí no entrar en detalles por lo que me saltaré operaciones intermedias y escribiré solo la el resultado de ellas:

$$
\delta = n \mbox{ln} \left( 1 + \frac{r}{n} \right),
$$

La _delta_ minúscula es el ratio de interés _cambiante_ por decirlo de una forma, y _r_ es el interés pactado y _n_ su frecuencia. 

Esta fórmula nos parece familiar ya... Sí, ¿no es la fórmula del interés francés?


---
