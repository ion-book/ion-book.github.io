---
layout: post
title: "¿Qué es Bundlephobia?"
date: 2018-09-05
tags: [angular, news, ionic, bundle, bundlephobia, rendimiento]
categories: tips
author: nicobytes
video: true
cover: "https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fcover.jpg?alt=media&token=1b3bfe1b-6d64-4650-a50d-a8a55d7aad29"
---
> Bundlephobia.com es una herramienta que nos permite evaluar el peso de librerías, de esta forma podemos comparar y evaluarlas antes de instalarlas dentro de una aplicación.

<img width="1280" height="720" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fcover.jpg?alt=media&token=1b3bfe1b-6d64-4650-a50d-a8a55d7aad29"> 

Bundlephobia se puede traducir como fobia al peso de la aplicación, pero en este caso vamos a ver [bundlephobia.com](https://bundlephobia.com/){:target="_blank"} que es una herramienta para poder evaluar el peso de las librerías que se usan en una aplicación. 

<img width="828" height="529" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fscreen1.png?alt=media&token=b1de11ab-33a0-4521-831d-3186353f58e2"> 

Con esta herramienta podemos buscar cualquier librería que este publicada dentro de `npm` y ver cual es su peso en bytes. A continuación, un ejemplo con `d3JS`:

<img width="1029" height="592" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fscreen2.png?alt=media&token=199be038-d54a-4c35-a709-f93d0aba5d6f"> 

Con esto podemos ver visualmente que `d3js` pesa 300kb, este peso será que costo en bytes para la aplicación, este es el punto donde debemos evaluar el costo/beneficio de la librería dentro de una aplicación.

En el mismo reporte nos muestra si esa librería esta compuesta por otras, en el caso de ejemplo, nos muestra que `d3js` esta compuesta por otras librerías:

<img width="1092" height="401" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fscreen3.png?alt=media&token=2bbe1cd6-a010-47e7-b70f-ced1535be43e"> 

Otro característica muy útil es poder subir el archivo `package.json` de cualquier aplicación:  

<img width="673" height="392" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fscreen4.png?alt=media&token=3f9b2526-c489-4b4d-ab97-8ce397fe1ee9"> 

Como resultado tendremos el peso de cada una de nuestras dependencias, ordenadas de mayor a menor respecto a el peso:

<img width="910" height="700" class="responsive" src="https://firebasestorage.googleapis.com/v0/b/ngclassroom-8ba81.appspot.com/o/posts%2F2018-09-10-bunldephobia%2Fscreen5.png?alt=media&token=bcecc649-ad70-41ce-9c0d-471eaec4b6cc"> 


El objetivo es determinar que librería puede estar causando un peso innecesario dentro de una aplicación.

En el video siguiente, examinó la herramienta a más detalle y vemos como poder determinar que librerías pueden llegar a ser innecesarias evaluando un costo/beneficio.

<amp-youtube width="560" 
            height="315"
            class="responsive"
            data-videoid="I-Jd0chWu2k"></amp-youtube>
