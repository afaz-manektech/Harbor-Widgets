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

#### direction

This parameter is used set the direction for the dropdown.

string | default value: down | possible values: up, down, auto

```html
<div is="search" direction="up"></div>
```

#### label

This parameter is used set the label for the expandable search.

string | default value: null

```html
<div is="search" label="Search your choice"></div>
```

#### button-label

This parameter is used set the label for the search button.

string | default value: null

```html
<div is="search" button-label="Search your choice"></div>
```

#### expandable

This parameter is used set the search widget to expandable.

boolean | default value: false

```html
<div is="search" :expandable="true"></div>
```

#### strict

This parameter instructs the widget to use the provided options striclty instead of session values.

boolean | default value: false

```html
<div is="search" :strict="true"></div>
```

#### load

This parameter is used to update other widgets when the values are updated.

boolean | default value: false

```html
<div is="search" :load="true"></div>
```
