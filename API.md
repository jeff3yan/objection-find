# API Reference

<br>
<br>
<br>

## require('objection-find')

#### `findQuery(ObjectionModelConstructor)` -> [FindQueryBuilder](#findquerybuilder)

The function returned by `require('objection-find')` can be used to create a [FindQueryBuilder](#findquerybuilder)
instance. Just pass an [objection.js](https://github.com/Vincit/objection.js/) model constructor to the function 
and start building the query. 

```js
var findQuery = require('objection-find');
var Person = require('./models/Person');
var builder = findQuery(Person);
```

`findQuery(Person)` is just a shortcut for [new findQuery.FindQueryBuilder(Person)](#new-findquerybuilderobjectionmodel-model---findquerybuilder)

#### `findQuery.FindQueryBuilder`

The [FindQueryBuilder constructor](#new-findquerybuilderobjectionmodel-model---findquerybuilder). 
You can use this to create subclasses and whatnot.

<br>
<br>
<br>

## FindQueryBuilder

### Methods

 - [new FindQueryBuilder(ObjectionModelConstructor)](#new-findquerybuilderobjectionmodel-model---findquerybuilder)

##### `new FindQueryBuilder(ObjectionModelConstructor)` -> `FindQueryBuilder`

The constructor.