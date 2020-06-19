# Calypso

The standalone accommodation widget which loads accommodation from harbor.

Example:
```html
<div is="calypso"></div>
```

Parameters:

#### accommodation-id

The accommodation id from harbor.

number | default value: `null`

```html
<div is="calypso" :accommodation-id="1"></div>
```

#### global

To update the accommodation as per selection in other global widgets.

boolean | default value: `false`

```html
<div is="calypso" :global="true"></div>
```