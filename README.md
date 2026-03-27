<div align="center">

# ☠️ BUG BOUNTY RECON TOOLKIT

**Your Elite Arsenal for Authorized Security Research & Bug Bounty Hunting**

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-recon--toolkit.netlify.app-00FF41?style=for-the-badge&logoColor=white)](https://recon-toolkit.netlify.app/)
[![GitHub](https://img.shields.io/badge/GitHub-rohit--1006-181717?style=for-the-badge&logo=github)](https://github.com/rohit-1006)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-00FF41?style=for-the-badge)]()
[![Tools](https://img.shields.io/badge/Tools-80%2B-red?style=for-the-badge)]()
[![Commands](https://img.shields.io/badge/Commands-250%2B-orange?style=for-the-badge)]()

</div>

---

## ⚠️ LEGAL DISCLAIMER

> **This toolkit is strictly for authorized security testing and educational purposes only.**
> Using these tools against systems without explicit written permission is illegal and unethical.
> The author assumes NO liability for any misuse. Always obtain proper authorization before testing.

---

## 🔍 Overview

The **Bug Bounty Recon Toolkit** is a comprehensive, browser-based platform that aggregates **80+ industry-standard security tools** with **250+ ready-to-use commands** across **25+ vulnerability categories**. Designed for penetration testers, bug bounty hunters, and security researchers, this toolkit streamlines the reconnaissance phase by generating customized, exploit-ready commands in real-time simply by entering a target domain.

No installation required — everything runs directly in your browser.

```bash
[ root@phano ]$ ./init_recon.sh --target <DOMAIN>
# Generating 250+ exploit-ready commands...
```

---

## 🌐 Live Demo

🔗 **[https://recon-toolkit.netlify.app/](https://recon-toolkit.netlify.app/)**

Simply enter a target domain (that you own or have written permission to test) and instantly get a full suite of tailored reconnaissance commands.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| 🎯 **Target-Aware Commands** | Enter any domain and get 250+ commands auto-populated with your target |
| 🛠️ **80+ Security Tools** | Covers the full recon-to-exploitation pipeline |
| 📂 **25+ Categories** | Organized by vulnerability type for rapid workflow |
| 📋 **One-Click Copy** | Copy individual commands or entire categories instantly |
| 💀 **Hacker Terminal UI** | Immersive, CLI-inspired interface themed after Kali Linux |
| ⚡ **Zero Installation** | 100% browser-based — no setup, no dependencies |
| 📱 **Responsive Design** | Works on desktop and mobile devices |
| 🔄 **Expand/Collapse** | Cleanly organized sections to reduce clutter |

---

## 🗂️ Tool Categories

The toolkit covers the following reconnaissance and exploitation categories:

```
┌─────────────────────────────────────────────────────────────────┐
│  RECON & OSINT           │  WEB APPLICATION TESTING             │
│  ──────────────          │  ───────────────────────             │
│  • Subdomain Enumeration │  • XSS (Cross-Site Scripting)        │
│  • DNS Reconnaissance    │  • SQL Injection                     │
│  • Port Scanning         │  • SSRF Detection                    │
│  • WHOIS Lookup          │  • IDOR Testing                      │
│  • Certificate Recon     │  • LFI / RFI                         │
│  • ASN / IP Enumeration  │  • Open Redirect                     │
│                          │  • CRLF Injection                    │
│  INFRASTRUCTURE          │                                      │
│  ──────────────          │  ADVANCED                            │
│  • Technology Detection  │  ───────────────────                 │
│  • Cloud Bucket Discovery│  • Fuzzing & Brute Force             │
│  • Firewall Detection    │  • API Security Testing              │
│  • Directory Brute Force │  • JWT Attacks                       │
│  • Virtual Host Discovery│  • Authentication Bypass             │
│  • Parameter Discovery   │  • Business Logic Flaws              │
└─────────────────────────────────────────────────────────────────┘
```

**Tools included (partial list):**
`nmap` • `amass` • `subfinder` • `httpx` • `nuclei` • `ffuf` • `gobuster` • `sqlmap` • `dalfox` • `gau` • `waybackurls` • `shodan` • `censys` • `dirsearch` • `wfuzz` • `nikto` • `burpsuite` • `metasploit` • `wireshark` • `masscan` and many more...

---

## 📸 Screenshots

> *Terminal-style interface — enter your target domain and watch commands come alive.*

```
┌──(root💀kali)-[~/targets]
└─$ set-target

  TARGET ~> example.com          [EXECUTE]

  ╔═══════════════════════════════════════════════╗
  ║  80+ TOOLS │ 250+ COMMANDS │ 25+ CATEGORIES   ║
  ╚═══════════════════════════════════════════════╝

  [SUBDOMAIN ENUMERATION]
  amass enum -passive -d example.com
  subfinder -d example.com -o subdomains.txt
  ...
```

---

## 🎯 Usage

1. **Open** the toolkit in your browser
2. **Enter** your authorized target domain in the input field
3. **Click** `EXECUTE` to generate all commands
4. **Browse** through 25+ categories of tools and techniques
5. **Copy** individual commands or entire sections with one click
6. **Run** the commands in your terminal on your authorized target

```bash
# Example: After entering "example.com" as target
# The toolkit generates commands like:

amass enum -passive -d example.com
subfinder -d example.com -all -recursive
nmap -sV -sC -p- example.com
ffuf -u https://example.com/FUZZ -w /usr/share/wordlists/dirb/common.txt
sqlmap -u "https://example.com/page?id=1" --dbs
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) | Structure & Markup |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) | Styling & Terminal Theme |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | Command Generation & DOM Manipulation |
| ![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white) | Hosting & Deployment |

- Pure **Vanilla JS** — zero frameworks, zero dependencies
- Custom **CLI-inspired CSS** theming with Kali Linux aesthetic
- Fully **client-side** — no backend, no data collection

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a new branch: `git checkout -b feature/new-tool-category`
3. **Add** new tools, commands, or fix bugs
4. **Commit** your changes: `git commit -m "Add: New SSRF detection commands"`
5. **Push** to your branch: `git push origin feature/new-tool-category`
6. **Open** a Pull Request

### What to contribute:
- 🆕 New tool categories or commands
- 🐛 Bug fixes
- 🎨 UI/UX improvements
- 📖 Documentation updates
- 🌍 Translations

Please ensure all contributed commands are ethical, legal, and intended for authorized testing only.

---

## 👤 Author

<div align="center">

**Rohit** — Security Researcher · Penetration Tester · Bug Bounty Hunter

[![GitHub](https://img.shields.io/badge/GitHub-rohit--1006-181717?style=for-the-badge&logo=github)](https://github.com/rohit-1006)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Rohit10-212C42?style=for-the-badge&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/Rohit10)


</div>

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## ⭐ Support

If this toolkit helped your bug bounty workflow, consider giving it a **⭐ Star** — it means a lot!

<div align="center">

**⚠️ Remember: Only use these tools on systems you have explicit written permission to test. ⚠️**

</div>
