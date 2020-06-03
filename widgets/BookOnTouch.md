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

#### override-people

This parameter is used to set the value for people and override the values which is set by the backend. The values represent the id of the people from harbor and the value to be used.

object | default value: null
```html
<div is="book-on-touch" :override-people="{1:2,2:1}"></div>
```

#### analytics

This parameter is used to either enable or disable the analytics on the widget.

boolean | default value: true
```html
<div is="book-on-touch" :analytics="true"></div>
```

#### show-features

This parameter is used to either enable or disable the features on the accommodation.

boolean | default value: true
```html
<div is="book-on-touch" :show-features="true"></div>
```

#### show-information

This parameter is used to either enable or disable the information on the accommodation.

boolean | default value: true
```html
<div is="book-on-touch" :show-information="true"></div>
```

#### theme

This parameter is used to set the theme for the accommodation.

string | default value: normal | possible values: normal, alternative
```html
<div is="book-on-touch" theme="alternative"></div>
```

#### should-reset-when-idle

This parameter is used to determine if the widget should reset when there is no activity for certain time (another parameter: idle-reset-time). The widget will refresh the page when there is no activity for the set time if this parameter is set to true. If the parameter is set to false, the widget will stay wherever it is for as long until the page is manually refreshed.

boolean | default value: true
```html
<div is="book-on-touch" :should-reset-when-idle="true"></div>
```

#### idle-reset-time

This parameter is used to set the reset time for the widget. If for the set time there is no activity the widget will refresh the page if should-reset-when-idle is set to true in the widget code or should-reset-when-idle parameter is not used in the widget code at all.

The value represent seconds.

number | default value: 300
```html
<div is="book-on-touch" :idle-reset-time="180"></div>
```

#### sales-channel

This parameter is used to set the sales channel to be used to post the booking to tommy. There is no sales channels in harbor. The parameter must be provided the id from the tommy sales channels.

number | default value: null
```html
<div is="book-on-touch" :sales-channel="12883"></div>
```

#### languages

This parameter is used to set the available language for the widget.

object | default value: {nl:'Nederlands'} | possible values: {nl:'Nederlands',de:'Duits',en:'Engels',fr:'Frans'}
```html
<div is="book-on-touch" :languages="{nl:'Nederlands',de:'Duits',en:'Engels'}"></div>
```

#### category-id

This parameter is used to limit the widget to the provided category. The accommodation from only the provided category will be allowed to book.

number | default value: null
```html
<div is="book-on-touch" :category-id="2"></div>
```

#### filtered-categories

This parameter is used to limit the widget to the provided categories. The accommodation from only the provided categoies will be allowed to book. There will be filters on the accommodations selection screen to filter the list of accommodation per category.

array | default value: null
```html
<div is="book-on-touch" :filtered-categories="[1,2]"></div>
```

#### remarks-field

This parameter is used to enable or disable the remarks field on personal data form.

boolean | default value: false
```html
<div is="book-on-touch" :remarks-field="true"></div>
```

#### short-personal-data

This parameter is used to enable or disable short personal data form. When enabled these fields will be disabled from personal data form.

country, postcode, houseNumber, street, city, telephone, licenceNumber

To enable any or some of these field use parameter short-data-fields.

boolean | default value: false
```html
<div is="book-on-touch" :short-personal-data="true"></div>
```

#### short-data-fields

This parameter is used to enable any or some of the fields which are disabled by short personal data flag. These fields are available to enable.

country, postcode, houseNumber, street, city, telephone, licenceNumber

To enable any or some of these field use parameter short-data-fields.

array | default value: null
```html
<div is="book-on-touch" :short-personal-data="true" :short-data-fields="['postcode','houseNumber','licenceNumber']"></div>
```

#### thanks-page-timeout

This parameter is used to set the value for timeout after the booking is successful. The page will be refreshed the the widget will reset once the timeout is over.

The value represent seconds.

number | default value: 120
```html
<div is="book-on-touch" :thanks-page-timeout="25"></div>
```
