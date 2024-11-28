# Crocodile

## Enumeration
Starting with a network enumeration with nmap (-sC: standard scripts, -sV: service version), we find one open FTP service on TCP port 21 and one open HTTP service running Apache 2.4.41:

<img src="https://i.imgur.com/5fcgt9H.png" width=50% height=50%>

## Foothold
Anonymous access to the FTP server:

<img src="https://i.imgur.com/wwjOz28.png" width=50% height=50%>

A username file and corresponding password file are found containing admin credentials:

<img src="https://i.imgur.com/U8lq1Y3.png" width=50% height=50%>

Going to the webpage:

<img src="https://i.imgur.com/u7K036y.png" width=50% height=50%>

Subsequent analysis with Wappalyzer shows the site is running with PHP.

Directory enumeration with GoBuster shows an accessible /login.php page:

<img src="https://i.imgur.com/uPqbfAf.png" width=50% height=50%>

## Flag
Logging into the /login.php page with admin credentials yields the flag:

<img src="https://i.imgur.com/bGFtupu.png" width=50% height=50%>

