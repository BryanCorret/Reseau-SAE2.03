# ATTENTION IL SE PEUT QUE DHCP NE SE LANCE PAS AUTOMATIQUEMENT SI C'EST LE CAS VEUILLEZ LE DEMARER A LA MAIN


#                               /!\ TEST RESEAU A

# PING INTERNE DE SERV SSH DEPUIS SERV WEB 
ping 192.168.161.1 OK


# PING AVEC C 
ping 192.168.164.1 OK

# PING AVEC D
ping 192.168.162.3 OK

# PING AVEC B
ping 192.168.164.1 ok

# LYNX WEB
lynx 192.168.161.2 ok

#                               /!\ TEST RESEAU B

# PING AVEC RESEAU A
ping 192.168.161.1 ok

# PING AVEC RESEAU D
ping 192.168.162.3 OK

# PING AVEC RESEAU C
ping 192.168.163.1 OK

# PING INTERNE DE SERV WEB 
ping 192.168.164.42 OK

# Connection SERV WEB A ET B
lynx 192.168.161.2 oK
lynx 192.168.164.42

# Connextion SSH 
ssh 192.168.161.1

#                                 /!\ TEST RESEAU C

# PING INTERNE  
ping 192.168.163.121

# PING AVEC A
ping 192.168.161.1 ok

# PING AVEC D
ping 192.168.162.3 ok

# PING AVEC B
ping 192.168.164.1 ok

# Connection SERV WEB A ET B
lynx 192.168.161.2 OK
lynx 192.168.164.42

# Connextion SSH 
ssh 192.168.161.1 ok

#                               /!\ TEST RESEAU D

# PING INTERNE  
ping 192.168.162.18 ok

# PING AVEC A
ping 192.168.161.1 ok

# PING AVEC C
ping 192.168.163.1 ok

# PING AVEC B
ping 192.168.164.1

# Connection SERV WEB A ET B
lynx 192.168.161.2 ok
lynx 192.168.164.42

# Connextion SSH 
ssh 192.168.161.1 ok


#                               EXT

# PING SERV WEB AVEC AUTRE IP TCPDUMP sur SERV WEB pour l'écoute et verifier le nat
ping 192.168.161.1 ok
tcpdump ok