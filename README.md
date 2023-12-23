# Securing-Enterprise-Access
## Elevating Security: The Power of 802.1X, EAP, and RADIUS in the Enterprise
Enterprise security mode, requires a __RADIUS__ server for __Authentication__, __Authorization__, and __Accounting__ __(AAA)__: 
### FreeRADIUS is the underlying AAA server that handles authentication and authorization, while DaloRADIUS is a web interface that simplifies the management and configuration of a FreeRADIUS server through a graphical user interface.
<a href="https://github.com/lirantal/daloradius/releases/tag/1.2">Install Daloradius </a>
### Install FreeRADIUS Server in ubunto system: 
sudo apt -y install freeradius freeradius-mysql freeradius-utils
### The combination of 802.1X, EAP, and RADIUS is employed to establish robust and secure network access control:
__802.1X__ is a network access control standard that requires user or device authentication before granting access to the network. It establishes the framework for authentication at the data link layer.
__EAP__ is used to encapsulate authentication messages between the client and the authentication server.
__RADIUS__ is commonly employed for communication between the authenticator (e.g., a switch) and the authentication server."

## The authentication process typically involves the following steps:
__Initialization__: The supplicant initiates the connection to the network, and the authenticator places the port in a "closed" or unauthorized state.

__EAPOL__: (Extensible Authentication Protocol over LAN): The supplicant and authenticator exchange EAPOL messages to initiate the authentication process.

__Identity Request__: The authenticator requests the identity of the supplicant.

__Identity Response__: The supplicant provides its identity (such as a username).

__Authentication__: The authentication server validates the supplicant's credentials (for example: username and password).

__Access Granted/Denied__: If the credentials are valid, the authenticator opens the port, allowing the supplicant access to the network. If the credentials are not valid, access is denied.
