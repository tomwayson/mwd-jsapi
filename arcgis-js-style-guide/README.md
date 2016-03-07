# ArcGIS API for JavaScript Style Guide

These are some best practices around organization and architecture of ArcGIS API for JavaScript applications. These are based on my own experience developing Dojo applications.

These opinions are my own. Fork and use as you see fit. Or don't. [Pull requests](https://github.com/tomwayson/mwd-jsapi/pulls) are welcome!

## Application Architecture and State

1. Organize app as a tree of components (widgets) and [singleton](http://www.anujgakhar.com/2013/08/29/singletons-in-dojo/) services
2. State should only be stored in the map and/or Dojo/store(s), which are exposed via singleton services
3. Components get their state by either:
  - data passed down tree as properties
  - public properties/methods of injected singleton services (i.e. authService)
4. Components communicate desired changes to state up through events or topics
  1. Only one module (app) should be allowed to subscribe to topics (i.e. topics are just a shortcut to top of the tree)
5. Limit components that have direct access to sources of state (i.e. smart vs dumb components)
6. only one module (mapService) should should have access to map/view
7. Dependencies should be pushed to edges of the app
  1. Only one module (mapService) should should load and use Esri modules
  2. Same w/ other libs (i.e. only chartService has access to d3, etc)

## Folder and File Structure

1. Follow the folder structure of the [Dojo Boilerplate](https://github.com/csnover/dojo-boilerplate) - this makes builds easier
2. One module per file

## Code Syntax and Formatting 

I prefer 2 spaces with semi-colons, but that's neither here nor there. Use your own opinions enforced by your favorite linter for syntax and formatting. I like [ESLint](http://eslint.org/) or [semistandard](https://github.com/Flet/semistandard).
