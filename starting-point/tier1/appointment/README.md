# Appointment

## Enumeration
Starting with network enumeration with nmap, we find an open HTTP service on TCP port 80:

<img src="https://i.imgur.com/61Yv1rP.png" width=50% height=50%>

The Apache/2.4.38 (Debian) currently has 4 CVEs: https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=Apache/2.4.38%20(Debian)

## Foothold
Accessing the webpage leads to a login form:

<img src="https://i.imgur.com/al5t2hN.png" width=25% height=25%>

Trying the following combinations to brute-force access did not work:
- admin/[blank]
- admin/admin
- root/root
- test/test
- user/password

## Flag
Attempting SQL injection using (<b>admin' --</b>) did not work. Other combinations using the (--) SQL comment in the user and password field did not work.

Using (<b>admin' #</b>) assuming PHP service with any password allowed access to the flag:

<img src="https://i.imgur.com/CT6zfik.png" width=50% height=50%>

## Afterwards

Something that should have been done previous to SQL injection was directory enumeration with GoBuster, dirbuster, or dirb. Going back to do quickly do this with a simple word list came up negative:

<img src="https://i.imgur.com/Sw9anr1.png" width=50% height=50%>


