# Aims

- To create a debugging tool which reads html creates a 3d debug layer

## Ideas / Potiential
- Could be a console tab tool similar to react tools in browser

## Elements
  - Container 
	  - (a plain container) moddable/codable
		+ Receives Css + JS
	- Element (a html element class base)
	- renderer (a container which styles itself like the css)
	- Background
	- View Switcher
	- Popup Box 
	  - A generic box for details display

## Libraries / Features
	Now
  - Something to read the html / js / css
	- React-three-fiber
	- [Sixel](https://github.com/jerch/node-sixel)
	- [Puppeteer ](https://github.com/puppeteer/puppeteer#readme)
	Future
	- Understand Vue + React
	- Mouse Handling
	- Electron / [neutralino]
	- irohjs ??

## How it goes
First: a file is handed to the cli
NodeLayers <file>

Second: the file is read: html, css, js
	- reading with iroh??
	- how to read html / xml documents
	  - create from inside element outward
		**data points**
		- containers
		- space between
		- level (data graph depth)
		- peak item
		- Popup box (css + js details per element)

Third: a threejs scene is created
	- Create views
	- Create Background
	- Read from step 2 (get html, associated css + js)
	  - create objects for each step 2 **data point**

Fourth: a sixel image is created
	- 

Now
	- [Example](https://github.com/jherr/iterm-graphics/blob/master/react-to-sixel/src/index.js)
	- Setup project
Future:
	- Interactive Version with hover + electron

