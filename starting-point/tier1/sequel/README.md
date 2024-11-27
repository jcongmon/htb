# Sequel

## Enumeration
Starting with an aggressive network enumeration with nmap, we find an open SQL service on TCP port 3306:

<img src="https://i.imgur.com/LkuexXI.png" width=50% height=50%>

Finding the service version and using a default script scan using nmap on port 3306 yields the following information:

<img src="https://i.imgur.com/0GradOu.png" width=50% height=50%>

Most important is its version MariaDB v5.5.5-10.3.27.

## Foothold
Connecting to the service with the username <b>root</b> with no password allows access to the database:

<img src="https://i.imgur.com/ZUuWC24.png" width=50% height=50%>

Below shows current databases:

<img src="https://i.imgur.com/TM0rQcA.png" width=50% height=50%>

## Flag
Accessing the <b>htb</b> database and using the config table gives the flag:

<img src="https://i.imgur.com/WvORoOk.png" width=50% height=50%>
