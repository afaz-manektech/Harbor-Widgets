# Overview Packages

Example:
```html
<div is="overview-packages"></div>
```

Parameters:

#### category-id

Filter the packages for the provided accommodation category(s).

array / number | default value: `null`

```html
<div is="overview-packages" :category-id="[1,2]"></div>
```
**or**
```html
<div is="overview-packages" :category-id="1"></div>
```

#### package-category-id

Filter the packages for the provided package category(s).

array / number | default value: `null`

```html
<div is="overview-packages" :package-category-id="[1,2]"></div>
```
**or**
```html
<div is="overview-packages" :package-category-id="1"></div>
```

#### accommodation-id

Load the packages for provided accommodation.

number | default value: `null`

```html
<div is="overview-packages" :accommodation-id="1"></div>
```

#### default-people

This parameter is used to set the default values for person types if the value is not set for each person type.

object | default value: `null`

```html
<div is="overview-packages" :default-people="{1:3}"></div>
```

#### override-people

This parameter is used to override the person type value whenever. It will ignore any remembered person type value and set the ones provided through this parameter.

object | default value: `null`

```html
<div is="overview-packages" :override-people="{1:3}"></div>
```

#### is-carousel

Show packages as carousel.

boolean | default value: `false`

```html
<div is="overview-packages" :is-carousel="true"></div>
```
