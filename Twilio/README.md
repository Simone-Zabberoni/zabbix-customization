# Twilio Zabbix Integration via webhook

### Disclaimer

Twilio uses http basic authentication, which is currently unsupported in Zabbix webhooks, so the script implements it via:

```
 req.AddHeader('Authorization: Basic ' + btoa(params.accountsid + ":" + params.accounttoken));
```

The `btoa` call is supported only from Zabbix 4.4.8rc1 and later versions.

### Usage

Import the [XML file](https://github.com/Simone-Zabberoni/zabbix-customization/blob/master/Twilio/zbx_export_mediatypes-twilio.xml) in the media type configuration page and configure it with your `SID`, `token` and `caller id` (See https://www.twilio.com/console )

Then add a media for your users and specify the phone number to contact, including the prefix (i.e. for Italy: 39335123456).

### Details on message body

The message contains only the subject of the alert, expanded from `{ALERT.SUBJECT}`. Modify if needed, but always consider the SMS message lenght!
