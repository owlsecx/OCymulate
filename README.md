# 🦉 OCymulate

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OAttack%20/%20Offensive-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OCymulate** — Breach & Attack Simulation (BAS)

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OCymulate is a breach-and-attack simulation (BAS) helper for safe purple-team detection testing. It emulates adversary-like beacons and recon behaviours with a default safety policy that restricts targets to localhost and private ranges. External targets require an explicit unsafe opt-in so drills stay controlled.

---

## ✨ Features

- Module-based BAS runs for HTTP/DNS-style beacon and recon behaviours
- Default localhost/private-only targeting with dry-run support
- Explicit --unsafe-external gate for authorised external drills
- Configurable beacon count, ports, URL, and DNS domain parameters
- MITRE coverage export plus optional Markdown reports
- Non-interactive --yes mode for scripted detection pipelines

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCymulate --module beacon --target 127.0.0.1 --dry-run
./OCymulate --module recon --target 10.0.0.5 --ports 80,443 --yes
./OCymulate --mitre-export --save-md
./OCymulate --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
