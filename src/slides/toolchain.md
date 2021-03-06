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
#### Get local Esri modules from [JSAPI Bower release](https://developers.arcgis.com/javascript/jshelp/inside_bower_custom_builds.html)

---

<!-- .slide: data-background-color="#fff" data-background="img/bower-logo.png" data-background-size="512px" -->
#### > `bower install arcgis-js-api`

---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Use [grunt-dojo](https://www.npmjs.com/package/grunt-dojo) to include in your build pipeline

---

<!-- .slide: data-background-color="#fff" data-background="img/gulp-grunt.png" data-background-size="273px" -->
#### Use [gulp-grunt](https://www.npmjs.com/package/gulp-grunt) to include in gulp pipeline

---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Do <span style="color: red">NOT</span> build Dojo as part of livereload

---

<!-- .slide: data-background-color="#fff" data-background="img/grunt-logo.png" data-background-size="512px" -->
#### Livereload serves local unbuilt modules and/or [CDN](http://js.arcgis.com/)

---

<!-- .slide: data-background="img/scantron-7674804806_7bd5ff8688_z.jpg" -->
#### Testing your code

---

<!-- .slide: data-background="img/intern.png" data-background-color="#fff" data-background-size="236px" -->
#### Dojo's own testing library: [the Intern](https://theintern.github.io/)

---

<!-- .slide: data-background="img/karma-logo.png" data-background-color="#fff" data-background-size="730px" -->
#### If you need to fine tune the knobs: [Karma](https://karma-runner.github.io)

---

<!-- .slide: data-background="img/karma-logo.png" data-background-color="#fff" data-background-size="730px" -->
#### Checkout [yo karma-esri](https://www.npmjs.com/package/generator-karma-esri)

---

<!-- .slide: data-background="img/scantron-7674804806_7bd5ff8688_z.jpg" -->
#### See our talk from [DevSummit 2015](https://github.com/tomwayson/esri-js-testing-tools-and-patterns)

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
- <i class="fa fa-thumbs-up"></i> Use [Dojo build](https://dojotoolkit.org/reference-guide/1.10/build/) with the [Bower release of the JSAPI](https://developers.arcgis.com/javascript/jshelp/inside_bower_custom_builds.html)
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

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## More Related Talks
<div>
<img src="img/TypeScript_Logo.png" class="transparent" width="220" />
</div>

Using Modern ES6 and TypeScript Features on Top of Dojo 1.x [Wed @ 4:00PM](https://devsummit.schedule.esri.com/#schedule/56b3c9904be5dd6b69003dd3/56b3cd784be5dd8f340141a5)

<small>Dylan Schiemann</small>

Using TypeScript with ArcGIS JS API Development [Thu @ 5:30PM](https://devsummit.schedule.esri.com/#schedule/56b2874f4be5dd46a3000310/56b287504be5dd46a3000311)

<small>Rene Rubalcava, Dasa Paddock</small>

Full Stack End to End JavaScript Testing with Intern [Thu 4:00PM](https://devsummit.schedule.esri.com/#schedule/56b3ca044be5dd8f34014154/56b4e9874be5dd8f3401ccf6)

<small>Dylan Schiemann</small>

Javascript Applications for the Enterprise: Test More, Work Less [Fri @ 1:00PM](https://devsummit.schedule.esri.com/#schedule/56b2875a4be5dd46a3000356/56b3da974be5dd8f34014544)

<small>George Bochenek, Randy Jones</small>
