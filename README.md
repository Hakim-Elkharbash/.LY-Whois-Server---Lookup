# .ly-whois-server
This project explains how to check .ly domain availability through ccTLD of Libya (.ly whois server).
------------------
1. Open Socket connection to WhoIs server of Libya (whois.nic.ly) using port (43)
2. Add "\r\n" to your domain to signifying the end of a line of text and the start of a new line.
3. Send the data to whois server.
4. Listen for incoming data, and save it in string variable, in our case is ($whois_info).
5. Print ($whois_info) variable, OR check it to specify whether the domain registered or not.

NOTE: This example could work with other whois servers, you just need to specify the link of your whois server.
