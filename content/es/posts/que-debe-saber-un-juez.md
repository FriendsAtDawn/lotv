---
title: "¿Que debe saber un juez?"
description: "O, dicho de otro modo: ¿Qué se supone que sabe?."
tags: ["saber", "matemáticas", "interés", "hechos notorios"]
draft: false
date: 2023-02-07
---

*Antes de leer este post, es mejor leer el de interés compuesto.*

## Saber común.


Usualmente ello está contenido dentro de lo que el Código llama los hechos notoriamente conocidos.

¿Por ejemplo? ¿Literatura? Tal vez no. Tal vez no sepan ubicar la cita:

```
<<A tí también, en lejanas playas de oro,
Te aguarda incorruptible tu tesoro,
La vasta vaga populosa muerte.>>
```

Pero debería saber que es un terceto porque... ¿no pasaron por la secundaria?

Y tal vez no sea necesario que sepan demostrar que $$\sqrt{2}$$ es, en efecto un número irracional. Pero deberían saber lo que es uno si no falsificaron su diploma de bachiller.

Y es ahí donde quiero llegar.

Matemáticas. Los abogados suelen presumir de no saber matemáticas. Que es más o menos que una persona sorda te diga que nunca necesitó  de la música. Realmente no. Pero al hacer los cálculos de cualquier obligación dineraria, y sólo de eso se encarga la ley, en realidad, es imposible no articularla de tal forma.

Y quién lo evalúa, el Juez...  ¿Deberían conocer, por ejemplo, la fórmula del interés compuesto? ¿Deberían saber que es una simplificación de la _real_ fórmula? El Mec entiende que es cuestión del [Primer Año de la Media](https://www.mec.gov.py/cms_v2/adjuntos/13208)

Cuando digo _real_ formula me refiero  a que la capitañizaxion al tipo de interés compuesto continuo también se conoce como tipo efectivo anual (TEA o EAR por sus siglas en inglés).

## El interés francés.

En esta _método_ los pagos de capital e intereses es la siguiente:

$$
a = \frac{C}{a_{|\overline{{n}}i}}
$$

Donde:
|       |     |                                                                |
| ----- | --- | -------------------------------------------------------------- |
| $$a$$ | ,   |es el término amortizativo del préstamo, en este caso, meses.   | 
| $$C$$ | ,   |es el capital prestado.                                         |
| $$i$$ | ,   |es el tipo de interés del préstamo.                             |
| $$n$$ | ,   |es el número de meses que dura el préstamo.                     |

$$
a_{|\overline{{n}}i} = \frac{(1+i)^n - 1}{i \times (1+i)^n}
$$

Luego:

$$
a = \dfrac{C}{\dfrac{(1+i)^n - 1}{i \times (1+i)^n}} \rightarrow a = C \times \dfrac{i \times (1+i)^n}{(1+i)^n - 1}
$$

Como se observa, el interés va incluido en las cuotas desde el inicio de manera que el capital vaya amortizándose en razón de

$$
(i+1)
$$

Y el resto se inpute a intereses. El _sistema francés_ quizás no es incompatible con la forma de inputar intereses del Código Civil.

Es incompatible solamente con la Ley del Banco Central.

> El interés moratorio será calculado sobre el saldo de la deuda vencida y en ningún caso podrán capitalizarse intereses sobre los intereses moratorios ni punitorios.

Dice la [LEY N° 2339 QUE MODIFICA EL ARTICULO 44 DE LA LEY N° 489/95 “ORGANICA DEL BANCO CENTRAL DEL PARAGUAY”.](https://www.bacn.gov.py/leyes-paraguayas/5034/ley-n-2339-modifica-el-articulo-44-de-la-ley-n-48995-organica-del-banco-central-del-paraguay)

Se lo puede hallar en el excelente sitio del Congreso de la Nación (en serio lo extrañe mientras suspendieron el servicio durante casi un mes).

_Ps:_ volvió a caer, este es el link del [cache de google](http://webcache.googleusercontent.com/search?q=cache:https://www.bacn.gov.py/leyes-paraguayas/5034/ley-n-2339-modifica-el-articulo-44-de-la-ley-n-48995-organica-del-banco-central-del-paraguay&strip=1&vwsrc=0).




   



















---