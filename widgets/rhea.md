# Rhea (Price matrix)

Example:
```html
<div is="rhea"></div>
```

Parameters:

#### category-id

Show price matrix for the provided category.

number | default value: `null`

```html
<div is="rhea" :category-id="1"></div>
```

#### accommodation-id

Show price matrix for the provided accommodation.

number | default value: `null`

```html
<div is="rhea" :accommodation-id="1"></div>
```

#### period-id

Load the price matrix for the specified period. The paramter accepts id of period from harbor backend.

number | default value: `null`

```html
<div is="rhea" :period-id="1"></div>
```

#### search-period-id

This parameter is used to limit the search periods to provided period ids.

array | default value: `null`

```html
<div is="rhea" :search-period-id="[1,2]"></div>
```

#### overview-link

Specify the link for the overview of the packages.

string | default value: `null`

```html
<div is="rhea" overview-link="http://your.site/link"></div>
```

#### show-price

Show or hide the price reciept besides the price matrix.

boolean | default value: `true`

```html
<div is="rhea" :show-price="false"></div>
```

#### small

Loads small price matrix.

boolean | default value: `false`

```html
<div is="rhea" :small="true"></div>
```

#### global

This parameter is used to make the changes globally (In other global widgets) when values are changed.

boolean | default value: `false`

```html
<div is="rhea" :global="true"></div>
```

#### nights

Load the period by specifying the nights. The widget will load matching period from harbor.

number | default value: `null`

```html
<div is="rhea" :nights="3"></div>
```

#### first

Specify the first date to load price matrix for and after.

string | default value: `null`

```html
<div is="rhea" first="2020-06-18"></div>
```

#### direction

Specify the first date to load price matrix for and after.

> Possible values  
> `left` | `right`

string | default value: `right`

```html
<div is="rhea" direction="left"></div>
```

#### override-people

This parameter is used to override the person type value. It will ignore any remembered person type value and set the ones provided through this parameter.

object | default value: `null`

```html
<div is="rhea" :override-people="{1:3}"></div>
```
