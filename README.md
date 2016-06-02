# Overview
This role installs the Darwin calendar and contacts server for the purposes of
providing synchronized contacts and calendars across multiple devices. The
standards-compliant server supports CardDAV and CalDAV formats, meaning that it
will work with the vast majority of contacts and calendar applications for desktop
and mobile.

More information about the project is available at http://calendarserver.org.
The license for the Calendar and Contacts server implementation is Apache v2.0.

# Dependencies
Common role
OpenLDAP role

# Variables
```yaml
- vars:
  domain: domain.com
  ldapadminpassword: change_the_password
  ldap_ip: 127.0.0.1
  ldap_user_searchbase: ou=people,dc=domain,dc=com
  caldavduserpassword: change_the_password
  tls_cert_file_location: /etc/letsencrypt/live/domain.com/fullchain.pem
  tls_key_file_location: /etc/letsencrypt/live/domain.com/privkey.pem
```
