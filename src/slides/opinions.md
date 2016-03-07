## Some (Free) Opinions on Structuring Dojo Applications

---

<!-- .slide: data-background="img/geese-2995630668_8586f49388_z.jpg" -->
#### JavaScript is a loosey goosey language

---

<!-- .slide: data-background="img/v-formation-362132093_b628e0fcd0_z.jpg" -->
#### Apps and teams benefit from some direction

---

<!-- .slide: data-background="img/starting-line-2520731995_ff1aa83e88_z.jpg" -->
#### Boilerplates are a starting point

---

<!-- .slide: data-background="img/starting-line-2520731995_ff1aa83e88_z.jpg" -->
#### At a minimum, use the official [Dojo Boilerplate](https://github.com/csnover/dojo-boilerplate)

---

<!-- .slide: data-background="img/starting-line-2520731995_ff1aa83e88_z.jpg" -->
#### Makes Dojo build configuration easier

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Style guides add consistency, help productivity

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Modern style guides _should_ be about best practices

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Official [Dojo style guide](https://dojotoolkit.org/reference-guide/1.10/developer/styleguide.html) is about syntax/formatting <i class="fa fa-frown-o"></i>

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Instead use favorite linter/rules ([ESLint](http://eslint.org/), [semistandard](https://github.com/Flet/semistandard))

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### <i class="fa fa-hand-o-right"></i>Esri's [jshint](https://github.com/Esri/jsapi-resources/tree/master/jshint) is OK for ES5, but not for ES2015

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Esri publishes a [coding guidelines](https://developers.arcgis.com/javascript/jshelp/inside_guidelines.html) section in docs

---

<!-- .slide: data-background="img/victorians-16506407390_49868a6e69_z.jpg" -->
#### Tom's [unofficial ArcGIS API for JavaScript Styleguide](https://github.com/tomwayson/mwd-jsapi/tree/master/arcgis-js-style-guide)

---

<!-- .slide: data-background="img/scaffold-2520054449_b8d243d857_z.jpg" -->
#### Generators scaffold out boilerplate code for us

---

<!-- .slide: data-background="img/scaffold-2520054449_b8d243d857_z.jpg" -->
#### There is a generator for Dojo boilerplate, but...

---

<!-- .slide: data-background="img/scaffold-2520054449_b8d243d857_z.jpg" -->
#### Use  [yo arcgis-js-app](https://github.com/odoe/generator-arcgis-js-app)

---

<!-- .slide: data-background="img/scaffold-2520054449_b8d243d857_z.jpg" -->
#### Includes: [Bower](http://bower.io/), [Grunt](http://gruntjs.com/), [Babel](https://babeljs.io/), [ESLint](http://eslint.org/), [Stylus](http://stylus-lang.com/) ...

---

<!-- .slide: data-background="img/scaffold-2520054449_b8d243d857_z.jpg" -->
#### To scaffold out a single widget: [yo esri-widget](https://github.com/tomwayson/generator-esri-widget)


---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Recommendations 
- <i class="fa fa-check-square-o"></i> Use the [Dojo Boilerplate](https://github.com/csnover/dojo-boilerplate)
- <i class="fa fa-check-square-o"></i> Use favorite linter/rules ([ESLint](http://eslint.org/), [semistandard](https://github.com/Flet/semistandard)) for syntax/formatting
- <i class="fa fa-check-square-o"></i> Check out some generators, try out their opinions, modify w/ your own
