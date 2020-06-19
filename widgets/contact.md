# Contact

Example:
```html
<div is="contact"></div>
```

Parameters:

#### category-id

Load the accommodations of provided category.

number | default value: `null`

```html
<div is="contact" :category-id="1"></div>
```

#### accommodation-id

Load the contact form for the provided accommodation.

number | default value: `null`

```html
<div is="contact" :accommodation-id="1"></div>
```

#### global

Setting this parameter to true will allow updating the selected values as per changes in other global widgets.

boolean | default value: `false`

```html
<div is="contact" :global="true"></div>
```

#### show-search

Show or hide the search widget within contact widget.

boolean | default value: `true`

```html
<div is="contact" :show-search="false"></div>
```

#### url

The url to send user to after the contact form has been successfully submitted.

string | default value: `null`

```html
<div is="contact" url="http://contact-form-submitted.here/thanks-for-interest"></div>
```
