# Telesto (Accommodations telesto style)

> Used in [Drenthe Campings](https://www.drenthecampings.nl/nl/camping-kiezer)

Example:
```html
<div is="telesto"></div>
```

Parameters:

#### category-id

The category id to load the category.

number | default value: `null`

```html
<div is="telesto" :category-id="1"></div>
```

#### category-item

The apollo javascript category object should be passed as a value. This object will be directly used as data and no additional api request will be made to show the category.

object | default value: `null`

```html
<div is="telesto" :category-item="categoryObject"></div>
```

#### more-info

Enable or disable more info for each accommodation.

boolean | default value: `false`

```html
<div is="telesto" :more-info="true"></div>
```

#### more-info

Enable or disable more info for each accommodation.

boolean | default value: `false`

```html
<div is="telesto" :more-info="true"></div>
```

#### show-accommodations

Show or hide accommodations for each category.

boolean | default value: `true`

```html
<div is="telesto" :show-accommodations="false"></div>
```

#### book-now-buttons

Show the more info button and book now button on accommodations.

> More info button will point to url field in accommodation in harbor.  
> Book now button will point to booking url field in accommodation in harbor.

boolean | default value: `false`

```html
<div is="telesto" :book-now-buttons="true"></div>
```
