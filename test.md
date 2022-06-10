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
ping 192.168.162.3

# PING AVEC RESEAU C
ping 192.168.163.1 OK

# PING INTERNE DE SERV WEB 
ping 192.168.164.42 OK

# Connection SERV WEB A ET B
lynx 192.168.161.2
lynx 192.168.164.42

# Connextion SSH 
ssh 192.168.161.1

#                                 /!\ TEST RESEAU C

# PING INTERNE  
ping 192.168.163.121

# PING AVEC A
ping 192.168.161.1 ok

# PING AVEC D
ping 192.168.162.3

# PING AVEC B
ping 192.168.164.1

# Connection SERV WEB A ET B
lynx 192.168.161.2
lynx 192.168.164.42

# Connextion SSH 
ssh 192.168.161.1

#                               /!\ TEST RESEAU D

# PING INTERNE  
ping 192.168.162.18

# PING AVEC A
ping 192.168.161.1

# PING AVEC C
ping 192.168.163.1

# PING AVEC B
ping 192.168.164.1

# Connection SERV WEB A ET B
lynx 192.168.161.2
lynx 192.168.164.42


# Connextion SSH 
ssh 192.168.161.1

#                               EXT

# PING SERV WEB AVEC AUTRE IP TCPDUMP sur SERV WEB pour l'écoute et verifier le nat
ping 192.168.161.1
tcpdump 