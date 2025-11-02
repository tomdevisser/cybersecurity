# Defensive Security Intro

Defensive security is concerned with two main tasks:

1. Preventing intrusions from occuring
2. Detecting intrustions when they occur, and responding properly

Blue teams are part of the defensive security landscape.

## Tasks

- Creating cybersecurity awareness
- Documenting and managing assets
- Updating and patching systems
- Setting up preventative security devices (like firewalls and IPSs)
- Setting up logging and monitoring devices

Other topics include:

- Security Operations Center (SOC)
- Threat intelligence
- Digital forensics and incident response (DFIR)
- Malware analysis

## Security Operations Center (SOC)

A team of security professionals that monitors the network and its systems to detect malicious cybersecurity events.

Some areas of interest are:

- Vulnerabilities — although remediating vulnerabilities is not necessarily assigned to SOC
- Policy violations
- Unauthorized activity
- Network intrusions

## Threat intelligence

Information you gather about actual and potential enemies to help the company better prepare against potential adversaries. A _threat_ is any action that can disrupt or adversely affect a system. Purpose: achieve a _threat-informed defence_.

Intelligence needs data, collected from local sources such as network logs and public sources such as forums, processed into a format suitable for analysis.

## Digital Forensics and Incident Response (DFIR)

### Digital forensics

The application of science to investigate crimes and establish facts. Focus on different areas:

- File system — installed programs, files
- System memory — if a malicious program runs in memory without being saved to the disk
- System logs
- Network logs

### Incident response

The methodology that should be followed to handle incidents. The aim: to reduce damage and recover in the shortest time possible.

Four major phases:

1. Preparation
2. Detection and analysis
3. Containment, eradication and recovery
4. Post-incident activity — a report, and sharing lessons learned

### Malware analysis

Malware — malicious software — comes in many types, such as:

- A virus — a piece of code designed to spread, altering, overwriting or deleting files
- Trojan Horse — a program that shows a desirable function, but hides a malicious function underneath
- Ransomware — a malicious program that encrypts the user's files, offering the encryption password if the user pays a _ransom_

There's two types of analysis:

1. Static analysis — inspecting the malicious program without running it (usually requires knowledge of assembly language)
2. Dynamic analysis — running the malware in a controlled environment and monitoring its activvities

## Practical example notes

A _SIEM_ tool (Security Information and Event Management), gathers security=related information and events from varous sources and presents them in one dashboard.

Malicous IP found: 143.110.250.149

You can use open-source databases like AbuseIPDB and Cisco Talos Intelligence to perform reputation and location checks for IP addresses.

A good next step is to block the IP address using a firewall.
