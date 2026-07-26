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

## About Me

I am a Computer Engineering graduate and certified security professional with hands-on experience in network traffic analysis, SIEM operations, threat detection, endpoint monitoring, and blue team operations. My engineering background in networking, embedded systems, and IoT gives me a deep understanding of how systems and protocols work at a fundamental level, and I apply that knowledge directly to identifying and investigating threats.

I have built and operated a full home SOC lab environment on Kali Linux and Windows 10 using VirtualBox, spanning network forensics, SIEM engineering, intrusion detection, vulnerability management, threat intelligence, and endpoint detection and response across three separate platforms. My work covers packet level analysis, IDS/IPS detection and tuning, SIEM log ingestion across Splunk, ELK, and Microsoft Sentinel, live attack detection, malware PCAP forensics, EDR investigation across Microsoft Defender for Endpoint and CrowdStrike Falcon, vulnerability scanning with real exploitable findings, CVE research, and the Splunk Boss of the SOC (BOTS v1) real world investigation challenge.

I hold CompTIA Security+, ISC2 Certified in Cybersecurity (CC), Cisco Junior Cybersecurity Analyst, Cisco CCNA, Huawei HCIA Security, and Microsoft AZ-900 certifications.

---

## Core Competencies

```
Network Traffic Analysis        Threat Detection & Hunting       Incident Response
Packet Capture & Forensics      SIEM Operations & Log Analysis   Vulnerability Assessment
Malware Traffic Investigation   IOC Extraction & Documentation   MITRE ATT&CK Framework
IDS/IPS Detection & Tuning      Endpoint Detection & Response     Threat Intelligence & CVE Research
Attack Simulation & Detection   Blue Team Operations              Detection Engineering
SPL Query Development           KQL Query Development             Web Policy Enforcement
Network Reconnaissance          Cloud SIEM Engineering
```

---

## Security Projects

### 1. Network Forensics & Traffic Analysis

**Wireshark Network Analysis Portfolio**, 10 practical investigations, Kali Linux + Windows 10 home lab.

Each project includes a full PCAP capture, annotated screenshots, IOC documentation, and a written analysis report mapped to MITRE ATT&CK techniques.

| # | Investigation | Key Skills |
|---|--------------|------------|
| 01 | [TCP Handshake & Session Analysis](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/TCP%20Handshake) | Protocol analysis, flag identification, baseline profiling |
| 02 | [DNS Traffic Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/DNS%20Traffic%20Investigation) | Record type analysis, NXDOMAIN detection, DGA indicators |
| 03 | [Cleartext Credential Capture](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Cleartext%20Credential%20Capture) | HTTP/FTP credential extraction, HTTPS comparison |
| 04 | [Nmap Scan Detection & Analysis](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Nmap%20Scan%20Detection%20%26%20Analysis) | SYN/NULL/XMAS scan signatures, OS fingerprinting, Windows vs Linux behaviour |
| 05 | [ARP Spoofing / MITM Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ARP%20Spoofing%20%26%20MITM%20Detection) | ARP poisoning, gratuitous ARP analysis, traffic interception |
| 06 | [Malware PCAP Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation) | NetSupport RAT C2, SmartApeSG infection chain, IOC extraction |
| 07 | [SSH Brute Force Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/SSH%20Brute%20Force%20Detection) | Brute force signatures, auth log correlation, event timeline |
| 08 | [Rogue DHCP Server Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Rogue%20DHCP%20Server%20Detection) | Protocol abuse detection, DORA sequence analysis |
| 09 | [ICMP Tunnel Detection](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ICMP%20Tunnel%20Detection) | Covert channel identification, payload size anomaly, exfiltration detection |
| 10 | [Full PCAP Forensics Investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Full%20PCAP%20Forensics) | End to end attack chain reconstruction, formal IR report |

> **Highlight, Project 06:** I investigated a real world malware PCAP from a confirmed NetSupport RAT infection delivered via the SmartApeSG fake browser update campaign. I identified the victim hostname, IP, MAC, Windows username, and full name via LDAP, all from passive network traffic analysis. I reconstructed the full attack chain from the `classicgrand.com` compromise through C2 beaconing at 60 second intervals, extracted all IOCs, and mapped findings to MITRE ATT&CK. [View investigation](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation)

**[nmap-recon-lab](https://github.com/collinsnwammuo/nmap-recon-lab)**: network reconnaissance from the attacker's perspective, host discovery, full service/OS detection, UDP scanning, and NSE vulnerability scripting against my lab environment.

> **Highlight:** My initial ping sweep and first full scan attempt against my own Windows 10 VM both failed silently, the host was actually up but its firewall was dropping ICMP probes by default. I diagnosed this as a false negative rather than a down host, and documented `-Pn` as the correct fix, a realistic reconnaissance blind spot that would cause a real asset-discovery sweep to miss a live host entirely.

---

### 2. SIEM, Detection Engineering & Intrusion Detection

**Splunk SIEM Operations Portfolio**, 14 practical projects, Splunk 10.4, Kali Linux home lab.

A complete progression from log ingestion through SPL fundamentals, dashboard building, alert engineering, Zeek network log integration, live attack detection, and the Splunk BOTS v1 real world investigation challenge.

| # | Project | Key Skills |
|---|---------|------------|
| 01 | [Ingesting Syslog and Apache Logs](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Ingesting%20Syslog%20and%20Apache%20Logs) | Multi-source ingestion, sourcetypes, index management |
| 02 | [Search and Filter Commands](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Search%20and%20Filter%20Commands) | SPL search, table, fields, where, dedup, rename |
| 03 | [Stats and Aggregation](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Stats%20and%20Aggregation) | stats, top, rare, dc, values, brute force detection |
| 04 | [Timechart: Visualising Events Over Time](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Timechart%20--%20Visualising%20Events%20Over%20Time) | timechart, span tuning, attack pattern visualisation |
| 05 | [Field Extraction with Rex](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Field%20Extraction%20with%20Rex) | rex, named capture groups, multi-field extraction |
| 06 | [Eval and Calculated Fields](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Eval%20and%20Calculated%20Fields) | eval, if, case, severity classification, risk scoring |
| 07 | [SSH Brute Force Dashboard](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/SSH%20Login%20Dashboard) | Dashboard builder, multi panel SOC monitoring view |
| 08 | [Brute Force Detection Alert](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Brute%20Force%20Detection%20Alert) | Scheduled alerts, threshold tuning, MTTD measurement |
| 09 | [PCAP Ingestion via Zeek](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Ingest%20Wireshark%20PCAPs%20via%20Zeek) | Zeek 8.2.0, conn_state analysis, PCAP to SIEM pipeline |
| 10 | [Correlating Wireshark Findings](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Correlate%20Wireshark%20Findings%20in%20Splunk) | Multi source correlation, IOC hunting, attack timeline |
| 11 | [Live SSH Brute Force Detection](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Live%20Attack%20Detection%20--%20SSH%20Brute%20Force) | Live monitoring, MTTD measured at 12 min 23 sec |
| 12 | [Live Nmap + HTTP Policy Violation Detection](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Live%20Attack%20Detection%3A%20Nmap%20Scan%20%2B%20HTTP%20Policy%20Violations) | Nmap in HTTP logs, web policy enforcement, repeat offender scoring |
| 13 | [BOTS v1: Boss of the SOC Investigation](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/BOTS%20v1%3A%20SOC%20Investigation) | Real world attack investigation, multi sourcetype correlation |
| 14 | [SOC Detection Use Case Library](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2014) | Detection engineering, MITRE ATT&CK mapping, rule documentation |

> **Highlight, Project 11:** I ran a live SSH brute force attack with Hydra while monitoring Splunk in real time. I measured an actual MTTD of 12 minutes 23 seconds, identified a tuning gap in the alert schedule, and corroborated the attack across three independent evidence sources: Wireshark PCAP, Zeek conn.log, and the Linux auth log.

> **Highlight, Project 13:** I completed the Splunk BOTS v1 (Boss of the SOC) real world attack investigation, identifying the web scanner, uploaded malware, C2 infrastructure, and exfiltration activity from a simulated Wayne Enterprises compromise using stream:http, suricata, sysmon, wineventlog, and pan:traffic sourcetypes.

**[SIEM-ELK-Stack](https://github.com/collinsnwammuo/SIEM-ELK-Stack)**: standalone ELK deployment (Elasticsearch 8, Kibana, Filebeat) built and debugged from a clean install, including resolving real ingestion and configuration failures rather than following a pre-solved guide. Includes a direct Splunk vs Kibana comparison built on identical source data.

**[Suricata-IDS-Lab](https://github.com/collinsnwammuo/Suricata-IDS-Lab)**: Suricata IDS deployment with custom detection rules for SSH brute force, NetSupport RAT C2 traffic, suspicious user agents, and Nmap NULL scans. Includes resolving a dual interface af-packet configuration issue. Live testing against a Hydra SSH brute force attack brought detection time down to roughly 0.87 seconds, compared with the 12 minute 23 second baseline measured in the Splunk lab above. Also documents a genuine detection gap, FIN and TCP connect scans passed through undetected by both the custom ruleset and ET/open.

---

### 3. Endpoint Detection & Response and Cloud SIEM

**[edr-xdr-lab](https://github.com/collinsnwammuo/EDR-XDR)**: multi-platform EDR/XDR deployment against the same Windows 10 VM used throughout my lab, covering onboarding, detection triggering, alert triage, and cross-platform investigation workflow.

| Platform | Status | Highlight |
|---|---|---|
| Microsoft Defender for Endpoint | ✅ Complete | Full tenant setup, device onboarding, and a triggered EICAR detection. Traced the complete device timeline from browser download warning through cloud-side alert generation, measured a real ~15 minute local-to-cloud sync delay, and found a MITRE ATT&CK tagging inconsistency between the consolidated alert and an unrelated event in the same timeline window |
| Microsoft Sentinel | ✅ Complete | Connected a cloud SIEM directly to the Defender for Endpoint tenant above. Diagnosed a "connected but zero data" state as a non-backfilling connector rather than a broken integration, then confirmed full ingestion with a fresh detection. Built a KQL-based workbook dashboard covering alert volume, severity, and raw alert detail |
| CrowdStrike Falcon | ⏳ Trial pending sales review | Signup requires vendor approval rather than instant self-serve access |

> **Highlight:** Rather than treating these as isolated tool installs, I connected Microsoft Defender for Endpoint's real alert data directly into Microsoft Sentinel, so the same EICAR detection is independently traceable across two platforms end to end, endpoint-level block, cloud EDR alert, and cloud SIEM incident, all from one trigger event.

---

### 4. Vulnerability Management & Threat Intelligence

**[openvas-vuln-management](https://github.com/collinsnwammuo/OpenVAS)**: Greenbone/OpenVAS deployment and full vulnerability scans against both a hardened Windows 10 VM and a deliberately vulnerable Metasploitable 2 VM.

> **Highlight:** Diagnosed a feed synchronization failure that blocked scan creation (isolated it to specific background data feeds rather than a broken install), then ran full scans producing 3 findings on the hardened host versus 38 on Metasploitable 2, including two critical, unauthenticated, publicly-exploitable backdoors (vsftpd CVE-2011-2523 and UnrealIRCd CVE-2010-2075), each mapped to MITRE ATT&CK.

**[threat-intel-lab](https://github.com/collinsnwammuo/Threat-Intelligence---CVE-Research)**: CVE exploitability research and IOC enrichment, built directly on findings from my own OpenVAS and Wireshark investigations rather than generic examples.

> **Highlight:** Researched the real-world exploitability of the two critical CVEs found in my OpenVAS scan, confirming both have fully weaponized, zero-authentication public Metasploit modules despite neither appearing in CISA's KEV catalog. Separately, re-investigated the C2 IP from my Wireshark NetSupport RAT case and found independent corroboration across three unrelated public sources, including a separate analyst's writeup of the exact same exercise, confirming the same `/24` block as reused NetSupport RAT infrastructure.

---

### 5. Network Design & Infrastructure

**[Cisco-Packet-Tracer-Projects](https://github.com/collinsnwammuo/Cisco-Packet-Tracer-Projects)**: enterprise network design and configuration, including VLAN segmentation, 802.1Q trunking, and Layer 3 switching across a full enterprise topology.

---

## Technical Skills

**Network Security & Analysis**
<div>
  <img src="https://img.shields.io/badge/-Wireshark-1679A7?&style=for-the-badge&logo=Wireshark&logoColor=white" />
  <img src="https://img.shields.io/badge/-Zeek-777BB4?&style=for-the-badge&logo=Zeek&logoColor=white" />
  <img src="https://img.shields.io/badge/-Suricata-EF3B2D?&style=for-the-badge&logo=Suricata&logoColor=white" />
  <img src="https://img.shields.io/badge/-Nmap-0E83CD?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-tcpdump-black?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-Hydra-darkred?&style=for-the-badge&logoColor=white" />
</div>

**SIEM & Log Analysis**
<div>
  <img src="https://img.shields.io/badge/-Splunk-000000?&style=for-the-badge&logo=Splunk&logoColor=white" />
  <img src="https://img.shields.io/badge/-Elastic-005571?&style=for-the-badge&logo=Elastic&logoColor=white" />
  <img src="https://img.shields.io/badge/-Microsoft_Sentinel-0078D4?&style=for-the-badge&logo=Microsoft&logoColor=white" />
</div>

**Endpoint Detection, Response & Vulnerability Management**
<div>
  <img src="https://img.shields.io/badge/-Microsoft_Defender-00A4EF?&style=for-the-badge&logo=Microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/-CrowdStrike_Falcon-E01F27?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-Velociraptor-4B275F?&style=for-the-badge&logo=Velociraptor&logoColor=white" />
  <img src="https://img.shields.io/badge/-TheHive-F0B400?&style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-OpenVAS-88CC14?&style=for-the-badge&logoColor=white" />
</div>

**Operating Systems & Infrastructure**
<div>
  <img src="https://img.shields.io/badge/-Kali_Linux-557C94?&style=for-the-badge&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/-Linux-FCC624?&style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/-Windows-0078D6?&style=for-the-badge&logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/-VirtualBox-183A61?&style=for-the-badge&logo=virtualbox&logoColor=white" />
  <img src="https://img.shields.io/badge/-Microsoft_Azure-0089D6?&style=for-the-badge&logo=microsoftazure&logoColor=white" />
</div>

---

## Certifications

<div>
  <img src="https://img.shields.io/badge/-Security%2B-FF0000?&style=for-the-badge&logo=CompTIA&logoColor=white" />
  <img src="https://img.shields.io/badge/-ISC2%20CC-0072C6?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-CCNA-1A73E8?style=for-the-badge&logo=Cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/-Junior%20Cybersecurity%20Analyst-1A73E8?style=for-the-badge&logo=Cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/-HCIA_Security-0066CC?style=for-the-badge&logo=Huawei&logoColor=white" />
  <img src="https://img.shields.io/badge/-AZ--900-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
</div>

---

## Skills & Associated Work

| Competency | Demonstrated In |
|---|---|
| Network Traffic Analysis & Packet Forensics | [Wireshark Portfolio](https://github.com/collinsnwammuo/Wireshark-projects), 10 projects |
| Reconnaissance & Scanning Detection | [nmap-recon-lab](https://github.com/collinsnwammuo/nmap-recon-lab) |
| SIEM Operations & SPL Development | [Splunk Portfolio](https://github.com/collinsnwammuo/SIEM-Splunk), 14 projects |
| SIEM Platform Engineering (ELK) | [SIEM-ELK-Stack](https://github.com/collinsnwammuo/SIEM-ELK-Stack) |
| Cloud SIEM Engineering (KQL) | [edr-xdr-lab](https://github.com/collinsnwammuo/EDR-XDR), Microsoft Sentinel |
| IDS Deployment & Custom Rule Writing | [Suricata-IDS-Lab](https://github.com/collinsnwammuo/Suricata-IDS-Lab) |
| Malware Investigation & IOC Extraction | [Wireshark Project 06](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/Malware%20PCAP%20Investigation), NetSupport RAT |
| Live Attack Detection & MTTD Measurement | [Splunk Project 11](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Live%20Attack%20Detection%20--%20SSH%20Brute%20Force) and [Suricata-IDS-Lab](https://github.com/collinsnwammuo/Suricata-IDS-Lab) |
| PCAP to SIEM Pipeline (Zeek) | [Splunk Project 09](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Ingest%20Wireshark%20PCAPs%20via%20Zeek) |
| Real World SOC Investigation | [Splunk Project 13](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/BOTS%20v1%3A%20SOC%20Investigation), BOTS v1 |
| Endpoint Detection & Response | [edr-xdr-lab](https://github.com/collinsnwammuo/EDR-XDR), Microsoft Defender for Endpoint + CrowdStrike Falcon |
| Vulnerability Management | [openvas-vuln-management](https://github.com/collinsnwammuo/OpenVAS) |
| Threat Intelligence & CVE Research | [threat-intel-lab](https://github.com/collinsnwammuo/Threat-Intelligence---CVE-Research) |
| Web Policy Enforcement Monitoring | [Splunk Project 12](https://github.com/collinsnwammuo/SIEM-Splunk/tree/main/Project%2012) |
| MITM Attack Detection & Response | [Wireshark Project 05](https://github.com/collinsnwammuo/Wireshark-projects/tree/main/ARP%20Spoofing%20MITM%20Detection) |
| Network Design & Routing | [Cisco Packet Tracer Labs](https://github.com/collinsnwammuo/Cisco-Packet-Tracer-Projects) |

---

## TryHackMe

<div align="center">
  <a href="https://tryhackme.com/p/conwamc">
    <img src="https://tryhackme-badges.vercel.app/api/badges?username=conwamc&theme=dark" alt="TryHackMe" />
  </a>
</div>

---

## GitHub Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=collinsnwammuo&show_icons=true&theme=tokyonight" height="150px" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=collinsnwammuo&theme=tokyonight" height="150px" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=collinsnwammuo&layout=compact&theme=tokyonight" height="150px" />
</div>

---

## Contact

**Email:** conwamc@gmail.com
**LinkedIn:** [linkedin.com/in/collins-nwammuo-645482248](https://linkedin.com/in/collins-nwammuo-645482248)
**TryHackMe:** [tryhackme.com/p/conwamc](https://tryhackme.com/p/conwamc)
