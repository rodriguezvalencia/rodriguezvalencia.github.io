---
layout: post
title:  "Designing Data-Intensive Applications - una reseña"
date:   2020-05-19 17:37:02 +0100
categories: Reseña
---

Designing Data-Intensive Applications - una reseña
---

[Designing Data-Intensive Applications](https://www.amazon.co.uk/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321) de Martin Kleppmann es un libro excelente y lo considero un clásico moderno cuasi-obligatorio para cualquier desarrollador senior. Representa una perfecta introducción a las soluciones para esos sistemas que buscan procesar cantidades de datos enorme y escalar hasta cantidades de usuarios tremenda. Este es un área donde es bastante difícil conseguir experiencia, no solo porque estos problemas solo existen en ciertas empresas de cierto tamaño, sino porque el campo es extensísimo (basta ver la bibliografía al final de cada capítulo, donde a veces podemos encontrar más de cien referencias!) y los problemas con que nos enfrentamos cuando hablamos de esta escala son muy distintos de los que se encuentran en sistemas de tamaño más modesto.  

El libro da una visión general del campo de las aplicaciones de datos a gran escala y generalmente en sistemas distribuidos. Sin nunca entrar en demasiado detalle específico sobre las tecnologías que menciona, sí que ofrece una aproximación a los principios, prácticas y métodos y generales empleadas en el diseño de estos sistemas. Uno de los aspectos más refrescantes es que el autor nunca presenta ningún concepto como la solución perfecta que soluciona cualquier problema. En lugar de eso se preocupa explícitamente de remarcar las ventajas y desventajas propias de cada concepto, con lo que en conjunto te ofrece una serie de “piezas” que tu, como ingeniero/arquitecto/developer que eres debes de saber aplicar para solucionar tu problema específico.

Pero.

Lo que pasa es que los desarrolladores somos tremendamente sensibles a las modas. Nos vemos una conferencia en la que uno de Google, Uber, Spotify o cualquier otra empresa molona nos cuenta como si fuera un actor de teletienda que desde que están usando esta nueva tecnología superchachi todos sus programas compilan más rápido y sus despliegues a producción en viernes salen siempre bien. Y nos lo creemos y raudos vamos a adoptar dicha tecnología a la siguiente oportunidad que se tercie.

Y entonces nos damos cuenta que esta tecnología es chachi y genial y soluciona todos tus problemas… si tus problemas son los de la empresa molona donde la crearon. Que fuera de una empresa gigante con miles de developers y cientos de millones de usuarios, o sea, a tu escala, esta tecnología da problemas, es difícil de mantener o que, simplemente ni siquiera es apropiada para tu problema. NoSQL, Microservicios, React, Kubernetes, Go, Dart, HHVM… la lista de tecnologías que se han puesto de moda y han sido adoptadas sin pensar es inmensa.

Un ejemplo: durante los últimos 10 años casi cualquier nuevo sistema se ha arquitecturado siguiendo microservicios. Esta arquitectura tiene como atractivos una serie de ventajas como modularidad, escalabilidad, el poder integrar sistemas heterogéneos y facilitar el desarrollo distribuido entre diversos equipos. Sin embargo, también conlleva una gran cantidad de problemas como la visibilidad del sistema, el descubrimiento y orquestación de los sistemas, y la gestión de versiones. Una startup recién empezada con 4 developers y 100 usuarios ¿de verdad pensamos que va a obtener alguna ventaja de implementar su prototipo con microservicios? ¿O se verá obstaculizada por una decisión técnica que solo tiene sentido en una empresa múltiples órdenes de magnitud más grande? A esta tendencia de adoptar lo que hacen las empresas molonas sin pensar si es lo apropiado algunos lo llaman *resume driven development*, aunque yo prefiero llamarlo ser un Google cosplayer. 

(Y no solo pasa con cosas técnicas… valga el ejemplo de la estructura de equipos en tribus de Spotify, o como toda la industria adoptó el modelo de entrevistas que sobrevalora los temas de algoritmia para puestos que no lo necesitan. ¿Cuantas veces has tenido que escribir codigo para rebalancear un árbol rojo-negro en tu trabajo?)

Leer libro Designing Data-Intensive Applications te pone en riesgo y es a la vez una defensa. Te tienta con multitud de conceptos molones (RPC! …) y a la vez te deja bien claro que implementar ese concepto tiene un precio, y no es gratis. Este libro no es un cookbook en el que abres por una página y copiar y pegar el primer código que veas, sino que recompensa una lectura y reflexión pausadas y profundas; y nos confiere una mirada más madura y justificada de los sistemas que construimos.

Y sobre todo, nos ayuda a no ser cosplayer.


