# JavaScript 30 #14: JavaScript-Reference-vs-Copy
This is the fourteenth project of JavaScript30 Challenge. </br></br>
This repo is for understanding difference between copying by value and reference in primitive data types, objects and arrays </br>
## Features & Usage
- Array copy methods </br>
```javascript
const copy = modelArray.slice(); 
const copy = [].concat(modelArray);
const copy = [...modelArray]; 
const copy = Array.from(modelArray); 
```
- Object copy methods
```javascript
const copy = Object.assign({}, modelObject, {property : newValue});
const copy = {...modelObject};
```
- Usage of deep clone methods to copy deeper levels of the object
```javascript
const deepCopy = JSON.parse(JSON.stringify(modelObject)); 
//lodash library
const _ = require('lodash');
const deepCopy = _.cloneDeep(modelObject);
```


