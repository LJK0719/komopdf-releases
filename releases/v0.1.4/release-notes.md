# komopdf 0.1.4

This release provides a **Windows x64 installer**. New macOS packages are not included; no unverified architecture is advertised.

## Editing and reading

- Edit rich paragraphs with mixed formatting, first-line indentation, spacing, and automatic continuation while preserving unrelated page content.
- Navigate search matches, choose case-sensitive or whole-word matching, fit the page to the available width, and enter a zoom percentage without losing your reading position.
- Add notes, rectangles, and freehand annotations directly on a page; filter and navigate annotations across the document.
- Draw a signature once and place it repeatedly with a movable, resizable preview and an explicit confirmation step.
- Import selected PDF pages at a chosen position and add page numbers with a starting value, cover-page exclusion, templates, and footer alignment.

## Desktop workflows

- Separate Save and Save As: the first save chooses a destination, subsequent saves reuse it, and cancelling does not mark the document as saved.
- Print all pages, the current page, or a selected range, with a copy count and an explicit default-printer notice.
- Export the currently edited document locally, including DOCX. Complex layouts, substituted fonts, and scanned documents may require manual review or OCR.
- Improve komo review visibility and preserve read-only navigation while approval is pending. Web question answering respects the PDF's copy permission.

## Correctness fixes

- Partial page extraction/import/copy no longer retains the unselected text from a continued paragraph's internal metadata.
- Deleting part of a continued paragraph leaves independent editable fragments instead of restoring deleted text later.
- Mixed-style edits continue to target the correct paragraph after it moves to a new page.
- Browser page and export-memory limits are enforced before changing the document or assembling oversized output.
- Include the local conversion entry script in the packaged product runtime.

## Requirements and limits

- Windows x64; minimum supported target: Windows 10 22H2. This release was locally installed and exercised on Windows 11 x64.
- The installer includes the product runtime and an offline WebView2 installer. PDF editing, OCR, and conversion run locally; AI requests require network access and the appropriate sharing permission.
- A handwritten signature is an Ink annotation, not a certificate-backed digital signature.
- Partial operations on continued paragraphs can produce independent editable fragments. These fixes are not a general secure-redaction facility.
- Physical printer output, clean-machine Windows 10 installation, macOS, and page-by-page comparison in Microsoft Word were not part of this release's local verification.
- Retain copies of important documents and review exported layouts before distribution.

Shared open-source core: https://github.com/LJK0719/komopdf/commit/dadc84738922bba610fdcba85fd20ac06ecb5ed3

Download only the fixed-version assets from this release and compare their SHA-256 values with `SHA256SUMS`. The separately listed third-party notices retain the components' respective licensing terms.
