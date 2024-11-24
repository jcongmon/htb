# Fawn

## Enumeration
Starting with network enumeration with nmap, we find an open FTP service on TCP port 21:

<img src="https://i.imgur.com/0eKwnpc.png" width=50% height=50%>

## Foothold
Initial anonymous login with no password allows access to the FTP server:

<img src="https://i.imgur.com/cJROhg0.png" width=50% height=50%>

## Flag
Once logged in, the flag is located in the current directory. Transferring the file to the local computer allows access to the flag.

<img src="https://i.imgur.com/edyJ72q.png" width=50% height=50%>

<img src="https://i.imgur.com/Tj57v1n.png" width=50% height=50%>

