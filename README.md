# komopdf Desktop Releases

Official distribution repository for **komopdf**, the local-first PDF editor for Windows and macOS, with the **komo** AI assistant.

- Website and download page: [komopdf.com/download](https://komopdf.com/download/)
- Available installers: [GitHub Releases](https://github.com/LJK0719/komopdf-releases/releases)
- Open-source web editor and shared PDF engine: [LJK0719/komopdf](https://github.com/LJK0719/komopdf)

The release list can be empty while verification is in progress. This repository does not turn development executables into production installers. The website will only show download links for published packages.

## Supported release targets

| Target | Installer |
|---|---|
| Windows x64 | `komopdf-VERSION-windows-x64-setup.exe` |
| macOS Apple Silicon | `komopdf-VERSION-macos-arm64.dmg` |
| macOS Intel | `komopdf-VERSION-macos-x64.dmg` |

macOS architectures have separate packages; an arm64 package is not a universal or Intel binary. See each release for its tested minimum OS and requirements.

Each release includes its verified installers, `stable.json`, `SHA256SUMS`, release notes and `THIRD_PARTY_NOTICES.txt`. Version 0.1.15 provides Windows x64 and macOS Apple Silicon (arm64, macOS 13.0+). The Mac package uses ad-hoc signing and is not Apple-notarized; verify its SHA-256 before opening. Intel macOS is not included. Version 0.1.15 translates a complete selection in one request and one result, removes redundant blank lines, and fixes finding and replacing words split across PDF text objects or font styles. Desktop search offers full-document OCR for scanned pages and resumes the query afterward. Link annotations no longer prevent comments from loading; comment errors stay in the relevant panel with a retry action. Notes, drawing and form placement use direct page interaction rather than coordinate entry. Target-language preferences, comment editing, undo and saved PDF content remain supported. Translation results do not automatically replace PDF text or occupy the KOMO conversation sidebar. Download only architectures actually listed in a release, using its fixed-version assets; do not substitute a guessed URL or a third-party wrapper.

## Verify a download

Windows PowerShell:

```powershell
Get-FileHash .\komopdf-VERSION-windows-x64-setup.exe -Algorithm SHA256
```

macOS:

```sh
shasum -a 256 komopdf-VERSION-macos-arm64.dmg
```

Compare the exact hash against `SHA256SUMS` and the website. Do not bypass operating-system security warnings to run an unexpected or unverifiable download.

## Source and licensing

The web editor and shared engine are open source under Apache-2.0. Desktop-specific host, Agent integration and packaging source are private. Public access to an installer is not an open-source license for the private desktop code.

The license in this repository covers its original documentation and metadata only. Installers retain their applicable application and third-party notices. GitHub's automatic **Source code (zip/tar.gz)** downloads contain this repository's public release documentation, **not the private desktop source or an installer**.

## Feedback and security

Use an issue for reproducible desktop bugs or feature requests. Provide the version, OS/architecture and steps; use synthetic or redacted samples, never confidential PDFs, credentials or private workspace files. Web-source issues belong in the [web repository](https://github.com/LJK0719/komopdf/issues).

For security vulnerabilities, use the [private reporting form](https://github.com/LJK0719/komopdf/security/advisories/new), not a public issue.
