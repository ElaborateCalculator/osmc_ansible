osmc
=========

Deploys local cfg to OSMC Raspberry Pi devices

Requirements
------------

OSMC installed, network configured, ssh key shared to `osmc` user

Role Variables
--------------

* vars/main.yml
  * `osmc_default_user`: Default OSMC user (not currently used)
  * `osmc_default_pass`: Default OSMC password (not currently used)
  * `mysql_host`: Host for Kodi MySQL db backend
  * `mysql_port`: Port for Kodi MySQL db backend
  * `mysql_user`: User for Kodi MySQL db backend
  * `nagios_host`: Host for Nagios service
  * `nas_host`: Host for Kodi sources
  * `ldap_uri`: LDAP URI for name services
  * `ldap_basedn`: LDAP base DN
  * `ldap_sudoers_ou`: LDAP sudoers OU
  * `ldap_ssl_cert`: SSL cert for secure LDAP
  * `krb_server`: Kerberos controller
  * `krb_realm`: Kerberos realm
  * `krb_domain`: Kerberos domain
* vars/secrets.yml
  * `osmc_pass`: New password for OSMC default user
  * `root_pass`: New password for root
  * `mysql_pass`: Password for Kodi MySQL db backend
  * `krb_prin`: Kerberos administration principal
  * `krb_pass`: Kerberos administration principal password
  * `mpg_codec`: Comma separated list of MPG2 codec keys (max 8)
  * `wvc_codec`: Comma separated list of WVC1 codec keys (max 8)


Dependencies
------------

None

Example Playbook
----------------

See `osmc.yml` in root directory

License
-------

GPL v3


