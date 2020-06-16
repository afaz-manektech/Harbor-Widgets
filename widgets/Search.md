# Search

Example:
```html
<div is="search"></div>
```

Parameters:
#### config

This parameter is used to pass the configuration.

Each possible values accepts boolean values (true/false).

object | default value: `{ generalCategories: true, categories: true, arrival: true, button: true }`

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

string | default value: `down` | possible values: `up, down, auto`

```html
<div is="search" direction="up"></div>
```

#### label

This parameter is used set the label for the expandable search.

string | default value: `null`

```html
<div is="search" label="Search your choice"></div>
```

#### button-label

This parameter is used set the label for the search button.

string | default value: `null`

```html
<div is="search" button-label="Search your choice"></div>
```

#### expandable

This parameter is used set the search widget to expandable.

boolean | default value: `false`

```html
<div is="search" :expandable="true"></div>
```

#### strict

This parameter instructs the widget to use the provided options striclty instead of session values.

boolean | default value: `false`

```html
<div is="search" :strict="true"></div>
```

#### load

This parameter is used to update other widgets when the values are updated.

boolean | default value: `false`

```html
<div is="search" :load="true"></div>
```

#### pre-fill

This parameter is used make the inputs prefilled with first available values.

boolean | default value: `false`

```html
<div is="search" :pre-fill="true"></div>
```

#### url

This parameter is used to set the url of page where the user should be directed to on clicking search button (zoek).

string | default value: `null`

```html
<div is="search" url="/overview"></div>
```

#### global

This parameter is used to make the changes globally (In other global widgets) when values are changed in the Search widget.

boolean | default value: `false`

```html
<div is="search" :global="true"></div>
```

#### category-id

This parameter is used to limit the search maximum person and calendars limited to the provided category.

number | default value: `null`

```html
<div is="search" :category-id="1"></div>
```

#### period-id

This parameter is used to limit the search periods to provided period ids.

array | default value: `null`

```html
<div is="search" :period-id="[1,2]"></div>
```

#### given

This parameter is used to pre set the values of category, accommodation, period in the Search widget.

object | default value: `{category: null, accommodation: null, period: null}`

```html
<div is="search" :given="{category:1,accommodation:2}"></div>
```

#### filtered

This parameter is used to set the filtered categories. Categories set through this parameter will only be available in the Search widget.

array | default value: `null`

```html
<div is="search" :filtered="[1,2]"></div>
```

#### filters

This parameter is used to pre set the value for the filters. The parameter accepts object with key value form where key is the id of filter and value is 0 (filter not applied), 1 (filter applied).

object | default value: `null`

```html
<div is="search" :filters="{21:1}"></div>
```

#### min-people

This parameter is used to set the minimum value for a person type in Search person selector.

object | default value: `null`

```html
<div is="search" :min-people="{1:3}"></div>
```

#### default-people

This parameter is used to set the default values for person types in Search person selector if the value is not set for each person type.

object | default value: `null`

```html
<div is="search" :default-people="{1:3}"></div>
```

#### override-people

This parameter is used to override the person type value whenever the Search widget is loaded. It will ignore any remembered person type value and set the ones provided through this parameter.

object | default value: `null`

```html
<div is="search" :override-people="{1:3}"></div>
```

#### date-format

This parameter is used to provide standalone date format function for Search widget date. The parameter accepts a javascript function which accepts an argument of javascript date object or string.

function | default value: `null`

```html
<div is="search" :date-format="function(date) { return functionFromDomJs(date, 'DD-MM-YYYY'); }"></div>
```

#### map-widget

This parameter is used to load the accommodations in search widget as standalone elements so the user can click a button and open the map selection.

*This is a work in progress thing.*

boolean | default value: `false`

```html
<div is="search" :map-widget="true"></div>
```

#### accommodation-theme

This parameter is used to load the accommodations in search widget as standalone elements so the user can click a button and open the map selection.
This parameter sets the theme for the accommodations in the dropdown list.

*This is a work in progress thing.*

string | default value: `normal` | possible values: `normal, alternative`

```html
<div is="search" accommodation-theme="alternative"></div>
```

#### search-filters

This parameter is used to set the search filter for the Search widget. The parameter accepts the key value form where key is the id of filter and the value is boolean 0 or 1. 
An example of this can be seen on Greencamp site.

object | default value: `null`

```html
<div is="search" :search-filters="{21:1}"></div>
```

#### search-category

This parameter is used to set category for specifically search widget. The category set here will be on higher priority to be selected on the search widget.

number | default value: `null`

```html
<div is="search" :search-category="1"></div>
```