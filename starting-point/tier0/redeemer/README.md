# Redeemer

## Enumeration
Initial network enumeration in the usual fashion leads to no open ports. In addition, scanning on all ports (-p-) is time-consuming (53 min elapsed, only 62% done).

<img src="https://i.imgur.com/OCpIRUn.png" width=50% height=50%>

Scanning with more aggressive flags (-sS, stealth scan; -Pn, don't ping; -T5, insane timing template (does not avoid IDS detection)) identifies an open Redis service on TCP port 6379 in 30 sec:

<img src="https://i.imgur.com/RoNSgnQ.png" width=50% height=50%>

## Foothold
We connect to the insecure Redis service:

<img src="https://i.imgur.com/3zy6JR1.png" width=50% height=50%>

## Flag
Accessing all the keys in the database allows us to find and retrieve the flag:

<img src="https://i.imgur.com/XEkh7eD.png" width=50% height=50%>



