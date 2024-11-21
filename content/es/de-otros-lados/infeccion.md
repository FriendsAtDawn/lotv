---
title: "Cómo lidiar con los pdfs infectados del Judisof(TM)."
description: "Guía de sobrevivencia."
draft: false
date: 2024-02-07
featured_image: "/images/pdf.png"
---

![](https://img.shields.io/badge/document_v.-0.5-blue)

Esta entrada no quiere desacreditar al Judisoft(TM). La implementación del sistema es de lejos el salto mas importante que ha tenido el acceso a la justicia y contribuye de manera grandiosa a abaratar los costos del proceso. En todo sentido es un éxito.

## Frecuencia.

Si me refiero más a los documentos que emanan de los juzgados, que a los que presentan los colegas, es porque tengo trato intenso con todos los Juzgados e interacción también intensa pero apenas con un puñado de abogados.  Es una cuestión de frecuencia.

Nunca he recibido un ```pdf``` infectado subido por un colega. En este sentido, parece ---no sé--- que el Judisoft ejercer mayor control.

## Preliminares.

### ¿Tienen virus los archivos del judisoft?

Depende de que se entienda por virus. Tiene código sospechoso o decididamente malicioso. Pero sitios mejor autorizados poca información podría dar al respecto salvo que "alguna cosa hacen" y decididamente ocupan un espacio en el tráfico.

### ¿Lo tienen todos, siquiera la gran mayoría?

No, ---basado en mi experiencia--- son pocos los ```pdfs``` infectados considerando el gran caudal de ellos. La mayoría provienen de nuevos pdfs. Pero no es aventurado pensar que su numero crece. De hecho el archivo que aquí se exhibe como muestra parece que se duplico en otro; porque aun cuando es de un expediente que contiene una petición mía, estaba adosado a otra lista. Como conocemos muy poco de la manera en que trabaja el Judisoft[^1], ello podría tratarse de otro tipo de error.

Carpeta con el [archivo original y _timestamps_](https://bafybeiau7f4waqhoinfba5gci2ecd3hfqxjopoykvfi6cc4sgcmfihyiue.ipfs.nftstorage.link/) Está allí al solo efecto de la prueba, si van a abrir algún pdf, mejor abrir el original que se halla en:[https://www.csj.gov.py/verificarDocumento/Default.aspx?c=cdecaech&o=b](https://www.csj.gov.py/verificarDocumento/Default.aspx?c=cdecaech&o=b).

El análisis [hybrid-analisys.com](https://hybrid-analysis.com/sample/d9ceea207e9dd5a0040ca8db12357f4c4a3607520ad993fe057fe84e4f24a25a/65dbb8cb7eaf4029bd001d5a). Nótese que hay archivos nombrados como "legítimos" recursos de Adobe. Y hay otros que no y hay otros que definitivamente son programas, vuelvo a subrayar, "legítimos". Es una ensalada varia a veces difícil de seguir por lo que requiere paciencia leer todos los documentos.

### ¿Como funciona si mi antivirus no detecta nada?

De alguna forma no se activa si no pasa de Windows a un *nix. Es decir de un SO a otro. Como la mayoría usa Windows parecería que no hay razón alguna para preocuparse, pero recuerden que desde Windows 10 creo o quizás ya antes, Windows incluye un API de Linux. Una inmensa minoría usa Darwin. Tal vez ni siquiera saben que usan Darwin: solo compraron la mejor PC guiándose por el precio. Secundariamente son ellos los objetivos. Muy secundariamente. 

[^1]: Y hasta donde yo sé, hasta ahora nadie ha usado la ley de transparencia para solicitar el código fuente del Judisoft.

### ¿Son peligrosos, debo tener cuidado?

Hay dos respuestas:

- No. De hecho todo el mundo vive la fantasía de que nada tiene que ocultar del mundo, mientras piensan en su esposa.  En ese caso puede dejar su numero de CI y contraseña del banco en el mensaje.

En otro caso:

- Si.

Si nadie sabe que hacen estos _scripts_ quizás no estén haciendo algo bueno. La proposición más entera supone que es un tipo de codigo malicioso llamado [ramsoware](https://www.avast.com/business/resources/protection-against-linux-ransomware#pc).

### Por que me pasan estas cosas?

Bien veamos.

## El plan PDF/A --- Ó: ¡Me encanta cuando un plan no se concreta!

Según la Acordada que se refiere al e-Expediente, al subir  un archivo desde nuestro equipo el mismo es recodificado a PDF/A.

Ello no pasa. [Teóricamente](https://pdfa.org/resource/pdfa-flyer/) ello hubiera sido suficiente para limpiar cualquier documento.

En cuanto a los juzgadores imposible siquiera pensar en el mismo proceso ya que el mismo invalidaría la firma.

## ¿Descuido de los jueces?

Cuando yo firmo  un ´´´pdf´´´ (¿a quien se le ocurre firmar un pdf?: a alguien que se hizo la idea de que los archivos de texto no son lo suficientemente sexy[^2]) con mi firma electrónica probablemente-no-certificada, la fecha se toma de [```Sectigo```](https://sectigo.com). Cuando los jueces lo hacen lo hacen, ...lo toman de su pc. El INTN tiene un servidor NTP. No sé si la gente syncroniza la hora de su pc con él y no lo creo.

[^2]: Im too sexy for my text, too sexy for my text, more sexy than I expect.

Así que, no. No es descuido de ellos.

## Bloquear los servidores no es es una salida.

Carezco de los conocimientos necesarios para conocer qué es lo que hace cada uno de los servidores que aprovechan la debilidad del ```pdf``` ni cual es el número de ellos, pero no serviría de nada.

No puedo decirles que la solución esta en bloquear las peticiones por ```dns``` y no creo que todos quieran tener un servidor ```dns``` corriendo en la oficina, lo que dicho sea de paso es solo una extravagancia. Y por mas de que lo tuvieran, de que valdría si estos sitios maliciosos mutan cada dia.

## So?

Yo he tomado estas medidas de emergencia

- **Desactivar WebRtc:** se lo puede hacer mediante una extensión que existe para los distintos browsers, en diferentes sabores.

- **No desplegar pdf** alguno dentro del browser.

- **Mantener la base de datos local fuera** del alcance de internet --en lo posible; internet esta en todos lados.

Los ```pdfs``` infectados los he impreso y escaneado. Se quen es una salida pedestre pero más no sé hacer ya que de hecho el [Paperless](https://docs.paperless-ngx.com/) corre sobre Linux.

---

Posdata: El _pp_ es un hermoso _wrapper_ de por lo menos 10 programas. Desactive uno de ellos y _solucioné_: mi problema.

---

No puedo hacer lo que algunos sitios recomiendan:

- desactivar Javascript: sin JS el Judisoft es inusable y mi propia base de datos es inusable.

# Hay una solución política?

Si, pero no le veo futuro. Para evitar el recargo de trafico, controlar el acceso a los recursos y abaratar los costos se podría escribir un API de REST para las personas que quieran usarlo. Ello, quizás frenaría lo que parece ser una creciente infección. ¿Se imagina alguien tener el Judisoft secuestrado y pedir rescate por él?

Con el API, ninguna secrecia será vulnerada.

Al contrario se puede mejorar el control de acceso a los recursos.

Pero... hay un formularios de denuncias que están hechos en ```Google Form```; si no hay tiempo para hacer un ```<form>``` no habrá tiempo para hacer una API.--

---

Posdata: Hace unas semanas, no pude postearlo en su momento, recibí un email de la C.G.T.: estaba tan lleno de cosas extrañas que el mismo Judisoft no podía aceptarlo. No sé si colocarlo en el blog. Debe ser, para un usuario de Win, muy peligroso.

{{< graphcomment >}}


