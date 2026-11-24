<p align="center">
  <img src="./assets/profile-header.svg" alt="David Santiago Gonzalez Rico - Rakvor DFIR tools" width="100%" />
</p>

<h1 align="center">David Santiago Gonzalez Rico</h1>

<p align="center"><strong>Digital forensics · Pentesting · SOC — for SMEs in Colombia and France</strong></p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3000&pause=800&color=1A936F&center=true&vCenter=true&width=560&lines=Digital+Forensics+Engineer;eDiscovery+Analyst;Cybersecurity+Analyst;Building+Rakvor+DFIR+tools+in+Rust" alt="Digital Forensics Engineer · eDiscovery Analyst · Cybersecurity Analyst · Building Rakvor DFIR tools in Rust" />
</p>

<p align="center">
  I build <strong>Rakvor</strong>, a suite of digital-forensics tools written in Rust for examiners who have to
  defend their findings in court. Every tool reports <em>signals, not verdicts</em>, and keeps a tamper-evident record of
  everything it did.
</p>

<p align="center">
  <a href="https://github.com/Panacota96/rv-hub/releases/latest"><img src="https://img.shields.io/github/v/release/Panacota96/rv-hub?label=RV%20Hub&style=for-the-badge&color=1A936F" alt="RV Hub latest release" /></a>
  <a href="https://www.linkedin.com/in/ing-dsantiagog/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://buymeacoffee.com/santiagogow"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-santiagogow-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=000000" alt="Buy Me a Coffee" /></a>
</p>

<p align="center">
  <a href="https://github.com/Panacota96/rv-hub"><img src="https://img.shields.io/badge/RV%20Hub-Front%20door-1A936F?style=flat-square&logo=github&logoColor=white" alt="RV Hub" /></a>
  <a href="https://github.com/Panacota96/rv-pdfauth"><img src="https://img.shields.io/badge/RV%20PDFAuth-Documents-1A936F?style=flat-square&logo=github&logoColor=white" alt="RV PDFAuth" /></a>
  <a href="https://github.com/Panacota96/rv-mailauth"><img src="https://img.shields.io/badge/RV%20MailAuth-Email-1A936F?style=flat-square&logo=github&logoColor=white" alt="RV MailAuth" /></a>
  <a href="https://github.com/Panacota96/rv-report"><img src="https://img.shields.io/badge/RV%20Report-Expert%20reports-1A936F?style=flat-square&logo=github&logoColor=white" alt="RV Report" /></a>
  <a href="https://github.com/Panacota96/rakvor-tool-forge"><img src="https://img.shields.io/badge/Tool%20Forge-Skill-1B6CA8?style=flat-square&logo=github&logoColor=white" alt="rakvor-tool-forge" /></a>
</p>

## The Rakvor DFIR suite

<p align="center">
  <a href="https://github.com/Panacota96/rv-hub"><img src="https://raw.githubusercontent.com/Panacota96/rv-hub/main/assets/brand/rv-mark.png" width="88" alt="Rakvor RV logo" /></a>
</p>

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

### See them working

All screenshots show synthetic sample evidence shipped with each tool.

<table>
  <tr>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-hub"><img src="https://raw.githubusercontent.com/Panacota96/rv-hub/main/docs/images/hub-tools.png" alt="RV Hub: installed tools with their signature status" /></a>
      <br /><sub><b>RV Hub</b> · installed tools, signature checked</sub>
    </td>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-pdfauth"><img src="https://raw.githubusercontent.com/Panacota96/rv-pdfauth/main/docs/images/gui-revision-viewer.png" alt="RV PDFAuth: revision 1 vs 2 of a synthetic invoice" /></a>
      <br /><sub><b>RV PDFAuth</b> · revision viewer, changed amount highlighted</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-imgauth"><img src="https://raw.githubusercontent.com/Panacota96/rv-imgauth/main/docs/img/viewer.png" alt="RV ImgAuth: copy-move overlay on a synthetic photo" /></a>
      <br /><sub><b>RV ImgAuth</b> · copy-move overlay</sub>
    </td>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-mailauth"><img src="https://raw.githubusercontent.com/Panacota96/rv-mailauth/main/docs/images/gui-message.png" alt="RV MailAuth: message view" /></a>
      <br /><sub><b>RV MailAuth</b> · message signals</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-timeline"><img src="https://raw.githubusercontent.com/Panacota96/rv-timeline/main/docs/images/gui-timeline.png" alt="RV Timeline: case super-timeline" /></a>
      <br /><sub><b>RV Timeline</b> · case super-timeline</sub>
    </td>
    <td width="50%" align="center">
      <a href="https://github.com/Panacota96/rv-report"><img src="https://raw.githubusercontent.com/Panacota96/rv-report/main/docs/images/gui-main.png" alt="RV Report: expert report with section preview" /></a>
      <br /><sub><b>RV Report</b> · expert report preview</sub>
    </td>
  </tr>
</table>

## How they are built

- **Rust**, Windows 10/11, a command line and a desktop app for every tool.
- **Signed releases**: Authenticode signatures chaining to the Rakvor root, `SHA256SUMS` and build provenance on every release; RV Hub checks the chain before it launches a tool.
- **Tamper-evident audit logs**: every action is written to a hash-chained log that anyone can re-verify (`verify-log`), including the outputs it recorded.
- **RFC 3161 timestamps** on the audit logs, with the TSA signature checked on verification.
- **Signals, not verdicts**: no tool ever says "authentic" or "forged"; every finding states what it shows *and what it does not prove*.
- **Three languages**: interface and reports in English, Spanish and French, with Colombian and French report structures.
- **Independent QA harness**: the signed release executables are re-tested from outside the repositories, per tool and across the whole case workflow.
- **Source-available, non-commercial**: the code is published for audit under the PolyForm Noncommercial 1.0.0 licence.

```mermaid
flowchart LR
    E[/"Evidence"/] --> RUN["Tool run<br/>read-only, isolated worker"]
    RUN --> LOG[("Audit log<br/>each entry hashes the previous one")]
    LOG --> TSA["RFC 3161 timestamp<br/>TSA-signed"]
    RUN --> OUT[["Reports<br/>shows / does not prove"]]
    OUT -. "SHA-256 recorded" .-> LOG
    TSA --> V{"verify-log<br/>anyone can re-check"}
    LOG --> V
```

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

### Education

<p>
  <img src="https://img.shields.io/badge/ESME%20Paris-Master's%20in%20Cybersecurity%20%F0%9F%87%AB%F0%9F%87%B7-0E8B57?style=for-the-badge" alt="ESME Paris, Master's in Cybersecurity" />
  <img src="https://img.shields.io/badge/Pontificia%20Universidad%20Javeriana-Bachelor's%20in%20Electronics%20%F0%9F%87%A8%F0%9F%87%B4-0F4C81?style=for-the-badge" alt="Pontificia Universidad Javeriana, Bachelor's in Electronics" />
</p>

### Spoken languages

<p>
  <img src="https://img.shields.io/badge/English-%F0%9F%87%AC%F0%9F%87%A7-1F6FEB?style=for-the-badge" alt="English" />
  <img src="https://img.shields.io/badge/Spanish-%F0%9F%87%A8%F0%9F%87%B4-CE1126?style=for-the-badge" alt="Spanish" />
  <img src="https://img.shields.io/badge/French-%F0%9F%87%AB%F0%9F%87%B7-0055A4?style=for-the-badge" alt="French" />
</p>

## Toolkit

<p align="center">
  <img src="https://skillicons.dev/icons?i=rust,py,js,ts,bash,sqlite,aws,docker,kubernetes,terraform,githubactions,linux,ubuntu,debian,kali,windows,wireshark&perline=9" alt="Rust, Python, JavaScript, TypeScript, Bash, SQLite, AWS, Docker, Kubernetes, Terraform, GitHub Actions, Linux, Ubuntu, Debian, Kali, Windows, Wireshark" />
</p>

### Digital forensics and mobile

<p>
  <img src="https://img.shields.io/badge/X--Ways%20Forensics-Disk%20analysis-8B1E3F?style=for-the-badge" alt="X-Ways Forensics" />
  <img src="https://img.shields.io/badge/Magnet%20AXIOM-Forensics-1E3A8A?style=for-the-badge" alt="Magnet AXIOM" />
  <img src="https://img.shields.io/badge/Autopsy-Forensics-374151?style=for-the-badge" alt="Autopsy" />
  <img src="https://img.shields.io/badge/FTK%20Imager-Imaging-4B5563?style=for-the-badge" alt="FTK Imager" />
  <img src="https://img.shields.io/badge/Tableau-Forensic%20imaging-4B5563?style=for-the-badge" alt="Tableau forensic hardware" />
  <img src="https://img.shields.io/badge/Volatility-Memory%20forensics-0E7C5A?style=for-the-badge" alt="Volatility" />
  <img src="https://img.shields.io/badge/Cellebrite-Mobile-0B6E4F?style=for-the-badge" alt="Cellebrite" />
  <img src="https://img.shields.io/badge/XRY-Mobile%20extraction-0B6E4F?style=for-the-badge" alt="MSAB XRY" />
  <img src="https://img.shields.io/badge/XAMN-Mobile%20analysis-0B6E4F?style=for-the-badge" alt="MSAB XAMN" />
</p>

### eDiscovery

<p>
  <img src="https://img.shields.io/badge/Relativity%20%2F%20RelativityOne-eDiscovery-1F3A5F?style=for-the-badge" alt="Relativity and RelativityOne" />
  <img src="https://img.shields.io/badge/Nuix-eDiscovery-1F3A5F?style=for-the-badge" alt="Nuix" />
  <img src="https://img.shields.io/badge/Reveal-eDiscovery-1F3A5F?style=for-the-badge" alt="Reveal" />
</p>

### SOC, SIEM and EDR

<p>
  <img src="https://img.shields.io/badge/Splunk-SIEM-000000?style=for-the-badge&logo=splunk&logoColor=white" alt="Splunk" />
  <img src="https://img.shields.io/badge/Microsoft%20Sentinel-SIEM-0078D4?style=for-the-badge" alt="Microsoft Sentinel" />
  <img src="https://img.shields.io/badge/Wazuh-SIEM%20%2F%20XDR-1E6FD9?style=for-the-badge" alt="Wazuh" />
  <img src="https://img.shields.io/badge/CrowdStrike-EDR-E01F26?style=for-the-badge" alt="CrowdStrike" />
  <img src="https://img.shields.io/badge/Trellix-EDR-C8102E?style=for-the-badge" alt="Trellix" />
  <img src="https://img.shields.io/badge/Wireshark-Traffic-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark" />
</p>

### Pentesting

<p>
  <img src="https://img.shields.io/badge/Nmap-Recon-4682B4?style=for-the-badge" alt="Nmap" />
  <img src="https://img.shields.io/badge/Metasploit-Exploitation-2596CD?style=for-the-badge" alt="Metasploit" />
  <img src="https://img.shields.io/badge/BloodHound-Active%20Directory-A31F34?style=for-the-badge" alt="BloodHound" />
  <img src="https://img.shields.io/badge/Burp%20Suite-Web%20testing-F47F24?style=for-the-badge&logo=burpsuite&logoColor=white" alt="Burp Suite" />
  <img src="https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali Linux" />
  <img src="https://img.shields.io/badge/Exegol-1F2937?style=for-the-badge" alt="Exegol" />
</p>

### Programming languages

<p>
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/SQL%20%2F%20SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQL and SQLite" />
  <img src="https://img.shields.io/badge/Bash-121011?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Terraform-0B6E4F?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/YAML-CB171E?style=for-the-badge&logo=yaml&logoColor=white" alt="YAML" />
</p>

### Cloud: AWS

<p>
  <img src="https://img.shields.io/badge/AWS-Cloud-232F3E?style=for-the-badge" alt="AWS" />
  <img src="https://img.shields.io/badge/Lambda-Serverless-FF9900?style=for-the-badge" alt="AWS Lambda" />
  <img src="https://img.shields.io/badge/API%20Gateway-HTTP%20APIs-2EA043?style=for-the-badge" alt="Amazon API Gateway" />
  <img src="https://img.shields.io/badge/CloudFront-CDN-238636?style=for-the-badge" alt="Amazon CloudFront" />
  <img src="https://img.shields.io/badge/DynamoDB-NoSQL-4053D6?style=for-the-badge" alt="Amazon DynamoDB" />
  <img src="https://img.shields.io/badge/S3-Storage-569A31?style=for-the-badge" alt="Amazon S3" />
  <img src="https://img.shields.io/badge/SQS-Queues-FF4F8B?style=for-the-badge" alt="Amazon SQS" />
  <img src="https://img.shields.io/badge/SES-Email-DD344C?style=for-the-badge" alt="Amazon SES" />
  <img src="https://img.shields.io/badge/EventBridge-Scheduling-FF4F8B?style=for-the-badge" alt="Amazon EventBridge" />
  <img src="https://img.shields.io/badge/ElastiCache-Redis-3FB950?style=for-the-badge" alt="Amazon ElastiCache" />
  <img src="https://img.shields.io/badge/CloudWatch-Monitoring-E7157B?style=for-the-badge" alt="Amazon CloudWatch" />
  <img src="https://img.shields.io/badge/IAM-Access-DD344C?style=for-the-badge" alt="AWS IAM" />
  <img src="https://img.shields.io/badge/EC2-Compute-FF9900?style=for-the-badge" alt="Amazon EC2" />
  <img src="https://img.shields.io/badge/Terraform-IaC-0B6E4F?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
</p>

[EnGarde](https://github.com/Panacota96/master-Project-Phishing), my phishing-awareness platform, runs serverless on AWS and is deployed with Terraform:

```mermaid
flowchart LR
    U(["Students and instructors"]) --> CF["CloudFront"]
    CF --> APIGW["API Gateway v2"]
    APIGW --> APP["Lambda<br/>Flask app"]
    APP --> DDB[("DynamoDB<br/>9 tables")]
    APP --> S3[("S3<br/>emails · reports")]
    APP --> Q["SQS"]
    EB["EventBridge<br/>schedules"] -.-> Q
    Q --> W["Lambda workers<br/>campaign mailer · registration"]
    W --> SES["SES<br/>email"]
    W --> DDB
```

<details>
  <summary><strong>Operating systems and lab environments</strong></summary>

  <br />

  **Operating systems**

  <p>
    <img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" />
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
    <img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu" />
    <img src="https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white" alt="Debian" />
    <img src="https://img.shields.io/badge/Parrot%20OS-15AABF?style=for-the-badge" alt="Parrot OS" />
  </p>

  **Lab and virtualized environments**

  <p>
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
    <img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Compose" />
    <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
  </p>

</details>

### Other projects

- [EnGarde](https://github.com/Panacota96/master-Project-Phishing): serverless phishing-awareness platform for engineering students.
- [Guild-Scroll](https://github.com/Panacota96/Guild-Scroll): terminal flight recorder for CTFs and authorized pentests with structured reporting.
- [AI Cyber Lab](https://github.com/Panacota96/ai-cyber-lab): desktop-first cyber-lab workspace for CTF, pentest and AI-assisted reporting.
