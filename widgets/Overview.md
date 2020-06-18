# Overview

Example:
```html
<div is="overview"></div>
```

Parameters:

#### load

This parameter is used to configure if the data in widget should be loaded when the values are retrieved.

boolean | default value: `true`

```html
<div is="overview" :load="true"></div>
```

#### expandable

This parameter is used set the search widget to expandable.

boolean | default value: `false`

```html
<div is="overview" :expandable="true"></div>
```

#### alternatives

Use this parameter to load alternative accommodations within the widget.

boolean | default value: `false`

```html
<div is="overview" :alternatives="true"></div>
```

#### light

Use this parameter to load overview as overview light.

boolean | default value: `false`

```html
<div is="overview" :light="true"></div>
```

#### show-search

Use this parameter to enable or disable the search widget within the overview.

boolean | default value: `true`

```html
<div is="overview" :show-search="false"></div>
```

#### show-person-price

Use this parameter to show or hide per person price in accommodations.

boolean | default value: `false`

```html
<div is="overview" :show-person-price="true"></div>
```

#### show-map-price

Use this parameter to show or hide price in the map container.

boolean | default value: `false`

```html
<div is="overview" :show-map-price="true"></div>
```

#### notification

Use this parameter to show notifications.

boolean | default value: `false`

```html
<div is="overview" :notification="true"></div>
```

#### config

Use this parameter to show notifications.

Each possible values accepts boolean values (true/false).

object | default value: `{ top: true, categories: true, arrival: true, departure: true, filter: void 0 }`

##### Possible values:

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
<div is="overview" :config="{ categories: false, accommodations: true }"></div>
```

#### offset

Use this parameter to add or reduce offset when autoscroll is performed after fetching data. The offset can be any integer with either nagative or positive signed.

> Both of these are valid `:offset="200"` and `:offset="-200"`

number | default value: `0`

```html
<div is="overview" :offset="200"></div>
```

#### notification-steps

This parameter is used to measure the notification steps progress.

number | default value: `25`

```html
<div is="overview" :notification-steps="10"></div>
```

#### offset-initial

Use this parameter to disable autoscroll after initially widget is loaded.

boolean | default value: `true`

```html
<div is="overview" :offset-initial="false"></div>
```

#### category-id

Use the category id to limit overview/overview light widget to a particular category. The id here is the id of the category from harbor backend.

number | default value: `null`

```html
<div is="overview" :category-id="1"></div>
```

#### filtered-categories

This parameter is used to set the filtered categories. Categories set through this parameter will only be available in the Search widget.

array | default value: `null`

```html
<div is="overview" :filtered-categories="[1,2]"></div>
```

#### default-people

This parameter is used to set the default values for person types in Search person selector if the value is not set for each person type.

object | default value: `null`

```html
<div is="overview" :default-people="{1:3}"></div>
```

#### default-people-light

> Usage unknown

object | default value: `null`

```html
<div is="overview" :default-people-light="{1:3}"></div>
```

#### override-people

This parameter is used to override the person type value whenever the Search widget is loaded. It will ignore any remembered person type value and set the ones provided through this parameter.

object | default value: `null`

```html
<div is="overview" :override-people="{1:3}"></div>
```

#### pre-fill

This parameter is used make the inputs prefilled with first available values.

boolean | default value: `false`

```html
<div is="overview" :pre-fill="true"></div>
```

#### filters

This parameter is used to pre set the value for the filters. The parameter accepts object with key value form where key is the id of filter and value is 0 (filter not applied), 1 (filter applied).

object | default value: `null`

```html
<div is="overview" :filters="{21:1}"></div>
```

#### theme

Use this parameter to set the theme for the accommodation widget within the overview.

> Possible values  
> `normal` | `alternative`

string | default value: `normal`

```html
<div is="overview" theme="alternative"></div>
```

#### marker

Specify the image url for the markers on map container.

string | default value: `/images/marker.png`

```html
<div is="overview" marker="http://external.com/images/marker.png"></div>
```

#### color

Specify the color for the clusters on map container.

string | default value: `#77873c`

```html
<div is="overview" color="#fff"></div>
```

#### accommodation-book-now-buttons

Show the more info button and book now button on accommodations.

> More info button will point to url field in accommodation in harbor.  
> Book now button will point to booking url field in accommodation in harbor.

boolean | default value: `false`

```html
<div is="overview" :accommodation-book-now-buttons="true"></div>
```

#### show-features

Show or hide features in accommodations.

boolean | default value: `true`

```html
<div is="overview" :show-features="false"></div>
```

#### show-information

Show or hide information in accommodations.

boolean | default value: `false`

```html
<div is="overview" :show-information="true"></div>
```

#### overlay

Loads the overview as overlay.

> This is a work in progress thing.

boolean | default value: `false`

```html
<div is="overview" :overlay="true"></div>
```

#### more-info-link-target

Specify the target for more info button. Should be used with `:accommodation-book-now-buttons="true"`

> Possible values  
> `_blank` | `_parent` | `_self` | `_top`

string | default value: `_blank`

```html
<div is="overview" :accommodation-book-now-buttons="true" more-info-link-target="_self"></div>
```

#### default-order

Load the accommodations in the order which is set in Harbor. By default the widget will try to load accommodations by sorting them according to maximum_people value for each accommodation.

boolean | default value: `false`

```html
<div is="overview" :default-order="true"></div>
```

#### book-now-reserve-button

Enable or disable book now reserve button when book now buttons are enabled. Should be used with `:accommodation-book-now-buttons="true"`

boolean | default value: `true`

```html
<div is="overview" :accommodation-book-now-buttons="true" :book-now-reserve-button="false"></div>
```

#### book-now-more-info-button

Enable or disable more info button when book now buttons are enabled. Should be used with `:accommodation-book-now-buttons="true"`

boolean | default value: `true`

```html
<div is="overview" :accommodation-book-now-buttons="true" :book-now-more-info-button="false"></div>
```

#### search-filters

This parameter is used to set the search filter for the Search widget. The parameter accepts the key value form where key is the id of filter and the value is boolean 0 or 1. 
An example of this can be seen on Greencamp site.

object | default value: `null`

```html
<div is="overview" :search-filters="{21:1}"></div>
```
