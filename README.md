# Zabbix Custom Templates, Webhook, Scripts and so on

## Disclaimer

Everything works, but use at your own risk ;-)

### Contents

- [Twilio Integration via webhook](https://github.com/Simone-Zabberoni/zabbix-customization/blob/master/Twilio/README.md)
- [SSL Checking](https://github.com/Simone-Zabberoni/zabbix-customization/blob/master/SSL_Check/README.md)
- [Preprocessing stuff](https://github.com/Simone-Zabberoni/zabbix-customization/blob/master/Preprocessing/README.md)

- More to come

## Useful scripts and oneliners

Windows Agent setup via msi:

```
msiexec /l*v log.txt  /i zabbix_agent-5.0.3-windows-amd64-openssl.msi /qn SERVER=yourZabbix SERVERACTIVE=yourZabbixs
```
