---
title: "Halting Problem por reducción al absurdo"
layout: post
date: 2023-04-26
image: /assets/images/markdown.jpg
headerImage: false
tag:
- halting problem
- lógica
category: blog
author: gede
description: Turing McFly 
---

# Halting problem por reducción al absurdo

Existe una categorización, por suerte cada vez menos significativa, entre filosofía analítica y continental. Esta distinción es muy graciosa, en principio, porque se trata de un criterio geográfico. ¿Por qué “analítica” en vez de “insular”? Resulta irónico que una clasificación que pretende anunciar distintos grados de logicidad sea ella misma tan ilógica. Es, también, una clasificación de tradición imperialista porque el “continente” al que alude es en realidad todo el mundo menos Inglaterra. Como sea, siguiendo este absurdo criterio se supone que la filosofía continental es existencialista mientras que la analítica sería más “matemática”. Sin embargo, pude confirmar parcialmente semejante tontería mientras estudiaba filosofía. Todas las carreras tienen alguna materia temida y, por lo menos donde y cuando estudié yo, en el caso de filosofía era “Lógica”. A muchxs lógicxs y matemáticxs les gusta pensar que este prejuicio se debe a la sofisticación de su campo, al elevado nivel de abstracción que requiere. No es así, más bien tiene que ver con lo mal que se enseña. 

Yo creía que la lógica y la matemática no me gustaban pero la verdad es que desde el primer momento me enamoré de los comandos y las operaciones cuando de muy chico tuve mi primera computadora. Cuanto más pasa el tiempo más me interesan estas materias y más me doy cuenta hasta qué punto las aplico cotidianamente. Los infames “ejercicios” con los que se rellenan las cátedras no tienen nada que ver con la lógica o la matemática. Toda esa pavada que se vende como gimnasia mental es en realidad una manera rebuscada de repetición irreflexiva. La sustancia de estas materias está en los sistemas y conceptos, no en los algoritmos. Qué tontería cómo se habla de “el algoritmo”. Como si fuera uno solo, como si contuviese algo esencial. ¿Acaso se pretende también embrutecer la enseñanza de la informática?

En filosofía, por lo menos, se cuenta con la ventaja de que se supone que las personas en general saben menos lógica que matemática (ya ven hasta qué punto llega todo este sinsentido). Entonces, en la materia “Lógica” se arranca con lo más básico mientras que ningún estudiante de ingeniería tendrá la suerte de que le enseñen como es debido qué son los números o cómo es que se puede sumar, restar, etc. Esto sumado a que la programación se concibe eminentemente lógica más que matemática, hizo que no solamente no le tenga miedo a “Lógica” sino que, con su perdón, la disfrutara muchísimo.

Uno de los problemas más famosos de la programación es el “halting problem” y me ha frustrado mucho encontrar explicaciones muy complicadas, quizás al pedo. Aclaro que no soy ningún especialista y que toco de oído pero a mí me resultó más fácil de aprehender desde la reducción al absurdo:
En Volver al Futuro, el protagonista viaja al pasado y provoca un accidente que impide que su padre y su madre se conozcan. Tiene, entonces, que lograr que se conozcan porque, de lo contrario, él mismo no nacerá. Pero si no nace tampoco puede viajar en el tiempo e impedir que su padre y su madre se conozcan. Es decir, suponer que es posible que alguien viaje en el tiempo e impida su propio nacimiento conduce a una paradoja, algo imposible, indecidible, irresoluble. Podemos concluir, entonces, que no es posible viajar en el tiempo (al menos en estos términos). Tal cosa en lógica se llama “reducción al absurdo”. Si una suposición nos conduce a una contradicción podemos afirmar que lo que supusimos no puede darse (sin destruir al universo).
El “halting problem” es como la paradoja del viaje en el tiempo pero con programas de computadora. 

0- Supongamos que existe un programa **A** que nos puede decir si otro programa se va a detener en algún momento o se va a colgar para siempre. Con esto en mente:
	1– Para probar nomás, hagamos un programa **B** que cuente hasta diez y termine.
	2- Preguntémosle a **A** por **B**. Nos dirá que se va a detener y, en efecto, al llegar a diez **B** finaliza. ¡Excelente!
	3- Ahora sí, para joder un poco, hagamos otro programa **C** que haga lo contrario de lo que diga **A** a ver qué pasa.
	4- Preguntémosle otra vez a **A** por **B**.  Como nos dice que **B** se va a detener, **C** se va a colgar. ¡Esto va muy bien!
	5- ¿La quieren cagar? Preguntémosle a **A** por **C**. Si **A** nos dice que **C** se va a detener, **C** se va a colgar y si **A** nos dice que **C** se va a colgar, **C** se va a detener. 

Acabamos de destruir al universo.
