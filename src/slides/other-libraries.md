## Working with Other Libraries

---

<!-- .slide: data-background="img/module-loading1.png" data-background-size="578px" data-background-color="#fff" -->
#### Dojo uses Asynchronous Module Definition (AMD)

---

<!-- .slide: data-background="img/different-7519496646_2bef924538_z.jpg" -->
#### Dojo implements AMD differently than others

---

<!-- .slide: data-background="img/oneway-4143717993_db54d25c2e_z.jpg" -->
#### Module loading in Dojo is a one way street

---

<!-- .slide: data-background="img/oneway-4143717993_db54d25c2e_z.jpg" -->
#### Can't load Esri/Dojo modules from other AMD loaders

---

<!-- .slide: data-background="img/oneway-4143717993_db54d25c2e_z.jpg" -->
#### You *can* load other libraries with Dojo's AMD loader

---

<!-- .slide: data-background="reveal.js/img/bg-1.png" -->
## You can do this, but...

<table class="logos">
	<tr>
		<td colspan="2"><img src="img/Logo_D3.svg.png" class="transparent" width="100" /></td>
		<td colspan="2"><img src="img/icon-bootstrap.png" class="transparent" height="100" /></td>
	</tr>
	<tr>
		<td><img src="img/lodash-logo.png" class="transparent" width="100" /></td>
		<td colspan="2"><img src="img/dojo-blue-circle.png" class="transparent" height="240" width="240" /></td>
		<td><img src="img/jquery_bumper.sh.png" class="transparent" height="100" /></td>
	</tr>
	<tr>
		<td colspan="2"><img src="img/Backbone_logo_logo_only.png" class="transparent" width="100" /></td>
		<td colspan="2"><img src="img/react-logo.png" class="transparent" width="100" /></td>
	</tr>
</table>

... redundant & heavy page weight

---

<!-- .slide: data-background="img/scales-7953227784_416ff3d16f_o.jpg" -->
#### Everything is a trade-off

---

<!-- .slide: data-background="img/scales-7953227784_416ff3d16f_o.jpg" -->
#### Page wieght vs. functionality <i class="fa fa-thumbs-up"></i>

---

<!-- .slide: data-background="img/scales-7953227784_416ff3d16f_o.jpg" -->
#### Page wieght vs. developer productivity <i class="fa fa-question-circle"></i>

---

<!-- .slide: data-background="img/dojo-config-packages.png" -->
#### Configure Dojo [loader packages](https://dojotoolkit.org/documentation/tutorials/1.10/dojo_config/#loader-configuration)


---

<!-- .slide: data-background="img/dojo-config-packages.png" -->
#### Specify `main` other than 'index.js'

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Recommendations 

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Use Dojo's AMD loader to load:
- <i class="fa fa-check-square-o"></i> Your own AMD modules
- <i class="fa fa-check-square-o"></i> 3rd Party UMD and AMD modules
- <i class="fa fa-check-square-o"></i> Esri/Dojo modules

---

<!-- .slide: data-background="reveal.js/img/bg-3.png" -->
## Be selective about the libraries you add
- <i class="fa fa-info-circle"></i> Check if Dojo already did that (it's already on the page)
- <i class="fa fa-thumbs-up"></i> Use for functional gaps (like mobile-first UI components)
- <i class="fa fa-question-circle"></i> Decide if it's worth any gains in developer productivity
- <i class="fa fa-thumbs-down"></i> Don't add libraries just because they're trendy
