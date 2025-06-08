# Quete_log_windows_server22

ligne 14 : <Channel>DNS Server,Microsoft-Windows-DNS-Client/Operational,System</Channel>  
Filtre cible trois journaux d'événements :
- DNS Server
- Microsoft-Windows-DNS-Client/Operational
- System

Ligne 18 : <Source>Microsoft-Windows-DNS-Client,Microsoft-Windows-DNS-Client-DiagTrack,Microsoft-Windows-DNS-Server-Service,dns</Source>
Filtre sources d’événements :
- Microsoft-Windows-DNS-Client : Événements générés par le client DNS.
- Microsoft-Windows-DNS-Client-DiagTrack : Événements de télémétrie DNS (DiagTrack).
- Microsoft-Windows-DNS-Server-Service : Événements générés par le service DNS serveur.
- dns : Une source générique DNS, souvent utilisée par certains outils.

Ligne 22 : <EventId>2,4,409,501,502,6001,6002</EventId>
Filtre les ID : 
- 2 : Résolution DNS réussie.
- 4 : Échec de résolution DNS.
- 409 : Notification de modification de cache DNS.
- 501, 502 : Erreurs serveur DNS.
- 6001, 6002 : Problèmes avec la zone ou le service DNS.

Ligne 24 : <Level>1,2,3,4,0</Level>
Filtre les niveaux de gravité :
- 0 : Log Always
- 1 : Critical
- 2 : Error
- 3 : Warning
- 4 : Information
