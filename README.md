# Inspector Dom

Pure vanilla-js ultra-lightweight dom inspector similiar to built-in tool in chrome browser with a custom callback onClick.
![](inspector.gif)

## Install

yarn add inspector-dom

`const Inspector = require('inspector-dom')`

`import Inspector from 'inspector-dom'`

## Usage

Initialize:

`const inspector = Inspector()`

Props:

```javascript
const inspector = Inspector({
    root: 'body',                       // root element
    excluded: [],                       // excluded children, string or node Element
    outlineStyles: '2px solid orange',  // styles
    onClick: el => console.log('Element was clicked:', constructCssPath(el)
});
```

## API

`inspector.enable(callback)             // turn the inspector on`

`inspector.cancel()                     // turn the inspector off`
