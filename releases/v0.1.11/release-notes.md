# komopdf 0.1.11

## More reliable editing

- Double-click text to place a blinking caret at the clicked position. Original bold and italic styles remain intact when typing begins.
- Changing bold or italic at an insertion point now affects new text without selecting or replacing the whole paragraph.
- Pressing Enter in text-format controls confirms the setting without inserting a line break into the document.
- Local formatting and continued typing preserve unchanged text and its original fonts.
- Save and Ctrl+S finish a pending note before saving. Applying form properties no longer discards an unfinished field value, and applying a value preserves unfinished property edits.

## More consistent navigation and workspace behavior

- Fixed the workspace's original-file association after saving a PDF under another name.
- Refreshing the workspace reloads the current text preview and refreshes previously collapsed folders when expanded.
- Facing-page keyboard navigation now reaches an odd-numbered final page.
- Keyboard resizing respects the selected side handle, matching mouse behavior.
- Dragging an object on another visible page works on the first gesture.

Page-level incremental refresh, source-font preservation, undo/redo, account features and conversation history remain available.

## Download

This release provides the Windows x64 installer for Windows 10 22H2 or later. macOS packages are not included in this release.

Use the fixed-version installer and compare its SHA-256 with `SHA256SUMS`. The installer includes the local PDF engine, fonts and offline tools. Existing user files, settings and history are preserved during upgrade.
