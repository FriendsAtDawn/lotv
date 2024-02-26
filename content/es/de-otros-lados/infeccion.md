---
title: "Cómo lidiar con los pdfs infectados del Judisoft^TM."
description: "Guía de sobrevivencia."
draft: false
date: 2024-02-07
---

Estado del documento: 0.5

## Cómo lidiar con los pdfs infectados del judisoft.

Estas breves líneas, a los cuáles incluso el humilde epíteto de artículo le queda holgado, no quiere desacreditar al Judisoft^[TM]. La implementación del sistema es de lejos el salto mas importante que ha tenido el acceso a la justicia y contribuye de manera grandiosa a abaratar los costes. En todo sentido es un éxito.

## Frecuencia.

Si me refiero más a los documentos que emanan de los juzgados, que a los que presentan los colegas, es porque tengo trato intenso con todos los Juzgados e interacción también intensa pero apenas con un puñado de abogados.  Es una cuestión de frecuencia.

Nunca he recibido un pdf infectado subido por un colega. En este sentido parece ---no sé--- que el Judisoft ejercer mayor control.

## Preliminares.

### Tienen virus los archivos del judisoft.

Depende de que se entienda por virus. Tiene código sospechoso o decididamente malicioso. Pero tanto yo como sitios mmejor autorizados poca información podría dar al respecto salvo que "alguna cosa hacen" y decididamente ocupan un espacio en el tráfico.

### ¿Lo tienen todos, siquiera la gran mayoría?

No, ---basado en mi experiencia--- son pocos los pdfs infectados considerando el gran caudal de ellos. Pero no es aventurado pensar que su numero crece. De hecho el archivo que aquí se exhibe como muestra parece que se duplico en otro; porque aun cuando es de un expediente que contiene una petición mía, estaba adosado a otra lista. Como conocemos muy poco de la manera en que trabaja el Judisoft[^1], ello podría tratarse de otro tipo de error.

### ¿Son peligrosos, debo tener cuidado?

Hay dos respuestas:

- No. De hecho todo el mundo vive la fantasía de que nada tiene que ocultar de su esposa.  En ese caso puede dejar su numero de CI y contraseña del banco en el mensaje.

En otro caso:

- Si.

Si nadie sabe que hacen estos _scripts_ quizás no estén haciendo algo bueno.

### Por que me pasan estas cosas?

Bien veamos.

## El plan PDF/A --- Ó: ¡Me encanta cuando un plan se concreta!

Según la Acordada, al subir  un archivo desde nuestro equipo el mismo es recodificado a PDF/A.

Ello no pasa.

En cuanto a los juzgadores imposible siquiera pensar en el mismo proceso ya que invalidaría la firma.

## ¿Descuido de los jueces?

Cuando yo firmo  un ´´´pdf´´´ (¿a quien se le ocurre firmar un pdf? A alguien que se hizo la idea de que los archivos de texto no son bonitos) con mi firma electrónica probablemente-no-certificada, la fecha se toma de ```Sectigo```. Cuando los jueces lo hacen lo hacen, ...lo toman de su pc. El INTN tiene un servidor NTP.

El código inserto es detectable a simple vista, pero aún asi los antivirus de Windows no lo detecta.

Así que.no. No es descuido de ellos.

## Mi susurrada entristecida historia.

Pero yo he estado a salvo de ellos. Sí he tenido problemas con el Paperless-ngx que los detecta. No uso Sistemas muy populares y los códigos que he podido observar hasta ahora son para el entorno Windows.

Aun asi, me propuse eliminarlos de mi archivo porque es muy fácil que alguien en el tramite diario remita por email alguna ```SD``` e infecte de esa manera la pc de otra persona.

Bueno eso era al menos lo que yo creía. Que estaba a salvo. Sin embargo hoy he revisado el tráfico de ```dns``` de la oficina... y, no, mis pdfs han estado "llamando a casa" desde hace tiempo, solo que, después de que un sitio hiciera demasiadas peticiones bajando cerca de 1 Gb de no se que cosa, el servidor bloqueo ese tráfico y me mandó un mensaje. De esos que nunca leo.

## Bloquear los servidores no es es una salida.

Carezco de los conocimientos necesarios para conocer qué es lo que hace cada cual, pero tampoco serviría de nada porque ya he reconocido como 5 distintos. Bah. Yo no lo reconocí. Lo hicieron los sitios web que se ocupan de ellos.

No puedo decirles que la solución esta en bloquear las peticiones por ```dns``` y no creo que todos tengan un servidor ```dns``` corriendo en la oficina. Y por mas de que lo tuvieran, de que valdría si estos sitios maliciosos mutan cada dia.

## So?

Yo he tomado estas medidas de emergencia

- desactivar WebRtc: se lo puede hacer mediante una extensión que existe para los distintos browsers, en diferentes sabores.

- No desplegar pdf alguno dentro del browser.

- Mantener la base de datos local fuera del alcance de internet --en lo posible; internet esta en todos lados.

Los pdfs infectados los he impreso y escaneado. Se quen es una salida pedestre pero más no sé hacer.

No puedo hacer lo que algunos sitios recomiendan:

- desactivar Javascript: sin JS el Judisoft es inusable y mi propia base de datos es inusable.

# Hay una solución política?

Si, pero no le veo futuro. Para evitar el recargo de trafico, controlar el acceso a los recursos y abaratar los costos se podría escribir un API de REST para las personas que quieran usarlo.

Ninguna secrecia será vulnerada.

Al contrario se puede mejorar el control.

Pero... hay un formularios de denuncias que están hechos en ```Google Form```; si no hay tiempo para hacer un ```<form>``` no habrá tiempo para hacer una API.

[^1]: Y hasta donde yo sé, hasta ahora nadie ha usado la ley de transparencia para solicitar el código fuente del Judisoft.
