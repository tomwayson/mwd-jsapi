## Dijit, The Good Parts

---

<!-- .slide: data-background="img/binoculars-7271415680_b64ecd8752_z.jpg" -->
#### Ahead of it's time

---

<!-- .slide: data-background="img/binoculars-7271415680_b64ecd8752_z.jpg" -->
#### i18n, a11y, templates

---

<!-- .slide: data-background="img/legos-2253657555_9306374c9f_z.jpg" -->
#### Component (widget) architecture

---

<!-- .slide: data-background="img/app-components.png" -->
#### Modern apps are organized as a tree of components

---

<!-- .slide: data-background="img/lego-jeep.jpg" -->
#### Use [dijit/_WidgetBase](http://dojotoolkit.org/documentation/tutorials/1.10/understanding_widgetbase/) & [dijit/_TemplatedMixin](http://dojotoolkit.org/documentation/tutorials/1.10/templated/)

---

<!-- .slide: data-background="img/claro-theme.png" -->
#### <i class="fa fa-exclamation-triangle"></i> Avoid dijits built-in layout and form widgets

---

<!-- .slide: data-background-color="#fff" data-background="img/internet_explorer_logo_6.png" data-background-size="700px" -->
#### Designed for challenges of a different era

---

<!-- .slide: data-background="img/dijit-markup.png" -->
#### Complicated ~~semantic~~ mark up

---

<!-- .slide: data-background="img/dijit-markup.png" -->
#### Difficult to style

---

<!-- .slide: data-background="img/claro-theme.png" -->
#### Dated themes

---

<!-- .slide: data-background="img/no-phone-16981803257_4bcd3c45dc_z.png" -->
#### Not mobile first

---

<!-- .slide: data-background="img/no-phone-16981803257_4bcd3c45dc_z.png" -->
#### Not responsive

---

<!-- .slide: data-background="img/no-phone-16981803257_4bcd3c45dc_z.png" -->
#### Not touch friendly

---

<!-- .slide: data-background="img/calcite-theme.png" -->
#### For Esri UI components, try new [calcite theme](https://blogs.esri.com/esri/arcgis/2016/03/04/arcgis-api-for-javascript-version-3-16-released/)

---

<!-- .slide: data-background="img/icon-bootstrap.png" data-background-size="650px" -->
#### For rest of app, use a modern UI framework

---

<!-- .slide: data-background="img/icon-bootstrap.png" data-background-size="650px" -->
#### Maybe just markup and CSS

---

<!-- .slide: data-background="img/calcite-bootstrap.png" -->
#### Optionally Use [calcite-bootstrap](http://esri.github.io/calcite-bootstrap/) theme

---

<!-- .slide: data-background="img/calcite-maps.png" -->
#### For map-centric apps layout checkout [calcite maps](http://esri.github.io/calcite-maps/index.html)

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Recommendations 

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## DO use component architecture 

[Create your own widgets](https://developers.arcgis.com/javascript/jshelp/intro_custom_dijit.html) using base classes and mixins
- <i class="fa fa-thumbs-up"></i> [`dijit/_WidgetBase`](http://dojotoolkit.org/documentation/tutorials/1.10/understanding_widgetbase/)
- <i class="fa fa-thumbs-up"></i> [`dijit/_TemplatedMixin`](http://dojotoolkit.org/documentation/tutorials/1.10/templated/)

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## <span style="color: red">DON'T</span> use built-in UI components
- <i class="fa fa-thumbs-down"></i> `dijit/form/...`
- <i class="fa fa-thumbs-down"></i> `dijit/layout/...`

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Instead, pair with a more modern UI library
- <i class="fa fa-thumbs-up"></i> We use [Bootstrap](http://getbootstrap.com/)
- <i class="fa fa-thumbs-up"></i> Consider Esri's [calcite theme](https://blogs.esri.com/esri/arcgis/2016/03/04/arcgis-api-for-javascript-version-3-16-released/) and [calcite-bootstrap](http://esri.github.io/calcite-bootstrap/)
- <i class="fa fa-thumbs-up"></i> For map-centric apps layout checkout [calcite maps](http://esri.github.io/calcite-maps/index.html)
