# Network-Scanning-and-Enumeration, Network traffic analysis
- <b>[Network Enumeration.](https://imgur.com/a/iPRyIJ8)</b>
    - Description: This lab allowed me to gain hands-on experience in network scanning and enumeration. I learned how to use the nmap tool for network discovery and explored different scanning techniques. Additionally, i understood the significance of enumeration and how to utilize enumeration techniques and tools for information gathering.
1. nmap -p 80 --script=http-enum.nse birchwood.org
Nmap is used to enumerate HTTP information on port 80 of the target host using the http-enum.nse script.
2. SNMP (Simple Network Management Protocol) can be used to query information from network devices. The snmpwalk command can be used to retrieve SNMP information.
snmpwalk -c public -v2c birchwood.org
This command queries the birchwood.org (137.114.14.145) address using the SNMP community string "public" and version 2c.
3. DNS Enumeration Tools (e.g dnsenum):
DNS enumeration tools like dnsenum can be used to gather information about DNS records, subdomains, and zone transfers.
rust
dnsenum birchwood.org
This command performs DNS enumeration on the " birchwood.org " domain to identify subdomains and DNS-related information.
4. Automated Enumeration Scripts:
"enum4linux" are designed to extract information from Windows systems.
enum4linux -a birchwood.org
This command runs enum4linux on the birchwood.org to gather information about Windows systems, including users, shares, and more.
SMTP Enumeration Tools (e.g., smtp-user-enum):
5. SMTP enumeration tools are used to identify valid email addresses on a mail server. One such tool is smtp-user-enum.
smtp-user-enum -M VRFY -U /usr/share/wordlists/metasploit/unix_users.txt -t birchwood.com -o output.txt
This command performs SMTP user enumeration using the VRFY method and a wordlist of potential usernames.
- <b>[WireShark and tcpdump](https://imgur.com/a/FIQPPDO)</b>
    - Description: This lab allowed me to gain practical experience in network traffic analysis using Wireshark and tcpdump. I learned how to capture network traffic, apply filters, and analyze packet-level details. By comparing Wireshark and tcpdump, i understood the differences in their usage and capabilities for network traffic analysis.
