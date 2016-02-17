Tomcat v7.0.56
==============

Installation d'un serveur tomcat 7.0.56

A la fin de l'installation, s'il est spécifié

Requirements
------------

Nécessite un JAVA 6 minimum

Role Variables
--------------

Voici les variables disponibles avec leurs valeurs par défaut :

    # installation tomcat
    tomcatAdminUsername: tomcat
    tomcatAdminPassword: ""
    tomcatCatalinaBase: /usr/share/tomcat
    tomcatCatalinaHome: /usr/share/tomcat
    tomcatUser: tomcat
    tomcatAjpPort: 8009
    tomcatHttpPort: 8080
    tomcatHttpsPort: 8443
    
    # liaison de l'application steamengine avec le ROOT Tomcat si souhaité
    homeDir: null
    skipApplicationLink: false

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
        - homeDir: "/projet"
      roles:
         - { role: steamroles/tomcat }

License
-------


Author Information
------------------

STEAMULO - http://www.steamulo.com