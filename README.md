# Ashalatha's Cybersecurity Portfolio

Welcome to my personal cybersecurity portfolio!  
This site showcases hands-on projects in *OSINT, **network scanning, **ethical hacking, and **Linux-based analysis*.

🔗 *Live Portfolio:* [https://ashalatha2003.github.io/asha.html](https://ashalatha2003.github.io/asha.html)

---

## 🛠 Tools & Technologies Used

1. OSINT Investigation — Sherlock

Goal: Map public footprint of a username
Comment: This project shows ability to gather online intelligence and profile users.
Tools: Sherlock, Python
Summary: Queried 30+ social media platforms, identified active accounts, and assessed exposure
Skills: OSINT, user profiling, exposure assessment
Key Command:

sherlock virat.kohli

2. IP Geolocation & Network Path Analysis

Goal: Analyze IP routing and international exposure
Comment: Useful for understanding traffic patterns and potential geo-risk.
Tools: Traceroute, mtr
Summary: Traced IP paths across 6+ countries, identified ISP transitions and latency patterns
Skills: Network reconnaissance, geo-risk assessment
Key Commands:

traceroute x.x.x.x
mtr -rw x.x.x.x

3. Domain Intelligence — Dmitry (WHOIS & Metadata)

Goal: Collect domain and hosting information
Comment: Highlights ability to perform passive reconnaissance and gather metadata.
Tools: Dmitry, Whois, dig
Summary: Collected domain metadata, emails, and hosting info for reconnaissance
Skills: Passive intelligence, domain profiling
Key Command:

dmitry -winse testfire.net

4. Scanning & Enumeration — Nmap, Hping3, Wireshark

Goal: Identify hosts, services, and capture traffic behavior
Comment: Shows practical scanning and packet analysis skills.
Tools: Nmap, Hping3, Wireshark
Summary: Performed service detection, packet-craft analysis, captured TCP/HTTP flows
Skills: Port scanning, protocol analysis, traffic interpretation
Key Commands:

nmap -T4 -A -v 192.x.x.x
hping3 -S 192.x.x.x -p 80
sudo tcpdump -i eth0 host 192.x.x.x -w capture.pcap

5. Scripted Service Detection — Nmap NSE

Goal: Detect unusual services and open ports
Comment: Demonstrates scripted scanning and identification of non-standard services.
Tools: Nmap NSE scripts
Summary: Found non-standard ports and AirTunes service
Skills: Automated service discovery, baseline deviation
Key Command:

nmap -sV -v --script=nbstat.nse 192.168.1.3

6. Password Security Audit — John, Hydra, Medusa

Goal: Evaluate password strength and detection patterns in lab
Comment: Controlled lab testing to analyze credential security and brute-force patterns.
Tools: John the Ripper, Hydra, Medusa, rockyou.txt
Summary: Cracked hashes, tested login resiliency, observed brute-force detection
Skills: Credential analysis, brute-force pattern recognition
Key Commands:

sudo unshadow /etc/passwd /etc/shadow > merged.txt
john --wordlist=/usr/share/wordlists/rockyou.txt merged.txt
john --show merged.txt
hydra -l admin -P rockyou.txt 192.168.x.x http-form-post "/login.php:username=^USER^&password=^PASS^:Invalid"
medusa -h 192.168.x.x -u admin -P rockyou.txt -M ftp
medusa -h 192.168.x.x -u testuser -P rockyou.txt -M ssh

7. Linux User Enumeration

Goal: Map system users and privilege hierarchy
Comment: Demonstrates Linux user and privilege auditing skills.
Tools: Linux commands
Summary: Reviewed /etc/passwd and /etc/shadow, examined logged-in users
Skills: Privilege analysis, system baseline validation
Key Commands:

cat /etc/passwd
cat /etc/shadow
pinky

8. Host Discovery — Subnet Sweep

Goal: Identify active devices in a network
Comment: Shows ability to perform asset discovery and network mapping.
Tools: Nmap
Summary: Conducted ping sweep across subnet, validated host inventory
Skills: Asset discovery, network reconnaissance
Key Command:

nmap -sn 192.x.x.x-254




© 2025 Ashalatha | GitHub: [@Ashalatha2003](https://github.com/Ashalatha2003)
