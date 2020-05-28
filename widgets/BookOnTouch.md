# Book on touch

Example:
```html
<div is="book-on-touch"></div>
```

Parameters:
#### greeter-name

This parameter is used to show the name on the welcome screen.

string | default value: null
```html
<div is="book-on-touch" greeter-name="Tenzer"></div>
```

#### logo

This parameter is used to add the url for the logo to be used on welcome screen.

string | default value: null
```html
<div is="book-on-touch" logo="http://url-to-logo"></div>
```

#### default-people

This parameter is used to set the value for default people for the widget. The values represent the id of the people from harbor and the value to be used.

object | default value: null
```html
<div is="book-on-touch" :default-people="{1:2,2:1}"></div>
```
