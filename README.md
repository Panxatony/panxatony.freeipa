panxatony.freeipa
=========

Installation of FreeIPA server 

Requirements
------------

    none

Role Variables
--------------

    freeipa_server_ip: 192.168.237.11
    freeipa_hostname: ipasrv.cs9demo.lab
    freeipa_alias: ipasrv
    freeipa_domain_search: cs9demo.lab
    freeipa_kerberos_realm_name: CS9DEMO.LAB
    freeipa_directory_manager_password: topSecret
    freeipa_dns_forwarder_ip: 8.8.8.8
    freeipa_ldap_search_base: "dc=cs9demo,dc=lab"
    freeipa_ldap_user_search_base: "cn=users,dc=cs9demo,dc=lab"
    freeipa_ldap_group_search_base: "cn=groups,dc=cs9demo,dc=lab"
    freeipa_ldap_default_bind_dn: "uid=admin,cn=users,dc=cs9demo,dc=lab"
    freeipa_ldap_uri: "ldaps://ipasrv.cloud-cell02.audi.vwg/"
    freeipa_ldap_sudo_search_base: "ou=SUDOers,dc=cs9demo,dc=lab"
    freeipa_user_homedir: "/home"

Dependencies
------------

    none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: panxatony.freeipa, freeipa_alias: cs9lab }

License
-------

BSD

Author Information
------------------

Lars Hunold
http://macnemo.tv
