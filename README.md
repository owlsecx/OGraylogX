# 🦉 OGraylogX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OGraylogX** — Graylog Server Configuration Hardening Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OGraylogX — Graylog Server Configuration Hardening Auditor. It provides stdlib properties / YAML-lite / JSON / pipeline / proxy parsers; server.conf & graylog.yml — password_secret, root hash, HTTP/TLS, trusted proxies, CORS, ES/OS hosts, MongoDB URI, SMTP, journal. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Stdlib properties / YAML-lite / JSON / pipeline / proxy parsers
- server.conf & graylog.yml — password_secret, root hash, HTTP/TLS, trusted proxies, CORS, ES/OS hosts, MongoDB URI, SMTP, journal
- LDAP / AD / OIDC / trusted-header auth; input, stream, pipeline, user & content-pack exports; /etc/graylog tree & plugin dir modes
- nginx / Apache reverse-proxy review; secrets masked everywhere
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0, CWE + ATT&CK
- Self-test --demo, CI gates --fail-on / --min-severity, templates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OGraylogX                                     # interactive menu
./OGraylogX --scan -r /path/to/root
./OGraylogX --demo
./OGraylogX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, bundled CPython version, and every bundled library with its exact
  version and license. Feed it to Grype, Trivy or Dependency-Track to audit
  our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

**No telemetry, no analytics, no licence check-in.** This tool does not phone
home. Verify that claim yourself:

```bash
sudo strace -f -e trace=network ./OGraylogX --help   # watch every network call
firejail --net=none ./OGraylogX --help               # deny the network entirely
```

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
