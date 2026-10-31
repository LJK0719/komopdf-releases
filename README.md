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

Each release includes its verified installers, `stable.json`, `SHA256SUMS`, release notes and `THIRD_PARTY_NOTICES.txt`.

Version **0.1.17** provides Windows x64 and macOS Apple Silicon with save-and-continue for updated materials, clearer question recovery and export retries that preserve settings. Windows includes signed in-app updates; install manually once if upgrading from 0.1.15 or earlier. Updates require user approval and preserve open-document save prompts; uninstall preserves user documents and application data. The Windows installer has a Tauri update signature but is not Authenticode-signed.

The macOS **0.1.17** package is built natively for Apple Silicon and requires macOS 13.0 or later. It uses ad-hoc signing and is not Apple-notarized; install updates from the DMG. No Intel package is included. Download only architectures actually listed in a release and verify their fixed-version assets.

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
