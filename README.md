# Web-Application-Network-Design

For an Ecommerce network, I designed the network security zones, including firewall pseudo code rules and IDS placement.

The following items have been identified as network components or requirements:


• Three Apache web servers, four database servers, and three application and financial processing servers are on the network.

• Web servers can be accessed via the internet.

• There is a protected internal network.

• Internal users have unrestricted access to internet resources.

• Internal users are able to access both the web servers and application servers using SSH (port 22).

• From the protected network, the Database Administrator will be able the database servers on port 3306.

• On a custom port 4400, the web servers can connect with the database servers.

• On a custom port 4420, the web servers can connect with the financial processing servers.

• There is an administration web site on one of the web servers that allows remote administration for a single Apache user ('manager') via a web interface.

      o The URL for the administration site is "/var/www/manager/webadmin.htm"

      o Remote access to the site is only available to hosts on the protected network subnet.
      
      o The administrator user must use an encrypted https connection to access the administration site.
      
      
The design documentation consists of the following sections:

    • A network layout diagram that shows the security zones, their network IP addresses, and any firewall and IDS sensor locations.

    • A document describing the firewall pseudo-code rules that must be followed in order to enforce the design

    • All documents containing any Apache directives required for the administrative website's implementation

      
