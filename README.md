nmap -A 192.168.50.0/24 (This is aggressive scan mode, telling the nmap to discover alive port, scan open ports, detect services, run scripts, detect OS, and perform traceroute)


![nmap-A](https://github.com/user-attachments/assets/2f794c70-c602-4788-b89c-6e7c76deaa4b)




nmap --script "vuln,brute" 192.168.50.11/24
“Scan the entire 192.168.50.0/24 network for vulnerabilities and weak passwords using all vuln and brute-force Nmap scripts.”


![nmap --script vul,brute](https://github.com/user-attachments/assets/285a084b-f767-49d6-87ac-81921b7149a6)




nmap --script smb-enum-shares.nse -p445 192.168.50.11/24 (shows all the shared folders on this windows device and tell you which one you can access, eg: 
ADMIN$: Remote Admin share
C$: Default drive share
Public: Read/Write
SharedDocs: Read-Only).
.nse is an nmap script file system


![smb-enum-shares nse](https://github.com/user-attachments/assets/0a491865-972f-4d09-9bc9-ebe1a118975d)





nmap -sn 192.168.50.13/24 (This sends ping to check which hosts are up)


![nmap -sn ](https://github.com/user-attachments/assets/7a4beeec-50d0-4622-8826-72449116d353)





nmap -sV 192.168.50.0/24 (identify running software service)


![nmap -sV](https://github.com/user-attachments/assets/ef3542c1-e1c9-4189-a746-494cf5b3e6a6)






