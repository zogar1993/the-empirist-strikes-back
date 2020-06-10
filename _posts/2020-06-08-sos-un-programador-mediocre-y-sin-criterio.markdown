---
layout: post
title:  "Sos un programador mediocre y sin criterio"
categories: programming
---

TL;DR: El conocimiento es importante para ser un programador decente, pero tener criterio es tanto o más importante. Mi objetivo en este post y los sucesivos es no solo explicar la teoría detrás de los conceptos expuestos, sino también detallar el criterio utilizado al aplicarlos. Es importante identificar cómo y cuándo usar una determinada técnica, pero es aún más importante saber cómo y cuándo no.

El contenido relativo a la programación suele encontrarse de dos maneras en internet:

Por un lado, el artículo técnico, rebosante de teoría, explicando paso a paso cómo implementar un patrón de diseño o cómo usar una determinada tecnología, artículos tan abstractos que jamás se rebajarían a la banalidad de ejemplificar casos cercanos a lo que uno pueda encontrarse en un ámbito realista. Depende del **criterio** del programador entender cuándo usar el conocimiento de este tipo de artículos, y lo que es aún más importante, cuando no. Más de una vez he visto código "ingenioso" en las que la solución fue forzada en un problema que no lo requería, dejando detrás una sobre ingenieria imposible de mantener y escalar (confieso que he pecado de ello más veces de las que caben en un Int).

Por otro lado, tenemos infinidad de individuos de variadas edades y experiencias ametrallando la web con contenido de diversa calidad. Contenido que prioriza la promoción a la enseñanza. Contenido hecho no para quien lo lee, sino para quien lo escribe. Estos son fáciles de identificar, suelen tener una foto sonriente al lado del post, un lenguaje muy cuidado, y una gran extensión de caracteres e imágenes que parecen demorar eternamente en llegar al punto que están intentando hacer. Otra característica que tienen es que suelen comenzar con "Hola, mi nombre es Individuo X, y llevo Y años en la industria desarrollando `LISTA IRRELEVANTE DE SOFTWARE` en `LISTA IRRELEVANTE DE EMPRESAS`". Si sos de esas personas que al leer uno de estos artículos piensa "Lleva 15 años desarrollando en Java, seguro sabe mucho de lo que habla, por lo que voy a incorporar todo lo que diga sobre el lenguaje como cierto", te pido por favor que releas el título. Alguien que tiene que mencionar su recorrido para que su punto sea tomado en serio pierde credibilidad. Ya que estamos pedile que se acerque a leer el título también. Alguien orgulloso de haber pasado tanto tiempo en un lenguaje o tecnología huele a estancamiento. En fin, en este tipo de contenido el lector debe atravesar toda la maraña publicitaria y entender las partes que son útiles, queda a su **criterio** entender que conocimiento le es genuinamente util y cual le esta intentando "vender algo". Algunos ni siquiera parecen tener contenido más allá de publicitarse a ellos mismos, a la empresa para la que trabajan, o a la tecnología o a framework que utilizan. Nótese que pocas son las veces que este contenido habla de metodologías o arquitecturas (he encontrado escaso material decente al respecto, y mucho menos en español).

Nótese que remarqué la palabra **criterio** al explicar cada uno de los puntos anteriores. Esto es porque considero que precisamente eso es lo que más falta en la industria, y es precisamente lo que hace que los dos tipos de artículos qye mencioné sean particularmente peligrosos. El criterio es lo que nos permite diferenciar que es útil y que no, cuando algo es productivo o cuando va a ralentizarnos en el largo plazo, es lo que permite que que no te comas esa pizza que lleva 3 semanas en la heladera por más que ahora tengas mucha hambre. Evaluar lo conveniente, lo redituable, cuando es que la ganancia supera a la pérdida. El criterio no es algo innato. Una persona no nace con criterio. Lo desarrolla, como el resto de sus habilidades. Desarrollarlo significa aprender y ponerlo en práctica. El conocimiento solo no alcanza. Es importante que la experiencia cubra los huecos que el conocimiento no supo cubrir, para aprender a identificar problemas que los libros siquiera nos dijeron que podríamos tener, para ganar la agilidad y confianza que nos permita esquivar los obstaculos que nos vayamos encontrando.

El conocimiento sin criterio no es más que un dogma.

Quiero enseñarte a tener criterio. Quiero mostrarte lo que el conocimiento por sí solo no puede.

Mi propósito es exponer mi criterio, no para que lo copies, sino para que ayude a formar al tuyo. No me malentiendas, la experiencia vas a tener que hacerla por tu cuenta de todas formas. Después de todo, si tomaras mi criterio como cierto sin experimentarlo, no ganarias criterio real, simplemente aplicamos mis reglas de forma dogmática un programador mediocre más.

A menos de momento, tengo pensado atacar los siguientes temas, todos relacionados con ser un mejor programador (o programadora) sin importarme lenguaje o tecnología:

Refactor: Para que la codebase que estas tocando deje de ser la enorme bola de bosta que muy probablemente sea hoy en día, es necesario trabajo periodico y activo. Diria que el codigo es como una planta, que si no la regas se muere, pero una analogia mas correcta sería que el codigo es como una planta mutante, que si no la regas se sale de la mazeta, sde come a tu perro, causa terror por las calles y hace que los tiempos de delivery sean imposibles de estimar. El itinerario de refactor es el siguiente:
- Tu codigo es horrible: Los cuatro refactor basicos
- No violes los niveles de abstraccion (Refactor "para arriba")
- No sabes utilizar bien un Value Object (Refactor "para abajo")
- Deja de hacer codigo poco cohesivo (Refactor "para afuera")
- Deja de cometer Feature Envy (Refactor "para adentro")

TDD: Me costó mucho aprender a hacer buenos tests. Cada vez que aprendia algo, daba dos pasos para adelante y uno para atras. Gran parte de esto se debe a que gran parte del material es contradictorio entre si, no se pone de acuerdo en terminologias, o no es suficientemente explicito con algunas cuestiones. El itinerario para que te ahorres muchas horas de busquedas en Google tratando de entender porque tus tests parecen llevar mucho tiempo sin dar suficiente ganancia es el siguiente:
- Una introduccion a TDD que incluso vos podes entender
- Como testear irrelevancias (Chicago TDD)
- Como hacer imposible el refactor mediante tests (London TDD)
- Basta de testear detalles de implementacion

Arquitectura: Aunque no lo paresca, esto es muchisimo mas subjetivo que los casos anteriores (que de por si son subjetivos). El problema con explicar las arquitecturas es que requieren mucho conocimiento contextual para poder ganar criterio sobre ellas (quien piense lo contrario será fusilado en una plaza publica por el pecado de su ignoracia). Haré mi mejor esfuerzo por que aprendas a ganar el criterio necesario para saber porque un arquitectura puede ayudarte, pero requerirá que investigues y experimentes mas de lo normal. Es lo mejor que puedo ofrecer. El itinerario es el siguiente:
- EMS: la arquitectura que no sabias que no necesitabas
- MVC: la sobreutilizada arquitectura del programador mediocre
- Microservicios: decis saber lo que son, yo se que no tenes idea
- Casos de Uso: seguro los estas haciendo mal

Eso es bastante mas de lo que parece, y hay bastante mas de lo que podria escribir... pero ese es un buen comienzo, al menos por ahora.

Para darle cierre, quiero dejar algo claro, y eso lo siguiente: Entiendo que hay gente a quien mi forma de escribir le puede resultar repelente, y lo entiendo. De todas formas, mi respuesta es que "es su problema". Yo escribo para quienes puedan separar el contenido de la forma, para quienes quieran aprender mas y no les importe el como, para los verdaderamente autenticos, quienes no necesitan de etiqueta, y saben apreciar las cosas dichas directamente y sin vueltas. Para el resto, solo puedo desearles buena suerte. Como punto extra, ser agradable y carismatico genera dinamicas donde importa "quien" lo dice, y no "que" dice. Yo en cambio puedo estar seguro de que mis lectores permaneces a pesar mio, y no por mi.