# Booking widget

Example:
```html
<div is="booking"></div>
```

Parameters:
#### terms

This parameter is used to specify the title and urls for the terms page of pdf.

The array accepts the objects with title and link parameters as shown in the example below.

array | default value: []
```html
<div is="booking" :terms="[{ title: 'Term Title', link: 'https://url-to-term-link' }]"></div>
```

#### confirm-location

This parameter is used to specify the url where the page should be redirected after successful booking.

string | default value: null
```html
<div is="booking" confirm-location="/booking/complete"></div>
```

#### analytics

This parameter is used to either enable or disable the analytics on the widget.

boolean | default value: true
```html
<div is="booking" :analytics="true"></div>
```

#### sales-channel

This parameter is used to set the sales channel to be used to post the booking to tommy. There is no sales channels in harbor. The parameter must be provided the id from the tommy sales channels.

number | default value: null
```html
<div is="booking" :sales-channel="12883"></div>
```

#### scrolling

This parameter is used to set the widget to scroll mode. The default mode for the widget is steps. If this value is set to true the widget will load in scrolling mode.

boolean | default value: false
```html
<div is="booking" :scrolling="true"></div>
```

#### short-personal-data

This parameter is used to enable or disable short personal data form. When enabled these fields will be disabled from personal data form.

country, postcode, houseNumber, street, city, telephone, licenceNumber

To enable any or some of these field use parameter short-data-fields.

boolean | default value: false
```html
<div is="booking" :short-personal-data="true"></div>
```

#### short-data-fields

This parameter is used to enable any or some of the fields which are disabled by short personal data flag. These fields are available to enable.

country, postcode, houseNumber, street, city, telephone

To enable any or some of these field use parameter short-data-fields.

array | default value: null
```html
<div is="booking" :short-personal-data="true" :short-data-fields="['postcode','houseNumber']"></div>
```

#### a-b-test

This parameter is used to make the widget auto load from any of the two available modes on random basis. The widget will either load in steps mode or scrolling mode on random basis.

boolean | default value: false
```html
<div is="booking" :a-b-test="true"></div>
```

#### lang

This parameter is used to explicitely set the language for the widget. If not set the default language from harbor-lang header meta will be used.

string | default value: null | possible values: 'nl', 'de', 'en', 'fr'
```html
<div is="booking" lang="de"></div>
```

#### scroll-offset

This parameter is used to set extra offset for autoscroll when navigated between steps in steps mode.

number | default value: 0
```html
<div is="booking" :scroll-offset="150"></div>
```

#### additional-fields

This parameter is used to enable any or some of the fields which are custom added to tommy. New fields may need to be added on the code. Below is the currently available additional field.

licenceNumber

To enable any or some of these field use parameter additional-fields.

array | default value: null
```html
<div is="book-on-touch" :additional-fields="['licenceNumber']"></div>
```
