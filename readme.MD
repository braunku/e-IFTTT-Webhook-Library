# e-IFTTT-Webhook-Library

## This is a library for e!COCKPIT to send webhook events to IFTTT

This compiled library once installed into e!COCKPIT using the library manager, will allow simple function block to send events to IFTTT cloud service.  This library relies on cURL, there for you will need to install the cURL ipk using the PFC100/200 web based management (WBM).

## Install

Use the PFC web based management to install the cURL ipk.
![IPK Installation](http://i66.tinypic.com/wuqcms.jpg)

Use the e!COCKPIT Library Manager to install the compiled IFTTT library.
![IFTTT Library Installation](http://i66.tinypic.com/wuqcms.jpg)


## How to use

1. Create an instance of the function block called IFTTT_Send

2. Pass the string variables for the three optional values.

3. Copy your IFTTT Webhook key.  This can be found by logging into your IFTTT acount, then look in IFTTT>Services>Webhooks>Documentation. 

See the example flow:

![Flow Example](http://i66.tinypic.com/wuqcms.jpg)

## Authors

[Kurt Braun][3]

[1]:https://www.youtube.com/user/WagoKurt