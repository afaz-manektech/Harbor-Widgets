# Search

Example:
```html
<div is="search"></div>
```

Parameters:
#### config

This parameter is used to pass the configuration.

Each possible values accepts boolean values (true/false).

object | default value: { generalCategories: true, categories: true, arrival: true, button: true }

##### possible values:

* accommodations 
* accommodation 
* top 
* categories 
* generalCategories 
* periods 
* months 
* arrival 
* departure 
* button 
* filter 
* prices 
* people 
* showDates

```html
<div is="search" :config="{ categories: false, accommodation: false, button: false }"></div>
```
