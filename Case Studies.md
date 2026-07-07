# ICS/OT Cybersecurity Case Studies
*A living document for learning, teaching, and expanding real-world Industrial Control Systems (ICS) and Operational Technology (OT) cybersecurity incidents.*

---

# Table of Contents

1. Stuxnet (2010)
2. Ukraine Power Grid Attack (2015)
3. Triton / Trisis Malware (2017)
4. Colonial Pipeline Ransomware (2021)
5. Oldsmar Water Treatment Incident (2021)
6. NotPetya (2017)
7. Industroyer / CrashOverride (2016)
8. Target HVAC Vendor Breach (2013)
9. German Steel Mill Attack (2014)
10. Maroochy Shire Sewage Spill (2000)
11. Key Takeaways
12. Learning Roadmap

---

# 1. Stuxnet (2010)

## Industry
Nuclear Energy

## Country
Iran

## Threat Type
State-sponsored malware

## Primary Target
PLC-controlled uranium centrifuges

## Overview

Stuxnet was the world's first publicly known malware specifically engineered to manipulate industrial control systems (ICS). It targeted Siemens PLCs used at Iran's Natanz uranium enrichment facility.

Rather than simply stealing information, the malware modified PLC logic to change centrifuge speeds while reporting normal operating values back to the operators.

This demonstrated that cyber attacks could cause real physical destruction.

---

## ICS Components

- PLC
- HMI
- Engineering Workstation
- Windows Systems
- Siemens Step7 Software
- Industrial Network

---

## Attack Chain

USB Drive
→ Windows Computer
→ Engineering Workstation
→ PLC
→ Centrifuge Control
→ Physical Damage

---

## Impact

- Hundreds of centrifuges destroyed
- Significant delay to Iran's nuclear program
- First malware known to cause physical equipment damage

---

## Key Lessons

- Air-gapped systems are not completely secure
- USB devices are a major attack vector
- PLC logic integrity must be monitored
- Engineering workstations require strong protection
- Physical processes can be manipulated through cyber attacks

---

# 2. Ukraine Power Grid Attack (2015)

## Industry

Electric Power

## Country

Ukraine

## Threat Type

Targeted cyber attack

## Overview

Attackers spent months inside utility networks after gaining access through phishing emails.

They stole administrator credentials, remotely accessed SCADA systems, opened circuit breakers, disabled UPS systems, and launched denial-of-service attacks against customer call centers.

Over 200,000 customers lost power.

---

## ICS Components

- SCADA
- HMI
- VPN
- Active Directory
- Distribution Automation
- Remote Access Systems

---

## Attack Chain

Phishing Email
→ IT Network
→ Credential Theft
→ Remote Access
→ SCADA
→ Open Breakers
→ Power Outage

---

## Impact

- 200,000+ customers without electricity
- Manual restoration required
- Operators temporarily lost visibility of substations

---

## Key Lessons

- Protect remote access with MFA
- Monitor privileged accounts
- Segment IT and OT networks
- Train employees against phishing attacks

---

# 3. Triton / Trisis Malware (2017)

## Industry

Oil & Gas

## Country

Saudi Arabia

## Threat Type

Safety Instrumented System (SIS) attack

## Overview

Unlike previous attacks targeting production systems, Triton specifically targeted Safety Instrumented Systems (SIS).

The attackers attempted to manipulate emergency shutdown controllers that protect industrial facilities during dangerous situations.

If successful, the attack could have resulted in explosions or loss of life.

---

## ICS Components

- Safety Instrumented System (SIS)
- Triconex Controllers
- Engineering Workstation
- Industrial Network

---

## Attack Chain

IT Network
→ Engineering Workstation
→ SIS Controller
→ Modify Safety Logic

---

## Impact

- Safety systems compromised
- Potential risk to human life
- Demonstrated attacks against safety systems

---

## Key Lessons

- Separate safety systems from production systems
- Monitor SIS engineering workstations
- Safety systems require independent security controls

---

# 4. Colonial Pipeline Ransomware (2021)

## Industry

Oil & Gas Pipeline

## Country

United States

## Threat Type

Ransomware

## Overview

A ransomware attack affected Colonial Pipeline's corporate IT systems.

Although operational technology was not directly compromised, pipeline operations were shut down because business systems such as billing and logistics became unavailable.

---

## ICS Components

- Corporate IT
- Business Systems
- SCADA (Indirectly Affected)
- Pipeline Operations

---

## Attack Chain

Internet
→ Corporate IT
→ Ransomware
→ Business Operations Disrupted
→ Pipeline Shutdown

---

## Impact

- Fuel shortages across multiple states
- Temporary shutdown of major fuel pipeline
- Significant economic disruption

---

## Key Lessons

- IT outages can stop OT operations
- Business continuity planning is essential
- Separate IT and OT environments

---

# 5. Oldsmar Water Treatment Incident (2021)

## Industry

Water Treatment

## Country

United States

## Threat Type

Unauthorized Remote Access

## Overview

An attacker gained remote desktop access to a water treatment facility and attempted to dramatically increase sodium hydroxide (lye) levels.

An operator observed the cursor moving unexpectedly and reversed the changes before damage occurred.

---

## ICS Components

- SCADA
- HMI
- Remote Desktop
- Chemical Dosing System

---

## Attack Chain

Remote Access
→ Operator Workstation
→ Chemical Control System
→ Attempted Chemical Change

---

## Impact

- No public harm
- Demonstrated vulnerabilities in remote access

---

## Key Lessons

- Secure remote access
- Enable multi-factor authentication
- Monitor operator sessions
- Limit remote administration privileges

---

# 6. NotPetya (2017)

## Industry

Global Manufacturing & Logistics

## Threat Type

Destructive Malware

## Overview

Originally appearing as ransomware, NotPetya was actually a destructive wiper.

Many global manufacturers and logistics companies experienced massive operational disruptions, forcing production lines and logistics operations offline.

---

## Industries Impacted

- Shipping
- Manufacturing
- Pharmaceuticals
- Food Production

---

## Attack Chain

Software Update
→ Corporate IT
→ Lateral Movement
→ Enterprise-wide Infection
→ Business Shutdown

---

## Impact

- Multi-billion dollar losses
- Manufacturing interruptions
- Global logistics disruptions

---

## Key Lessons

- OT depends heavily on IT infrastructure
- Patch management is critical
- Network segmentation limits spread

---

# 7. Industroyer / CrashOverride (2016)

## Industry

Electric Utilities

## Country

Ukraine

## Threat Type

Protocol-aware Malware

## Overview

Industroyer was designed to communicate directly with industrial protocols used by electrical substations.

Instead of encrypting systems, it issued legitimate control commands to electrical equipment.

---

## ICS Components

- SCADA
- RTUs
- Protective Relays
- Industrial Communication Protocols

---

## Supported Protocols

- IEC 60870-5-101
- IEC 60870-5-104
- IEC 61850

---

## Impact

- Power outages
- Loss of operational control

---

## Key Lessons

- Industrial protocols often lack authentication
- Deep protocol monitoring is essential
- Secure substation communications

---

# 8. Target HVAC Vendor Breach (2013)

## Industry

Retail

## Threat Type

Third-party Vendor Compromise

## Overview

Attackers compromised Target through credentials stolen from an HVAC contractor.

Although this was primarily an IT breach, it demonstrated how vendor access can become a gateway into larger enterprise environments.

This lesson is directly applicable to ICS environments where vendors frequently maintain remote access.

---

## Key Lessons

- Control vendor access
- Enforce least privilege
- Monitor third-party connections
- Segment vendor networks

---

# 9. German Steel Mill Attack (2014)

## Industry

Steel Manufacturing

## Country

Germany

## Threat Type

Industrial Network Compromise

## Overview

Attackers compromised corporate systems before moving into industrial networks.

They interfered with blast furnace shutdown procedures, resulting in physical damage.

---

## ICS Components

- PLC
- SCADA
- Industrial Network
- Blast Furnace Controls

---

## Impact

- Physical equipment damage
- Production disruption

---

## Key Lessons

- Strong IT/OT segmentation
- Monitor lateral movement
- Protect engineering workstations

---

# 10. Maroochy Shire Sewage Spill (2000)

## Industry

Wastewater

## Country

Australia

## Threat Type

Insider Threat

## Overview

A former contractor used stolen radio equipment to remotely manipulate wastewater pumping stations.

Millions of liters of untreated sewage were released into nearby waterways.

---

## ICS Components

- Remote Telemetry Units (RTUs)
- Wireless Control
- Wastewater Control Systems

---

## Attack Chain

Former Employee
→ Stolen Radio Equipment
→ RTUs
→ Pump Control
→ Sewage Spill

---

## Impact

- Environmental damage
- Service disruption
- Highlighted insider threats

---

## Key Lessons

- Revoke access immediately after employment ends
- Secure wireless industrial communications
- Monitor insider activity

---

# Common Themes Across All Case Studies

## Initial Access

- Phishing
- USB devices
- Vendor access
- Remote Desktop
- VPN compromise
- Insider threats

---

## Targeted ICS Assets

- PLCs
- HMIs
- SCADA servers
- Engineering Workstations
- SIS Controllers
- RTUs
- Historians

---

## Common Weaknesses

- Weak authentication
- Flat networks
- Poor segmentation
- Legacy systems
- Shared credentials
- Lack of monitoring

---

## Typical Business Impacts

- Production downtime
- Equipment damage
- Environmental damage
- Safety risks
- Financial losses
- Service disruption
- Loss of public trust

---

# Best Practices

## Network Security

- Segment IT and OT
- Implement Zero Trust principles
- Restrict remote access
- Use industrial firewalls

---

## Identity & Access Management

- Multi-Factor Authentication (MFA)
- Least privilege
- Privileged Access Management (PAM)
- Regular credential reviews

---

## Monitoring

- Asset inventory
- Continuous network monitoring
- ICS protocol inspection
- Security Information and Event Management (SIEM)

---

## Engineering Security

- Backup PLC logic
- Verify controller configurations
- Monitor engineering workstations
- Validate firmware integrity

---

## Incident Response

- Develop OT-specific response plans
- Practice recovery procedures
- Coordinate IT and OT teams
- Maintain offline backups

---

# Learning Roadmap

## Beginner

- Stuxnet
- Oldsmar Water Treatment
- Colonial Pipeline

Focus:
- Understanding ICS basics
- Remote access risks
- IT vs OT relationships

---

## Intermediate

- Ukraine Power Grid
- German Steel Mill
- Maroochy Shire

Focus:
- SCADA attacks
- Lateral movement
- Insider threats

---

## Advanced

- Triton
- Industroyer
- NotPetya

Focus:
- Safety Instrumented Systems
- Industrial protocols
- Enterprise-wide operational resilience

---

# Future Topics to Add

- MITRE ATT&CK for ICS mapping
- Purdue Model architecture
- IEC 62443 security standards
- NIST SP 800-82 guidance
- ISA/IEC 62443 zones and conduits
- ICS incident response playbooks
- OT asset discovery
- Industrial protocols (Modbus, DNP3, OPC UA, PROFINET, EtherNet/IP)
- Real-world ransomware targeting manufacturing
- Secure remote maintenance
- Supply chain attacks affecting ICS
- OT vulnerability management
- Case studies from energy, water, transportation, and manufacturing sectors
- Emerging threats involving IIoT and cloud-connected OT

---

# References 

- CISA ICS Advisories
- MITRE ATT&CK for ICS
- NIST SP 800-82
- IEC 62443 Series
- SANS ICS Resources
- Dragos Threat Reports
- Mandiant OT Reports
- ICS-CERT Historical Advisories
