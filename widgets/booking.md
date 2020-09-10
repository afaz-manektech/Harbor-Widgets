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
<div is="booking" :additional-fields="['licenceNumber']"></div>
```

#### scroll-offset

This parameter is used to set the offset for autoscroll when step is navigated forward or backward.

number | default value: 0
```html
<div is="booking" :scroll-offset="100"></div>
```

#### languages

The parameter is used to set the switchable languages on the booking widget.

object | default value: `{nl:''Nederlands'}` | possible value: `{nl:'Nederlands',de:'Duits',en:'Engels',fr:'Frans'}`
```html
<div is="booking" :languages="{nl:'Nederlands',de:'Duits',en:'Engels',fr:'Frans'}"></div>
```

#### help-phone

Specify the contact number to be shown on need help section. If value for this parameter is present then the phone link will be shown in the need help section otherwise only the email button will be shown.

string | default value: null
```html
<div is="booking" help-phone="0341 –751 752"></div>
```

#### logo

Specify the url of logo to be shown on the overlay loading message. If the logo is not present it will not be shown on the widget, only the loading message will be shown.

string | default value: null
```html
<div is="booking" logo="https://demo.tenzer.nl/images/logo.png"></div>
```

#### max-articles

Specify the threshold to show the maximum number of articles initially. If more than specified articles are present then the expand button will be shown.

number | default value: 5
```html
<div is="booking" :max-articles="3"></div>
```

#### location-icon-size

Specify the size of the location icon div so that the map library shows the icon on correct place.

array, number | default value: null
```html
<div is="booking" :location-icon-size="20"></div>
```

#### auto-scroll

Enable autoscroll widget into view when loaded.

boolean | default value: false
```html
<div is="booking" :auto-scroll="true"></div>
```

#### scroll-variation

If not satisfied with the autocalculated scroll position, the variation can be added to autodetected position using this parameter.

number | default value: 0
```html
<div is="booking" :scroll-variation="10"></div>
```
