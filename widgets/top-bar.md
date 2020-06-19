# Top / Bottom Bar

Example:
```html
<div is="top-bar"></div>
```

Parameters:

#### category-id

Load the accommodations of provided category.

number | default value: `null`

```html
<div is="top-bar" :category-id="1"></div>
```

#### accommodation-id

Load the top bar for the provided accommodation.

number | default value: `null`

```html
<div is="top-bar" :accommodation-id="1"></div>
```

#### global

To update the values globally.

boolean | default value: `false`

```html
<div is="top-bar" :global="true"></div>
```

#### show-categories

Show or hide the categories in the top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-categories="false"></div>
```

#### show-accommodations

Show or hide the accommodations in the top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-accommodations="false"></div>
```

#### show-when

Show top bar when selector dom element is available in dom.

string | default value: `null`

```html
<div is="top-bar" show-when="#zb-titan"></div>
```

#### url

Provide the custom url for booking.

string | default value: `null`

```html
<div is="top-bar" url="http://booking-page.here/book"></div>
```

#### position

Set the position of bar.

> Possible values  
> `top` | `bottom`

string | default value: `top`

```html
<div is="top-bar" position="bottom"></div>
```

#### override-url

Provide the override url to override pandora url.

string | default value: `null`

```html
<div is="top-bar" override-url="http://some-other-page.here/book"></div>
```

#### override-label

Provide the override label when override url is added.

string | default value: `null`

```html
<div is="top-bar" override-label="Book from some other page" override-url="http://some-other-page.here/book"></div>
```

#### enable-search

Show or hide the search within top bar.

boolean | default value: `true`

```html
<div is="top-bar" :enable-search="false"></div>
```

#### show-persons

Show or hide the person selector within top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-persons="false"></div>
```

#### show-packages

Show or hide the packages within top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-packages="false"></div>
```

#### show-button

Show or hide the book button within top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-button="false"></div>
```

#### show-dates

Show or hide the calendars within top bar.

boolean | default value: `true`

```html
<div is="top-bar" :show-dates="false"></div>
```