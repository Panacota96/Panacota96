<p align="center">
  <img src="./assets/profile-header.svg" alt="David Santiago Gonzalez Rico - Rakvor DFIR tools" width="100%" />
</p>

<h1 align="center">David Santiago Gonzalez Rico</h1>

<p align="center"><strong>Digital forensics · Pentesting · SOC — for SMEs in Colombia and France</strong></p>

<p align="center">
  I build <strong>Rakvor</strong>, a suite of digital-forensics tools written in Rust for examiners who have to
  defend their findings in court. Every tool reports <em>signals, not verdicts</em>, and keeps a tamper-evident record of
  everything it did.
</p>

<p align="center">
  <a href="https://github.com/Panacota96/rv-hub/releases/latest"><img src="https://img.shields.io/github/v/release/Panacota96/rv-hub?label=RV%20Hub&style=for-the-badge&color=6B00FF" alt="RV Hub latest release" /></a>
  <a href="https://www.linkedin.com/in/ing-dsantiagog/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
</p>

## The Rakvor DFIR suite

Start with **[RV Hub](https://github.com/Panacota96/rv-hub)**: the one window an examiner opens first. It finds the
installed tools, checks their signatures, launches them on a case folder, shows the case at a glance and verifies the
whole case. The other tools stay separate, separately signed programs.

| Tool | What it does | Latest |
| --- | --- | --- |
| [**RV Hub**](https://github.com/Panacota96/rv-hub) | Front door: finds and verifies the tools, launches them on a case, verifies the whole case. | [![](https://img.shields.io/github/v/release/Panacota96/rv-hub?label=)](https://github.com/Panacota96/rv-hub/releases/latest) |
| [**RV Triage**](https://github.com/Panacota96/rv-triage) | Live Windows triage from a USB stick: volatile data, event logs, hives, prefetch, browsers, tasks, into a hashed, logged package. | [![](https://img.shields.io/github/v/release/Panacota96/rv-triage?label=)](https://github.com/Panacota96/rv-triage/releases/latest) |
| [**RV HashInv**](https://github.com/Panacota96/rv-hashinv) | Evidence inventory: hashes every file, detects its real type, flags anomalies, registers the evidence of a case. | [![](https://img.shields.io/github/v/release/Panacota96/rv-hashinv?label=)](https://github.com/Panacota96/rv-hashinv/releases/latest) |
| [**RV PDFAuth**](https://github.com/Panacota96/rv-pdfauth) | Signals of modification in PDFs: every saved revision extracted and compared visually, plus metadata, fonts, signatures and hidden content. | [![](https://img.shields.io/github/v/release/Panacota96/rv-pdfauth?label=)](https://github.com/Panacota96/rv-pdfauth/releases/latest) |
| [**RV ImgAuth**](https://github.com/Panacota96/rv-imgauth) | Signals of modification in photos and screenshots (JPEG, HEIC, PNG, WebP): structure, metadata, double compression, ELA/noise maps, copy-move. | [![](https://img.shields.io/github/v/release/Panacota96/rv-imgauth?label=)](https://github.com/Panacota96/rv-imgauth/releases/latest) |
| [**RV AvAuth**](https://github.com/Panacota96/rv-avauth) | Audio and video authenticity signals: container structure (MP4/MOV, Ogg/Opus, WAV, MP3) and encoder traces. | [![](https://img.shields.io/github/v/release/Panacota96/rv-avauth?label=)](https://github.com/Panacota96/rv-avauth/releases/latest) |
| [**RV MailAuth**](https://github.com/Panacota96/rv-mailauth) | Email authenticity signals in .eml, .msg and .mbox: DKIM/ARC re-verified offline, Received path, dates, attachments, BEC signals. | [![](https://img.shields.io/github/v/release/Panacota96/rv-mailauth?label=)](https://github.com/Panacota96/rv-mailauth/releases/latest) |
| [**RV RSMF**](https://github.com/Panacota96/rv-rsmf) | Converts WhatsApp, Telegram, Teams and mobile-tool CSV chat exports to validated RSMF 2.0 for Relativity, each message traced to its source line. | [![](https://img.shields.io/github/v/release/Panacota96/rv-rsmf?label=)](https://github.com/Panacota96/rv-rsmf/releases/latest) |
| [**RV CertCheck**](https://github.com/Panacota96/rv-certcheck) | Validates X.509 chains, revocation, RFC 3161 tokens and trust lists found in evidence; also creates Rakvor's own PKI and lab certificates. | [![](https://img.shields.io/github/v/release/Panacota96/rv-certcheck?label=)](https://github.com/Panacota96/rv-certcheck/releases/latest) |
| [**RV Timeline**](https://github.com/Panacota96/rv-timeline) | One cited super-timeline of a case, built from the verified runs of the other tools, with cross-source time signals. | [![](https://img.shields.io/github/v/release/Panacota96/rv-timeline?label=)](https://github.com/Panacota96/rv-timeline/releases/latest) |
| [**RV Report**](https://github.com/Panacota96/rv-report) | Assembles one expert report (dictamen pericial / rapport d'expertise) from the verified runs, quoting each tool verbatim; never writes a conclusion. | [![](https://img.shields.io/github/v/release/Panacota96/rv-report?label=)](https://github.com/Panacota96/rv-report/releases/latest) |

```mermaid
flowchart LR
    T["RV Triage<br/>collect"] --> H["RV HashInv<br/>register evidence"]
    H --> A["PDFAuth · ImgAuth · AvAuth<br/>MailAuth · RSMF · CertCheck"]
    A --> TL["RV Timeline"]
    A --> R["RV Report"]
    TL --> R
    HUB(["RV Hub<br/>launch · dashboard · verify case"]) -.-> H & A & TL & R
```

## How they are built

- **Rust**, Windows 10/11, a command line and a desktop app for every tool.
- **Signed releases**: Authenticode signatures chaining to the Rakvor root, `SHA256SUMS` and build provenance on every release; RV Hub checks the chain before it launches a tool.
- **Tamper-evident audit logs**: every action is written to a hash-chained log that anyone can re-verify (`verify-log`), including the outputs it recorded.
- **RFC 3161 timestamps** on the audit logs, with the TSA signature checked on verification.
- **Signals, not verdicts**: no tool ever says "authentic" or "forged"; every finding states what it shows *and what it does not prove*.
- **Three languages**: interface and reports in English, Spanish and French, with Colombian and French report structures.
- **Independent QA harness**: the signed release executables are re-tested from outside the repositories, per tool and across the whole case workflow.
- **Source-available, non-commercial**: the code is published for audit under the PolyForm Noncommercial 1.0.0 licence.

### rakvor-tool-forge

[**rakvor-tool-forge**](https://github.com/Panacota96/rakvor-tool-forge) is the skill that turns "we need a tool that
does X" into a Rakvor tool that builds, passes its tests and meets the forensic contract from the first commit: a
phased procedure, reference templates (Rust and Python) and a contract validator that every tool must pass.

## Services

Through Rakvor I work with small and medium-sized businesses in **Colombia** and **France**:

- **Digital forensics**: evidence collection, document, image, email and chat authenticity, expert reports.
- **Pentesting**: authorized assessments of web applications, networks and infrastructure.
- **SOC**: monitoring, detection and incident response sized for SMEs.

## About me

**Roles:** Cybersecurity Analyst · eDiscovery Analyst · Digital Forensics Engineer

**Education**

- Master's in Cybersecurity, ESME, Paris
- Bachelor's in Electronics, Pontificia Universidad Javeriana, Bogotá

**Languages:** English · Spanish · French

### Other projects

- [EnGarde](https://github.com/Panacota96/master-Project-Phishing): serverless phishing-awareness platform for engineering students.
- [Guild-Scroll](https://github.com/Panacota96/Guild-Scroll): terminal flight recorder for CTFs and authorized pentests with structured reporting.
- [AI Cyber Lab](https://github.com/Panacota96/ai-cyber-lab): desktop-first cyber-lab workspace for CTF, pentest and AI-assisted reporting.
