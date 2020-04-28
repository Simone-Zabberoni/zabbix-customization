# Simple SSL Check template

### General informations

Relies on `zext_ssl_cert` - https://zabbix.org/wiki/Docs/howto/ssl_certificate_check

Made my own template because of import errors on the existing one, it was faster :-)

### Usage

Import the [XML file](https://github.com/Simone-Zabberoni/zabbix-customization/blob/master/SSL_Check/zbx_exportt_template_ssl_check.xml) in the template configuration page.

Each host must have a `{$SNI}` macro pointing to the the Server Name (ie: www.yoursite.tld)
