<div align="center">

# 🦉 OCymulate

**Breach & Attack Simulation Engine**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*Part of the [OwlSec](https://owlsec.org) Toolkit*
```
██████╗  ██████╗██╗   ██╗███╗   ███╗██╗   ██╗██╗      █████╗ ████████╗███████╗
██╔═══██╗██╔════╝╚██╗ ██╔╝████╗ ████║██║   ██║██║     ██╔══██╗╚══██╔══╝██╔════╝
██║   ██║██║      ╚████╔╝ ██╔████╔██║██║   ██║██║     ███████║   ██║   █████╗
██║   ██║██║       ╚██╔╝  ██║╚██╔╝██║██║   ██║██║     ██╔══██║   ██║   ██╔══╝
╚██████╔╝╚██████╗   ██║   ██║ ╚═╝ ██║╚██████╔╝███████╗██║  ██║   ██║   ███████╗
 ╚═════╝  ╚═════╝   ╚═╝   ╚═╝     ╚═╝ ╚═════╝ ╚══════╝╚═╝  ╚═╝   ╚═╝   ╚══════╝
            Recon · HTTP Beacon · DNS Beacon · Obfuscation · Full Chain
```

</div>

---

## 📌 Overview

**OCymulate** is a safe Breach & Attack Simulation (BAS) engine built for purple team exercises and detection validation. All simulations are entirely benign — no real payloads, no credentials, no harmful content.

---

## 🖥️ Simulation Modules

| Option | Module | MITRE TTP | Description |
|--------|--------|-----------|-------------|
| `[1]` | Recon | T1046 | TCP connect scan — network service discovery |
| `[2]` | HTTP Beacon | T1071.001 | Simulate C2 HTTP/HTTPS beacon traffic |
| `[3]` | DNS Beacon | T1071.004 | Simulate DNS resolution beacon patterns |
| `[4]` | Obfuscation | T1027 | Generate and test encoded benign artifact |
| `[5]` | Full Chain | All | Run all modules in sequence |

---

## 📊 Risk Scoring

| Severity | Score |
|----------|-------|
| 🔴 Critical | 95 |
| 🟠 High | 70 |
| 🟡 Medium | 35 |
| 🔵 Low | 10 |

**Risk Level Thresholds:**

| Level | Score |
|-------|-------|
| 🔴 Critical | ≥ 85 |
| 🟠 High | ≥ 65 |
| 🟡 Medium | ≥ 40 |
| 🔵 Low | > 0 |

> Final risk score = average of all event scores + high/critical severity boost.

---

## 🔒 Safety Policy

- Default scope: localhost and private IPs only
- External targets blocked unless explicitly enabled
- All artifacts are benign and auto-deleted after simulation
- No credentials, payloads, or harmful content used

---

## 📁 Output Files

| File | Description |
|------|-------------|
| `ocymulate_report.json` | Full JSON simulation report |
| `ocymulate_report.md` | Markdown report (optional) |

> Files saved in the same directory as OCymulate.

---

## ⚙️ Requirements

- Linux (any distro)
- The tool is pre-built — no Python installation needed

---

## ⚠️ Legal Disclaimer

> **THIS TOOL IS FOR AUTHORIZED PURPLE TEAM EXERCISES ONLY.**  
> Must only be run on networks and systems you own or have explicit written permission to test.  
> Unauthorized use is illegal and unethical.  
> The developer is not responsible for any misuse.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

> 🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
