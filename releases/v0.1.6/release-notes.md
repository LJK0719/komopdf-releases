# komopdf 0.1.6

Windows x64 update. PDF editing remains free and does not require an account.

## Improvements

- Browser sign-in returns to the desktop automatically. Failed and cancelled sign-ins now have clear, consistent feedback.
- Account, connected-service and subscription settings reflect the correct state, including offline sign-out and overdue-payment actions.
- Opening an assistant's PDF attachment keeps the conversation and its output folder. Conversation history preserves task attachments and can be reopened.
- Account changes and late attachment actions cannot reuse another task's history.
- Billing returns to the desktop without exposing a long-lived session token or confusing a different browser account.
- Tool inputs are fully included in credit reservations; only actual validated image attachments exclude base64 payloads.

1 credit equals 10,000 tokens. New accounts receive 1,000 welcome credits. KOMO Plus is $4.99/month for unlimited conversations; KolmoPDF parsing is billed separately.

## Download and compatibility

This release contains the Windows x64 installer, checksums, release manifest and third-party notices. Windows 10 22H2 or later, 64-bit, is required. The installer includes the local PDF, OCR, font and material-processing runtimes. AI requests need an internet connection.

No macOS installer is included in this release. Previous release assets remain unchanged. GitHub's automatic source archives contain this public distribution repository, not the private desktop source or an installer.
