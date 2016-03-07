## The Modern Dojo Toolchain

---

<!-- .slide: data-background="img/babel.png" data-background-size="744px" -->
#### Babel: ES2015 modules => AMD (livereload &amp; build) 

---

<!-- .slide: data-background="img/babel.png" data-background-size="744px" -->
#### Use the [transform-es2015-modules-amd](https://babeljs.io/docs/plugins/transform-es2015-modules-amd/) plugin

---

<!-- .slide: data-background="img/assembly-line-2994043188_4e9ccbcb3f_z.jpg" -->
#### Must use [Dojo's build](https://dojotoolkit.org/reference-guide/1.10/build/) tool to optimize (no WebPack)

---

<!-- .slide: data-background="img/tesla-6858583426_1f003ea519_z.jpg" -->
#### Add [Bower](http://bower.io/)/[Grunt](http://gruntjs.com/)/[Babel](https://babeljs.io/) for more modern workflow

---

<!-- .slide: data-background="img/tesla-6858583426_1f003ea519_z.jpg" -->
#### Grunt+ESLint+SASS+Babel+[Dojo build](https://dojotoolkit.org/reference-guide/1.10/build/) &cong; WebPack

---

<!-- .slide: data-background-color="#fff" data-background="img/bower-logo.png" data-background-size="512px" -->
#### Get local Esri modules from [JSAPI Bower release](https://github.com/Esri/jsapi-resources/tree/master/bower)

---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Use [grunt-dojo](https://www.npmjs.com/package/grunt-dojo) to include in your build pipeline


---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Do <span style="color: red">NOT</span> build Dojo as part of livereload

---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Livereload serves local unbuilt modules and/or [CDN](http://js.arcgis.com/)

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Recommendations 

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Use [Babel](https://babeljs.io/) to transpile ES2015 to ES5 AMD 
- <i class="fa fa-thumbs-up"></i> Use the [transform-es2015-modules-amd  plugin](https://babeljs.io/docs/plugins/transform-es2015-modules-amd/)
- <i class="fa fa-hand-o-right"></i> Pro-tip: use [babel-plugin-transform-es2015-modules-simple-amd](https://www.npmjs.com/package/babel-plugin-transform-es2015-modules-simple-amd) <br />for code that will run in other Dojo apps (like Web AppBuilder)

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Optimize (build) apps with large code bases 
- <i class="fa fa-thumbs-up"></i> Use [Dojo build](https://dojotoolkit.org/reference-guide/1.10/build/) with the [Bower release of the JSAPI](https://github.com/Esri/jsapi-resources/tree/master/bower)
- <i class="fa fa-hand-o-right"></i> Pro-tip: use [`layerOptimize: 'uglify'`](https://dojotoolkit.org/reference-guide/1.10/build/transforms/writeOptimized.html#id4) with 3rd party libs <br />(closure defaults to ES3, throws compile errors on ES5 code)
- <i class="fa fa-thumbs-up"></i> Use [grunt-dojo](https://www.npmjs.com/package/grunt-dojo) to include build step in grunt pipeline

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Related Talks
<div>
<img src="img/bower-logo.png" class="transparent" width="128" />
<img src="img/babel.png" class="transparent" width="188" />
<img src="img/grunt-logo.png" class="transparent" width="128" />

</div>

Modern Tools for the Modern Web Developer [Thu @ 1:00PM](https://devsummit.schedule.esri.com/#schedule/56b2874a4be5dd46a30002e9/56b2874a4be5dd46a30002ea)

<small>Joshua Peterson, Gavin Rehkemper</small>

Automating Builds for Enterprise JavaScript Applications [Thu @ 2:30PM](https://devsummit.schedule.esri.com/#schedule/56b2874f4be5dd46a300030e/56b4eff34be5dd8f3401d266)

<small>George Bochenek, Randy Jones</small>

Optimizing Your JavaScript App for Performance [Thu @ 2:30PM](https://devsummit.schedule.esri.com/#schedule/56b287444be5dd46a30002b7/56b287444be5dd46a30002b8)

<small>Lloyd Heberlie, Rene Rubalcava</small>

