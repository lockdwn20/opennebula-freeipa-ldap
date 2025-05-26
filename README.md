# opennebula-freeipa-ldap
Repository for configuration items for integrating FreeIPA LDAP services into OpenNebula

This configuration is based on the current OpenNebula Community Edition ver 6.10 which can be found at https://opennebula.io/use/#download_opennebula  
Note: I have used a similar configuration in previous versions  

The OpenNebula documentation can be found at https://docs.opennebula.io/6.10/installation_and_configuration/authentication/ldap.html, all information found in this repository should be used in conjunction with the official documentation 

**Note: This configuration assumes that you have disabled anonymous binds on your FreeIPA server and use StartTLS rather than LDAPS or SimpleTLS**  
**Note:  This configuration will auto-generate the server1.yaml assuming that you have built the groups inside OpenNebula and given them a GROUP_DN option with the full group DN (ex. cn=<group_name>,cn=groups,cn=accounts,dc=example,dc=com)**

![image](https://github.com/user-attachments/assets/2148b75c-b652-46b9-ad76-48e284aa832d)


The files are located on your Fireedge/Sunstone Server:  
The ldap_auth.conf is located in the /etc/one/auth folder  
The server1.yaml is located in the /var/lib/one directory  

