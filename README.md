# SCADAGuard-OSINT
An Open-Source OSINT Reconnaissance Framework for Industrial Control Systems (ICS), SCADA, and OT Security.
This is a conceptual sibling project to the CyberSalukis-Healthguard-OSINT repo. It adapts the same modular, responsible, TIPPSS-aligned (or equivalent OT-focused) design but tailored to the unique risks of SCADA/ICS/OT environments. 
The purpose is to help defenders (asset owners, OT security teams, red teams with authorization) map and reduce the external attack surface of SCADA/ICS systems using OSINT and autoamtion to mitigate risks from AI integration and relationships.
Inspired by HealthGuard: Same CLI structure, modules, reporting, Docker support, YAML query libraries, and responsible-use emphasis.
Key Differences:
Focus on industrial protocols, critical infrastructure sectors (energy, water, manufacturing, transport, etc.).
Emphasis on Shodan/Censys/IVRE for device discovery, protocol-specific dorks, vendor firmware leaks, and OT-specific intelligence.
Core Features (Mirroring HealthGuard)
Dork-scan: Google/Bing/Brave/Mojeek dorks for SCADA configs, vendor portals, exposed HMIs, etc.
Shodan-scan/Censys-scan: Protocol-specific queries (Modbus 502, DNP3 20000, Siemens S7, etc.), country/sector filters.
Github-intel: Search for exposed PLC code, .scd files, engineering station dumps, vendor credentials.
Ivre-recon /Leakix-scan: Network/ leak discovery for OT assets.
Vendor-intel: Supply chain (Siemens, Rockwell, Schneider, etc.) intel, CVE correlations.
Protocol-Recon: Fingerprinting exposed services, banner grabbing (careful!).
Social-Recon: OT personnel (engineers, integrators) exposure.
Report:Structured reports mapped to ICS risk frameworks, with severity, remediation, and visualizations (e.g., device heatmaps).
Responsible Use Built-In:
Passive-first mode.
Explicit authorization flags for any active probes.
Strong warnings against unauthorized use! Do not use this repo for illegal and dangerous in critical infrastructure.
