# RetoBBVA-Concept

 [![Augmented Website](https://user-images.githubusercontent.com/252962/27472386-0d11e59a-57f3-11e7-9fa5-34332c5484f7.png)](https://github.com/jeromeetienne/AR.js)

[![npm](https://img.shields.io/npm/v/ar.js.svg)](https://www.npmjs.com/package/ar.js)
[![npm](https://img.shields.io/github/repo-size/badges/shields.svg)
<br class="badge-separator" />
[![Gitter chat](https://badges.gitter.im/AR-js/Lobby.png)](https://gitter.im/AR-js/Lobby)
<span class="badge-patreon"><a href="https://patreon.com/jerome_etienne" title="Donate to this project using Patreon"><imghttps://github.com/Umistudio/RetoBBVA-Concept/blob/master/README.md src="https://img.shields.io/badge/patreon-donate-yellow.svg" alt="Patreon donate button" /></a></span>
[![Twitter Follow](https://img.shields.io/twitter/follow/jerome_etienne.svg?style=plastic&label=Twitter&style=plastic)](https://twitter.com/jerome_etienne)

Descripción del proyecto
Proponer un nuevo proceso de vinvulación digital para futuros clientes del BBVA.

- **Objetivos** 
El objetivo de este ejercicio es poner a prueba la forma en que encaras un problema de diseño, desde una previa investigación de usuario hasta la conceptualización de la solución del problema.
- **La meta** es realizar un proceso de diseño basado en una de las historias de usuario entregadas (escoger una sola), y desarrollar:
- **1. Hipótesis:** Acerca de lo que debe tener el sistema, y lo que no debe tener.
- **2. Los elementos del diseño de interacción:**  Que consideres importante para tener en cuenta en la propuesta.
[![AR.js 1.0 Video](https://cloud.githubusercontent.com/assets/252962/23441016/ab6900ce-fe17-11e6-971b-24614fb8ac0e.png)](https://youtu.be/0MtvjFg7tik)

#Para tener en cuenta:
• Puedes escoger todos los elementos o artefactos de diseño que consideres necesarios para completar el sistema de vinculación. • Eres libre de proponer cualquier cosa que tenga que ver con el reto. No te limites, ni contengas tu imaginación. ¡Sé creativo!.

It works on all platforms. Android, IOS and window phone. It run **any browser with WebGL and WebRTC**.
(for IOS, you need to update to ios11)

To try on your phone is only 2 easy steps, check it out!

1. Open this [hiro marker image](https://jeromeetienne.github.io/AR.js/data/images/HIRO.jpg) in your desktop browser.
1. Open this [augmented reality webapps](https://jeromeetienne.github.io/AR.js/three.js/examples/mobile-performance.html) in your phone browser, and point it
to your screen.

**You are done!** It will open a webpage which read the phone webcam, localize a hiro marker and add 3d on top of it, as you can see below.

![screenshot](https://cloud.githubusercontent.com/assets/252962/23072106/73a0656c-f528-11e6-9fcd-3c900d1d47d3.jpg)

# CSS3

So we shown it is now possible to do 60fps web-based augmented reality on a phone.
This is great for sure but how did we get here ? **By standing on the shoulders of giants!**
It is thanks to the hard work from others, that we can today reach this mythic 60fps AR.
So I would like to thank:

- **three.js** for being a great library to do 3d on the web.
- **artoolkit**! years of development and experiences on doing augmented reality
- **emscripten and asm.js**! thus we could compile artoolkit c into javascript
- **chromium**! thanks for being so fast!

Only thanks to all of them, I could do my part : Optimizing performance from 5fps on high-end
phone, to 60fps on 2years old phone.

After all this work done by a lot of people, we have a *web-based augmented reality solution fast enough for mobile*!

Now, many people got a phone powerful enough to do web AR in their pocket.
I think this performance improvement makes web AR a reality.
I am all exited by what people are going to do with it :)

# Javascript

We are still early in the project but here are some initial numbers to give you an idea.

- I got 60fps stable on nexus6p
- Some reports [Sony Xperia Z2 (2.5 years old) runs around 50fps](https://twitter.com/leinadkalpot/status/834121238087925763) - this is a 170euro phone
- Some reports [~50fps on a old nexus5, and ~60fps on nexus 9](https://twitter.com/Ellyll/status/834312442926751744) - nexus5 is 3.5 years old!
- Some reports it working on windows phone edge!! [13fps on Lumia 950](https://twitter.com/leinadkalpot/status/834299384510763012) for some.
  [40-45fps on lumia 930](https://twitter.com/fastclemmy/status/834817155665391616) for others.

Obviously your mileage may vary. The performance you get will depend on 3 things: How heavy your 3D is, How you tune your parameters
and the hardware that you are using.

![screenshot](https://cloud.githubusercontent.com/assets/252962/23068128/40343608-f51a-11e6-8cb3-900e37a7f658.jpg)

# GIT y GITHUB
With this project, we bring more performance to artoolkit.
artoolkit is a software with years of experience doing augmented reality. It is able to do a lot!

It is marker based. It supports a wide range of markers: multiple types of markers [pattern](https://artoolkit.org/documentation/doku.php?id=3_Marker_Training:marker_training)/[barcode](https://artoolkit.org/documentation/doku.php?id=3_Marker_Training:marker_barcode)
multiple independent markers at the same time, or [multiple markers acting as a single marker](https://artoolkit.org/documentation/doku.php?id=3_Marker_Training:marker_multi)
up to you to choose.

# PostgreSQL
Recently, we’ve been getting creative and working on developing new things with AR.js. One of them is playing around with [shadows](https://twitter.com/jerome_etienne/status/837240034847764480), syncing the position of virtual lights with reality for a more life-like finish:
![screen shot 2017-03-16 at 21 06 24](https://cloud.githubusercontent.com/assets/6317076/24018623/7f787ba8-0a8c-11e7-8088-fea4799b5d09.png)

We’ve been collaborating very closely with [Fredrick Blomqvist](https://twitter.com/snigelpaogat). His input has had a great impact on AR.js innovation and we want to thank him. Together, we’ve been implementing [refraction](https://twitter.com/jerome_etienne/status/838749280999518208), giving the 3d a transparent/glassy effect. It ended up having a nice polished look. What do you guys think?
![screen shot 2017-03-06 at 16 31 28](https://cloud.githubusercontent.com/assets/6317076/23832948/9b64c79e-0736-11e7-9cb8-747f6a8fc082.png)

Other crazy ideas we’ve been working on include a [hole in the wall](https://twitter.com/jerome_etienne/status/836754117964017664) and a [portal into another world](https://twitter.com/jerome_etienne/status/838404908235776000). We want to take AR.js to new dimensions.
![screen shot 2017-03-12 at 15 19 51](https://cloud.githubusercontent.com/assets/6317076/23833024/b2e045be-0737-11e7-9ef0-8e1ac9e49ba8.png)
![screen shot 2017-03-07 at 10 08 39](https://cloud.githubusercontent.com/assets/6317076/23833015/947f6abe-0737-11e7-9a0d-1ea919f6ffbe.png)

# Ruby 
- "Shared #ar is a lot more real than solo #AR." - Augmented reality principle [tweet](https://twitter.com/jerome_etienne/status/847889867296124933)
- "The marker must be a portal from where the virtual emerges." by @AndraConnect - #AR principles at dinner 😏 [tweet](https://twitter.com/jerome_etienne/status/842112692211056640)

# Ruby On Rails
- At the three.js level is the main one. It is working well and efficiently
- a-frame component - it export ```<a-marker>``` tag. It becomes real easy to use.
  It allows the things three.js extension does. Here are some slides
  [aframe-artoolkit](http://jeromeetienne.github.io/slides/artoolkit-aframe/)
- webvr-polyfill: it is kind of working - still a work-in-progress

# Angular 5 y Typescript

A-Frame magic :) All details are explained in this super post
["Augmented Reality in 10 Lines of HTML - AR.js with a-frame magic"](https://medium.com/arjs/augmented-reality-in-10-lines-of-html-4e193ea9fdbf)
by
[@AndraConnect](https://twitter.com/AndraConnect).

```html
<!doctype HTML>
<html>
<script src="https://aframe.io/releases/0.6.1/aframe.min.js"></script>
<script src="https://cdn.rawgit.com/jeromeetienne/AR.js/1.5.0/aframe/build/aframe-ar.js"> </script>
  <body style='margin : 0px; overflow: hidden;'>
    <a-scene embedded arjs>
  	<a-marker preset="hiro">
            <a-box position='0 0.5 0' material='color: black;'></a-box>
  	</a-marker>
  	<a-entity camera></a-entity>
    </a-scene>
  </body>
</html>
```

See on [codepen](https://codepen.io/jeromeetienne/pen/mRqqzb) or [bl.ocks.org](https://bl.ocks.org/jeromeetienne/feeb69257803e69f18dc3ea5f4fc6d71)

# Ionic
We started a [AR.js blog](https://medium.com/arjs), thus we can write about
all the crazy ideas related to AR.js.

- ["Area Learning with Multi-Markers in AR.js - For a Larger & More Stable Augmented Reality"](https://medium.com/arjs/area-learning-with-multi-markers-in-ar-js-1ff03a2f9fbe)
  by [@AndraConnect](https://twitter.com/AndraConnect)
- ["WebVR for Augmented Reality - Using WebVR to write cross-platform AR applications"](https://medium.com/arjs/webvr-for-augmented-reality-f1e69a505902)
  by [@jerome_etienne](https://twitter.com/jerome_etienne)
- ["Augmenting The Web Page - Bringing augmenting reality to normal web pages"](https://medium.com/arjs/augmenting-the-web-page-e893f2d199b8)
  by [@jerome_etienne](https://twitter.com/jerome_etienne)
- ["Server Rendering for Augmented Reality - Cloud Rendering with Web Standards"](https://medium.com/arjs/server-rendering-for-augmented-reality-2de0a71aae04)
  by [@jerome_etienne](https://twitter.com/jerome_etienne)
- ["AR-Code:a Fast Path to Augmented Reality - From qrcode to AR.js content"](https://medium.com/arjs/ar-code-a-fast-path-to-augmented-reality-60e51be3cbdf)
  by [@jerome_etienne](https://twitter.com/jerome_etienne)
- ["Augmented Reality in 10 Lines of HTML - AR.js with a-frame magic"](https://medium.com/arjs/augmented-reality-in-10-lines-of-html-4e193ea9fdbf)
  by [@AndraConnect](https://twitter.com/AndraConnect)

# Nginx

- How to write a AR.js application ?
Here is a [full tutorial](https://marmelab.com/blog/2017/06/19/augmented-reality-html5.html)
by [marmelab](https://marmelab.com/) featuring [François Zaninotto](https://twitter.com/francoisz).
It explain how to code a full application on phone! Step by Steps, with explaination and videos.
Very great! the perfect step if you want to start writing AR application today.
- Great post about [WebAR for designer](http://www.nexusinteractivearts.com/webar/)
by [nexus interactive arts](http://www.nexusinteractivearts.com/)

# Postman
[Seminal post](https://medium.com/arjs/augmenting-the-web-page-e893f2d199b8) explaining the concept.
The service is available [webxr.io/augmented-website](https://webxr.io/augmented-website/)

[![Augmented Website](https://user-images.githubusercontent.com/252962/27472386-0d11e59a-57f3-11e7-9fa5-34332c5484f7.png)](https://webxr.io/augmented-website/)


# Examples

Some applications:

- [Pattern Marker Training](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) :
  Generate a [pattern marker](https://artoolkit.org/documentation/doku.php?id=3_Marker_Training:marker_training) with your own image.
- [ARCode Generator](https://jeromeetienne.github.io/AR.js/three.js/examples/arcode.html) :
  Generator of AR-Code
  ([source](https://github.com/jeromeetienne/AR.js/blob/master/three.js/examples/arcode.html))
- [WebAR Playground](https://jeromeetienne.github.io/webar-playground/) :
  Playground running in WebAR with ar.js/chromiumAR

[ALL EXAMPLES](https://jeromeetienne.github.io/AR.js-docs/misc/EXAMPLES.html)

# Folders
- ```/three.js``` is the extension to use it with [pure three.js](https://threejs.org)
- ```/aframe``` is the extension to use it with [a-frame](https://aframe.io)
- ```/webvr-polyfill``` is the WebVR polyfill so you can reuse your #AR / #VR content easily

# Licenses
It is **all open source** ! jsartoolkit5 is under LGPLv3 license and additional permission.
And All my code in AR.js repository is under MIT license. :)

For legal details, be sure to check [jsartoolkit5 license](https://github.com/artoolkit/jsartoolkit5/blob/master/LICENSE.txt)
and [AR.js license](https://github.com/jeromeetienne/AR.js/blob/master/LICENSE.txt).

# Change Log
[CHANGELOG.md](https://github.com/jeromeetienne/AR.js/blob/master/CHANGELOG.md)

# What's Next ?

We did good on performance, but there are still a lot of room for optimisation.
Using [webworkers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers)
would increase cpu usage. Compiling in [webassembly](https://webassembly.org) instead
of [asm.js](http://asmjs.org/) should improve loading time and likely cpu performance.
And obviously, we can still do more parameters tweaking :)


I would like people start experience augmented reality and play with it.
This is highly creative! Just look at this [puzzle game in #AR playing with mirror and laser beam](https://www.youtube.com/watch?v=OzLJb7HitvA).
You could do it with AR.js, so opensource and running on normal phones, no need to buy a new device. isn't that great!


Augmented reality on phone have applications in many fields:
[history education](https://www.youtube.com/watch?v=gyp8ZYtyu_M)
, [science](https://www.youtube.com/watch?v=gMxdBdLpVgc)
or [gaming](https://www.youtube.com/watch?v=kEMDgvfFUcI).
I exited to see what people will do with AR.js :)
