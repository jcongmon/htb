# Meow

## Enumeration
I began by verifying connectivity using the ping command. 

<img src="https://i.imgur.com/UnZzrqL.png" width=50% height=50%>

Next, I performed network enumeration with nmap, identifying an open Telnet service on TCP port 23.

<img src="https://i.imgur.com/nCTeUt5.png" width=50% height=50%>

## Foothold
Using Telnet, I attempted various login methods, including an empty username/password, anonymous access, and ultimately succeeded by logging in as the root user with a blank password.

<img src="https://i.imgur.com/lzgdQTE.png" width=50% height=50%>

## Flag
Once logged in, I located the flag in the current directory.

<img src="https://i.imgur.com/xGhyOap.png" width=50% height=50%>
