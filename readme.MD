# e!COCKPIT IFTTT Webhook Library

## This is a library for e!COCKPIT to send webhook events to IFTTT

This compiled library once installed into e!COCKPIT using the library manager, will allow simple function block to send events to IFTTT cloud service.  This library relies on cURL, there for you will need to install the cURL ipk using the PFC100/200 web based management (WBM).

## Install

Use the an scp client to copy the cURL ipk file to the root folder of the PFC, then use an ssh client to install the file as shown below.  

You can test this by cut/pasting your IFTTT example cURL command, with a -k added at the end to disable SSL.  If you want to pass the three values, then modify the command this way.

	curl -X POST -H "Content-Type: application/json" -d "{\"value1\":\"Hello \",\"value2\":\"World \",\"value3\":\"!\"}" https://maker.ifttt.com/trigger/{event}/with/key/{your key here} -k

![IPK Installation](http://i68.tinypic.com/2dabzue.jpg)
![IFTTT Key](http://i68.tinypic.com/vxedh.jpg)

Use the e!COCKPIT Library Manager to install the compiled IFTTT library.
![IFTTT Library Installation](http://i65.tinypic.com/2cq02vl.png)


## How to use

1. Create an instance of the function block called IFTTT_Send

2. Pass the string variables for the three optional values.

3. Copy your IFTTT Webhook key.  This can be found by logging into your IFTTT acount, then look in IFTTT>Services>Webhooks>Documentation. 

4. Create a recipe in your IFTTT account using the event name you create to trigger the "then" action you desire.

example usage:
![Flow Example](http://i64.tinypic.com/2lwlmhx.png)

## Authors

[Kurt Braun][3]

[1]:https://www.youtube.com/user/WagoKurt