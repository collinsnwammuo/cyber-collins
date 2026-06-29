## Collins Nwammuo
**SOC Analyst | Network Security | Blue Team Operations**

<a href="https://www.linkedin.com/in/collins-nwammuo-645482248/" target="_blank">
  <img src="https://img.shields.io/badge/-LinkedIn-0072b1?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="mailto:conwamc@gmail.com">
  <img src="https://img.shields.io/badge/-Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>
<a href="https://tryhackme.com/p/conwamc">
  <img src="https://img.shields.io/badge/-TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white" />
</a>
<img src="https://komarev.com/ghpvc/?username=collinsnwammuo&style=flat-square&color=blue" />

---

## 👨‍💻 About Me

I am a Computer Engineering graduate and certified security professional with hands-on experience in network traffic analysis, SIEM operations, threat detection, incident response, and blue team operations. My engineering background in networking, embedded systems, and IoT gives me a deep understanding of how systems and protocols work at a fundamental level -- knowledge I apply directly to identifying and investigating threats.

I have built and operated a full home SOC lab environment on Kali Linux and Windows 10 using VirtualBox, completing over 23 documented practical projects across two portfolios -- network forensics with Wireshark and SIEM operations with Splunk. My work spans packet-level analysis, IDS/IPS detection, SIEM log ingestion, live attack detection, malware PCAP forensics, and the Splunk Boss of the SOC (BOTS v1) real-world investigation challenge.

I hold CompTIA Security+, Cisco CCNA, HCIA Security, and Microsoft AZ-900 certifications.

---

## 🛡️ Core Competencies

```
Network Traffic Analysis        Threat Detection & Hunting       Incident Response
Packet Capture & Forensics      SIEM Operations & Log Analysis   Vulnerability Assessment
Malware Traffic Investigation   IOC Extraction & Documentation   MITRE ATT&CK Framework
IDS/IPS Detection & Tuning      Attack Simulation & Detection    Blue Team Operations
SPL Query Development           Web Policy Enforcement           Detection Engineering
```

---

## 📂 Security Projects

### 🦈 Wireshark Network Analysis Portfolio
**10 practical network forensics investigations | Kali Linux + Windows 10 Home Lab**

Each project includes a full PCAP capture, annotated screenshots, IOC documentation, and a written analysis report mapping findings to MITRE ATT&CK techniques.

| # | Investigation | Key Skills |
|---|--------------|------------|
| 01 | [TCP Handshake & Session Analysis](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/TCP%20Handshake) | Protocol analysis, flag identification, baseline profiling |
| 02 | [DNS Traffic Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/DNS%20Traffic%20Investigation) | Record type analysis, NXDOMAIN detection, DGA indicators |
| 03 | [Cleartext Credential Capture](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Cleartext%20Credential%20Capture) | HTTP/FTP credential extraction, HTTPS comparison |
| 04 | [Nmap Scan Detection & Analysis](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Nmap%20Scan%20Detection) | SYN/NULL/XMAS scan signatures, OS fingerprinting, Windows vs Linux behaviour |
| 05 | [ARP Spoofing / MITM Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ARP%20Spoofing%20MITM%20Detection) | ARP poisoning, gratuitous ARP analysis, traffic interception |
| 06 | [Malware PCAP Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation) | NetSupport RAT C2, SmartApeSG infection chain, IOC extraction |
| 07 | [SSH Brute Force Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/SSH%20Brute%20Force%20Detection) | Brute force signatures, auth log correlation, event timeline |
| 08 | [Rogue DHCP Server Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Rogue%20DHCP%20Server%20Detection) | Protocol abuse detection, DORA sequence analysis |
| 09 | [ICMP Tunnel Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ICMP%20Tunnel%20Detection) | Covert channel identification, payload size anomaly, exfiltration detection |
| 10 | [Full PCAP Forensics Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Full%20PCAP%20Forensics) | End-to-end attack chain reconstruction, formal IR report |

> **Project 06 highlight:** Investigated a real-world malware PCAP from a confirmed NetSupport RAT infection delivered via the SmartApeSG fake browser update campaign. Identified victim hostname, IP, MAC, Windows username, and full name via LDAP -- all from passive network traffic analysis. Reconstructed the full attack chain from `classicgrand.com` compromise through C2 beaconing at 60-second intervals, extracted all IOCs, and mapped findings to MITRE ATT&CK. [View investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation)

---

### 📊 Splunk SIEM Operations Portfolio
**14 practical SIEM projects | Splunk 10.4 | Kali Linux Home Lab**

A complete progression from log ingestion through SPL fundamentals, dashboard building, alert engineering, Zeek network log integration, live attack detection, and the Splunk BOTS v1 real-world investigation challenge.

| # | Project | Key Skills |
|---|---------|------------|
| 01 | [Ingesting Syslog and Apache Logs](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2001) | Multi-source ingestion, sourcetypes, index management |
| 02 | [Search and Filter Commands](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2002) | SPL search, table, fields, where, dedup, rename |
| 03 | [Stats and Aggregation](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2003) | stats, top, rare, dc, values, brute force detection |
| 04 | [Timechart -- Visualising Events Over Time](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2004) | timechart, span tuning, attack pattern visualisation |
| 05 | [Field Extraction with Rex](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2005) | rex, named capture groups, multi-field extraction |
| 06 | [Eval and Calculated Fields](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2006) | eval, if, case, severity classification, risk scoring |
| 07 | [SSH Brute Force Dashboard](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2007) | Dashboard builder, multi-panel SOC monitoring view |
| 08 | [Brute Force Detection Alert](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2008) | Scheduled alerts, threshold tuning, MTTD measurement |
| 09 | [PCAP Ingestion via Zeek](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2009) | Zeek 8.2.0, conn_state analysis, PCAP-to-SIEM pipeline |
| 10 | [Correlating Wireshark Findings](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2010) | Multi-source correlation, IOC hunting, attack timeline |
| 11 | [Live SSH Brute Force Detection](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2011) | Live monitoring, MTTD: 12min 23sec measured |
| 12 | [Live Nmap + HTTP Policy Violation Detection](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2012) | Nmap in HTTP logs, web policy enforcement, repeat offender scoring |
| 13 | [BOTS v1 -- Boss of the SOC Investigation](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2013) | Real-world attack investigation, multi-sourcetype correlation |
| 14 | [SOC Detection Use Case Library](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2014) | Detection engineering, MITRE ATT&CK mapping, rule documentation |

> **Project 11 highlight:** Ran a live SSH brute force attack with Hydra while monitoring Splunk in real time. Measured actual MTTD of 12 minutes 23 seconds, identified tuning gap in alert schedule, and corroborated the attack across three independent evidence sources -- Wireshark PCAP, Zeek conn.log, and Linux auth log.

> **Project 13 highlight:** Completed the Splunk BOTS v1 (Boss of the SOC) real-world attack investigation -- identifying the web scanner, uploaded malware, C2 infrastructure, and exfiltration activity from a simulated Wayne Enterprises compromise using stream:http, suricata, sysmon, wineventlog, and pan:traffic sourcetypes.

---

### 🗺️ Cisco Packet Tracer Network Labs
**Enterprise network design and configuration**

| Project | Technologies |
|---------|-------------|
| [VLAN Segmentation & Inter-VLAN Routing](https://github.com/collinsnwammuo/packet-tracer-projects) | VLAN design, 802.1Q trunking, Layer 3 switching, enterprise topology |

---

## 🧰 Technical Skills

### Network Security & Analysis
<div>
  <img src="https://img.shields.io/badge/-Wireshark-1679A7?&style=for-the-badge&logo=Wireshark&logoColor=white" />
  <img src="https://img.shields.io/badge/-Zeek-777BB4?&style=for-the-badge&logo=Zeek&logoColor=white" />
  <img src="https://img.shields.io/badge/-Suricata-EF3B2D?&style=for-the-badge&logo=Suricata&logoColor=white" />
  <img src="https://img.shields.io/badge/-Nmap-0E83CD?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-tcpdump-black?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-Hydra-darkred?&style=for-the-badge&logoColor=white" />
</div>

### SIEM & Log Analysis
<div>
  <img src="https://img.shields.io/badge/-Splunk-000000?&style=for-the-badge&logo=Splunk&logoColor=white" />
  <img src="https://img.shields.io/badge/-Elastic-005571?&style=for-the-badge&logo=Elastic&logoColor=white" />
  <img src="https://img.shields.io/badge/-Microsoft_Sentinel-0078D4?&style=for-the-badge&logo=Microsoft&logoColor=white" />
</div>

### Endpoint & Incident Response
<div>
  <img src="https://img.shields.io/badge/-Microsoft_Defender-00A4EF?&style=for-the-badge&logo=Microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/-Velociraptor-4B275F?&style=for-the-badge&logo=Velociraptor&logoColor=white" />
  <img src="https://img.shields.io/badge/-TheHive-F0B400?&style=for-the-badge&logoColor=white" />
</div>

### Operating Systems & Infrastructure
<div>
  <img src="https://img.shields.io/badge/-Kali_Linux-557C94?&style=for-the-badge&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/-Linux-FCC624?&style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/-Windows-0078D6?&style=for-the-badge&logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/-VirtualBox-183A61?&style=for-the-badge&logo=virtualbox&logoColor=white" />
</div>

---

## 🎓 Certifications

<div>
  <img src="https://img.shields.io/badge/-Security%2B-FF0000?&style=for-the-badge&logo=CompTIA&logoColor=white" />
  <img src="https://img.shields.io/badge/-CCNA-1A73E8?style=for-the-badge&logo=Cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/-HCIA_Security-0066CC?style=for-the-badge&logo=Huawei&logoColor=white" />
  <img src="https://img.shields.io/badge/-AZ--900-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
</div>

---

## 🛡️ Skills & Associated Work

| Competency | Demonstrated In |
|---|---|
| Network Traffic Analysis & Packet Forensics | [Wireshark Portfolio](https://github.com/collinsnwammuo/Wireshark-projects) -- 10 projects |
| SIEM Operations & SPL Development | [Splunk Portfolio](https://github.com/collinsnwammuo/SIEM-Splunk) -- 14 projects |
| Malware Investigation & IOC Extraction | [Wireshark Project 06](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation) -- NetSupport RAT |
| Live Attack Detection & MTTD Measurement | [Splunk Project 11](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2011) -- SSH brute force |
| PCAP-to-SIEM Pipeline (Zeek) | [Splunk Project 09](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2009) -- Zeek integration |
| Real-World SOC Investigation | [Splunk Project 13](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2013) -- BOTS v1 |
| Detection Engineering & Use Case Library | [Splunk Project 14](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2014) -- MITRE ATT&CK mapped |
| Web Policy Enforcement Monitoring | [Splunk Project 12](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2012) -- HTTP policy violations |
| MITM Attack Detection & Response | [Wireshark Project 05](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ARP%20Spoofing%20MITM%20Detection) -- ARP spoofing |
| Network Design & Routing | [Cisco Packet Tracer Labs](https://github.com/collinsnwammuo/packet-tracer-projects) |

---

## 🕹️ TryHackMe

<div align="center">
  <a href="https://tryhackme.com/p/conwamc">
    <img src="https://tryhackme-badges.vercel.app/api/badges?username=conwamc&theme=dark" alt="TryHackMe" />
  </a>
</div>

---

## 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=collinsnwammuo&show_icons=true&theme=tokyonight" height="150px" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=collinsnwammuo&theme=tokyonight" height="150px" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=collinsnwammuo&layout=compact&theme=tokyonight" height="150px" />
</div>

---

## 🤝 Contact

📩 **Email:** conwamc@gmail.com
🔗 **LinkedIn:** [linkedin.com/in/collins-nwammuo-645482248](https://linkedin.com/in/collins-nwammuo-645482248)
🎯 **TryHackMe:** [tryhackme.com/p/conwamc](https://tryhackme.com/p/conwamc)
