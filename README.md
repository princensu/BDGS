BDGS COD 4 Server


Prerequisites

* Ensure Static IP address is configured on the Server laptop/machine
  * https://nordvpn.com/blog/how-to-set-up-static-ip-address/ 
* Connect using Remote Desktop app for lagfree experience, vnc is considerably slower and do not have copy paste file functionality
* On the router DMZ should be set to the static IP address of server machine
* Make sure the following ports are forwarded
  * TCP - 3074,27014-27050
  * UDP - 3074,3478,4379-4380,27000-27031,27036
  * Source - https://openmyip.com/-call-of-duty-modern-warfare


Server Setup :

* Install COD 4
* Install patch 1.6
* Install patch 1.6-1.7
* Create shortcut of cod4 mw file in desktop
* Add parameter +exec server.cfg
* Add parameter of COD4x server Auth ID in the server.cfg to ensure server appears in server.cfg file
  * Source - http://cod4master.cod4x.ovh/

Rcon Tool
* https://fearless-assassins.com/files/file/685-rconmaxmw/


Useful rcon commands :
* set g_gametype ""
* set sv_punkbuster 0
* set rcon_password bdgs1234
* set g_password ""

COD 4x master server authentication command, should be included in server.cfg file :
* set sv_authtoken "180EC87EFB4FAFEEB8960EF3A56DC2982733E13F"

General shortcut :
 * +set dedicated 2 +set rcon_password "bdgs1234 +set g_password "" +set sv_punkbuster 0  +exec server.cfg

Shortcut for running server with ModWarfare - must be run for user maps :
* +exec server.cfg +"Mods\ModWarfare"+set sv_token 180EC87EFB4FAFEEB8960EF3A56DC2982733E13F 


Webserver should be installed in d: where cod4 folder will reside :
* python -m http.server 8181

Map autodownload links :
* http://92.220.11.60:8181/cod4/usermaps/
* https://dl.fsho.st/cod4/usermaps/
* http://dl.fsho.st/cod4/usermaps/
* http://92.220.11.60:8181/cod4/
  
