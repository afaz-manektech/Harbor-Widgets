# Bar

The standalone bar with search widget.

Example:
```html
<div is="bar"></div>
```

Parameters:

#### category-id

Create standalone bar for the provided category.

number | default value: `null`

```html
<div is="bar" :category-id="1"></div>
```

#### accommodation-id

Create standalone bar for the provided accommodation.

number | default value: `null`

```html
<div is="bar" :accommodation-id="1"></div>
```

#### global

To update the values globally.

boolean | default value: `false`

```html
<div is="bar" :global="true"></div>
```