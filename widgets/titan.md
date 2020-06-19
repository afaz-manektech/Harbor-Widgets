# Titan

Example:
```html
<div is="titan"></div>
```

Parameters:

#### category-id

Provide the category to load the accommodations from.

number | default value: `null`

```html
<div is="titan" :category-id="1"></div>
```

#### accommodation-id

Create titan widget for the specified accommodation.

number | default value: `null`

```html
<div is="titan" :accommodation-id="1"></div>
```

#### global

Setting this parameter to true will allow updating the selected values as per changes in other global widgets.

boolean | default value: `false`

```html
<div is="titan" :global="true"></div>
```

#### metrics

Update the accommodation counter matrics on the server when the widget is viewed.

boolean | default value: `false`

```html
<div is="titan" :metrics="true"></div>
```

#### url

Custom url for request information (Informatie aanvragen) button.

string | default value: `null`

```html
<div is="titan" url="http://custom-url.here"></div>
```

#### direction

The direction on which side the price receipt will open.

string | default value: `right`

```html
<div is="titan" direction="left"></div>
```

#### override-url

Specify url to override default pandora url. The override url will be generated with same parameters as pandora url.

string | default value: `null`

```html
<div is="titan" override-url="http://some-other-url.somewhere/book-from-here"></div>
```

#### override-label

Specify the label to be used with override-url.

string | default value: `null`

```html
<div is="titan" override-label="Book from some-other-page" override-url="http://some-other-url.somewhere/book-from-here"></div>
```

#### show-booklink

Show or hide the default book button with original pandora url when override-url is used.

boolean | default value: `false`

```html
<div is="titan" :show-booklink="true" override-url="http://some-other-url.somewhere/book-from-here"></div>
```
