# komopdf 0.1.16 — Windows and macOS

## A faster, more direct PDF workspace

- The website now opens directly into the PDF editor. Open or drop a PDF without a marketing page or sign-in step.
- A compact toolbar gives documents more space, with improved small-screen layouts and clear opening, editing and saving feedback.
- Reading selections keep their right-click actions when menu focus changes. Highlight, underline, edit and AI actions use the selected text, with menus appropriate to reading, object editing and hand-tool modes.
- Highlight comment buttons no longer cover the start of the marked text.
- Fix page extraction/insertion targeting after navigation, cancelled-export messages, and undo with pending form drafts. Field property panels retain their expanded state.
- Improve account retry/re-authentication, explicit account switching and connected-service state synchronization.

## Windows updates and uninstall

- Settings → About provides update checking, verified downloads and user-initiated installation. Updates do not interrupt editing or force a restart.
- Installation asks you to quit the editor instead of killing it. Uninstall keeps user documents, settings, workspace material and recovery data.
- Version 0.1.15 and earlier need this installer once to enable future in-app updates.

## Distribution notes

- This release contains Windows x64 and macOS Apple Silicon (arm64, macOS 13.0+) installers. No Intel macOS package is included.
- Update packages are protected by a Tauri updater signature. The Windows installer is not Authenticode-signed; Windows may display an unknown-publisher/SmartScreen prompt.
- The GitHub-generated source archives contain only this public release repository, not the private desktop implementation. Public editor source: https://github.com/LJK0719/komopdf

## macOS Apple Silicon

- Version 0.1.16 is built natively on an Apple Silicon Mac from the fixed desktop and shared-editor source revisions.
- Includes the refreshed editor, reliable context menus and account/service workflow improvements.
- The Mac app uses ad-hoc local signing and is not Apple-notarized. Mac updates in this release use the DMG installer; the in-app updater feed remains Windows-only.
