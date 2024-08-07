---
title: 'Análisis Espacial con R: manejo, visualización y modelos econométricos'

tags:
 -R software
 -Rstats
 -regional science
 -data visualization
 -spatial autocorrelation
 -spatial econometrics

authors:
 - name: Jaime A. Prudencio-Vázquez 
   orcid: 0000-0001-5866-1280
   affiliation: 1

affiliations:
 - name: Economics Department, Universidad Autónoma Metropolitana, Unidad Azcapotzalco, CDMX, México.  
   index: 1

date: 1 March 2022

bibliography: paper.bib

---
#Resumen

Análisis Espacial con R: manejo, visualización y modelos econométricos es un [curso abierto completo](https://github.com/jaime-pru/Analisis-de-datos -espaciales) en español para el análisis de información espacial en software R. El curso está dirigido a estudiantes de pregrado de economía de habla hispana interesados en desarrollar habilidades técnicas para el análisis cuantitativo que requieren las ciencias regionales [@Fischer2014] y el enfoque espacial de la economía [@Fujita2000], pero podría ser útil para otras estudiantes de ciencias sociales atraídas por el tema.

El objetivo del libro es guiar a la estudiante, desde un enfoque fundamentalmente práctico, en el conocimiento y manejo de técnicas de exploración, análisis y modelado de información espacial mediante el uso de R [@RSoftware] y RStudio que son, respectivamente, un programa informático y lenguaje de programación enfocado al análisis estadístico y visualización de información, por un lado, y un entorno de desarrollo integrado (IDE), por otro.

El curso se presenta en forma de libro electrónico y está estructurado en cinco capítulos de aprendizaje gradual. En el Capítulo 1, se presentan los elementos básicos de R y RStudio mediante el uso del enfoque de análisis exploratorio de datos [@HSM2014] no sólo con el paquete básico de R, sino también con el popular conjunto de herramientas que provee tidyverse [@tidyverse], es decir, se introduce completamente al estudiante en el uso del software para proponer y resolver preguntas relacionadas con la estructura información. El Capítulo 2 muestra cómo crear varios tipos de mapas de coropletas y la enorme flexibilidad de personalización de estilo que tiene R para este propósito a través del paquete tmap [@tmap]. El Capítulo 3 presenta la forma de realizar un análisis exploratorio de datos espaciales donde el estudiante encontrará cómo definir las interrelaciones que se dan en el espacio a través de la construcción de matrices de pesos espaciales y aprenderá sobre la autocorrelación espacial y sus implicaciones en el análisis de la información, todo ello a través de diversos paquetes como spdep [@spdep] y rgeoda [@rgeoda]. Mientras tanto, en el Capítulo 4, se presenta una revisión muy sintética de los modelos de regresión simple, enfatizando el problema de autocorrelación que podría ocurrir al estimar un modelo lineal con datos espaciales. Finalmente, en el Capítulo 5, se muestran dos de las diferentes alternativas de modelado econométrico espacial disponibles en R, con spatialreg [@spatialreg].

La lógica de cada capítulo integra tres elementos: i) explicación de los conceptos fundamentales tratados, ii) el uso de información real en el software que sirve para ilustrar los conceptos proporcionados, iii) ejercicios propuestos para que el estudiante profundice sobre los temas expuestos.

Los ejemplos y ejercicios que se presentan en el curso se basan en una base de datos sobre la situación de la pandemia de COVID19 entre marzo y septiembre de 2020 en la Zona Metropolitana del Valle de México (Zona Metropolitana del Valle de México), el área metropolitana más grande de México, integrado por 76 unidades administrativas locales o municipios con más de 21 millones de habitantes. Además, la base de datos utilizada proporciona información sobre la estructura económica a nivel municipal y un conjunto de variables de características sociodemográficas provenientes del censo de población.

# Historia del proyecto

El proyecto surge y se alimenta de dos experiencias académicas. La primera, que se remonta a 2014, corresponde a mi labor como docente de herramientas para el análisis espacial a través de varios cursos introductorios. La segunda es un curso de actualización sobre el uso del software R que impartí en otoño de 2020, desde el Departamento de Economía de la Universidad Autónoma Metropolitana Unidad Azcapotzalco.  

Como resultado, múltiples notas y materiales fueron generados y gradualmente incorporados a mi actividad docente en el curso de Econometría Espacial, del que soy responsable desde hace más de 3 años. Econometría Espacial forma parte de la oferta académica de la línea de especialización de la Licenciatura en Economía llamada "Economía de la Innovación: empresas, redes y territorio", de la citada universidad. Frecuentemente me vi en la necesidad de generar materiales para la enseñanza de los contenidos de dicho curso. Así, en lugar de materiales aislados y desestructurados, decidí compilar y ordenar con una lógica expositiva coherente y de aprendizaje gradual el conjunto de materiales trabajados hasta ahora y que ahora componen este curso.

Desde enero de 2022, que se puso en circulación la versión integrada de esta serie de materiales bajo la forma de libro electrónico, el curso de Econometría Espacial se ha impartido de forma continua en promociones trimestrales a casi 50 estudiantes.

# Declaración de Necesidad

Las ciencias regionales se caracterizan por su carácter multidisciplinario y su sólido soporte cuantitativo [@Fischer2014]. Si bien es cierto que en todas las carreras de economía encontramos un sólido repertorio de instrumentos cuantitativos: matemáticas, estadística y, por supuesto, econometría, las herramientas necesarias para el análisis de la realidad desde una perspectiva espacial y regional siguen siendo escasas dentro de la formación a nivel de licenciatura. [Análisis de datos espaciales con R](https://jaime-pru.github.io/Analisis-de-datos-espaciales/index.html) pretende ser una contribución, aunque sea mínima, para remediar esta situación.

Además, gran parte de la literatura sobre el manejo de datos y análisis de información espacial aún se encuentra en un idioma diferente al español, mayoritariamente en inglés, lo que dificulta el acceso a estas herramientas a quienes aún no dominan el idioma. Esto se convierte en una barrera al conocimiento, de manera notable en países como México en los que el dominio del inglés sigue siendo muy bajo [@IMCO2015; @EF2020]. Así, este material en español se convierte en una puerta de entrada para las interesadas en estos temas y facilita el proceso de aprendizaje.
El libro, enfocado a estudiantes de pregrado no especialistas en el tema, se pretende constituir como un material accesible, en la medida en que el estilo de la exposición busca ser didáctico y lo más sencillo posible, sin perder rigor expositivo.

Al ser un libro introductorio, recomienda e invita al uso de múltiples materiales, tanto en castellano como en inglés, para que la estudiante profundice por su propia cuenta en el conocimiento del manejo de información espacial y de la plataforma informática en la que se lleva a cabo.

# Sugerencias para seguir el curso

Cada capítulo contiene elementos tanto teóricos como prácticos relacionados con el tratamiento de datos espaciales en el contexto de la economía. Estos se ilustran a través de segmentos de código en R que se explican en su lógica y estructura para que la estudiante no solo pueda replicar los resultados, sino también comprender qué hace cada pieza de código. Además, a lo largo de cada capítulo se proponen ejercicios para profundizar, a manera de reto, en el conocimiento sobre las herramientas que se exponen, por lo que las respuestas no son proporcionadas.  

La forma sugerida de seguir el curso es a través de la secuencia propuesta por la estructura del libro, del capítulo 1 al 5, pues se expone las herramientas de forma gradual, tratando de asegurar una adecuada asimilación. Sin embargo, si la estudiante ya se siente cómoda con el manejo de algún tema, puede continuar con el siguiente sin dificultad.

La experiencia en el uso de este material indica que puede ser cubierto en 5 o 6 semanas, dedicando entre 4.5 y 5 horas semanales de estudio. El capítulo 1 puede ser cubierto en aproximadamente 4.5 horas, sin embargo, si la estudiante no está familiarizada con R y RStudio podría extenderse un poco más. La sección correspondiente a la elaboración de mapas de coropletas sería cubierta sin inconvenientes en alrededor de 3 horas. En tanto, el Capítulo 3 relativo al análisis exploratorio de datos espaciales, una de las partes centrales del libro, puede requerir de al menos 6 horas de estudio. El Capítulo 4, dedicado al repaso elemental de la regresión lineal, puede ser cubierto en 3 horas de estudio, dado que se asume cierto conocimiento previo sobre el tema, no obstante, podría requerirse más si la estudiante necesita repasar con mayor profundidad dichos tópicos. Finalmente, el Capítulo 5, también nodal en este material, requeriría de alrededor de 6 horas de estudio.

# Contribuciones

Este libro es, en alguna medida, un esfuerzo de recopilación y sistematización de múltiples materiales que la activa comunidad de R, interesada en el análisis espacial en México y el mundo, comparte desinteresadamente.

Considero que así debería ser siempre el conocimiento: libre, abierto y colaborativo, como el software que es usado aquí. Así pues, este proyecto es un proyecto vivo, en permanente construcción y modificación, por lo que todos los comentarios y observaciones serán bienvenidas, tanto de las estudiantes que lo han usado, como de las docentes que consideren oportuno incluirlo dentro de sus materiales de referencia.

Una guía sobre cómo contribuir a este proyecto se puede encontrar en el repositorio de GitHub en https://github.com/jaime-pru/Analisis-de-datos-espaciales/blob/main/How_to_contribute.md. Las personas interesadas también pueden contactar directamente vía correo electrónico (japv@azc.uam.mx) o incluso en las redes sociales en [twitter](https://twitter.com/jaime_pru). Todos los comentarios serán bienvenidos.

# Referencias