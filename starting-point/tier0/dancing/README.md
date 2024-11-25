# Dancing

## Enumeration
Starting with network enumeration with nmap, we find an open SMB service on TCP port 445:

<img src="https://i.imgur.com/hBUaAit.png" width=50% height=50%>

## Foothold
Misconfiguration with no password allows us to see the existing shares on the server:

<img src="https://i.imgur.com/dffikDG.png" width=50% height=50%>

## Flag
The only acessible share is "WorkShares" containing two directories.

<img src="https://i.imgur.com/u5ZZOvQ.png" width=50% height=50%>

The "James.P" directory contains the flag:

<img src="https://i.imgur.com/peN5FIi.png" width=50% height=50%>
<img src="https://i.imgur.com/2eAC410.png" width=50% height=50%>


