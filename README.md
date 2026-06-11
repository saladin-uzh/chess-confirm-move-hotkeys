# Chess.com Confirm Move Hotkeys

[Українська версія](README.uk.md)

A minimal Manifest V3 extension for Chrome and Chromium-based browsers that
controls the Chess.com move confirmation dialog with keyboard shortcuts.

## Install locally

This extension is not distributed through the Chrome Web Store. Install it as
an unpacked extension from a local copy of this repository.

### 1. Get the extension files

Choose one option:

- Clone the repository:

  ```bash
  git clone https://github.com/saladin-uzh/chess-confirm-move-hotkeys.git
  ```

- Or select **Code → Download ZIP** on GitHub and extract the downloaded
  archive. Do not load the ZIP file directly.

### 2. Load the unpacked extension

1. Open `chrome://extensions` in Chrome or a Chromium-based browser.
2. Enable **Developer mode**.
3. Select **Load unpacked**.
4. Select the extracted `chess-confirm-move-hotkeys` directory containing
   `manifest.json`.
5. Reload any Chess.com tabs that were already open.

After pulling or downloading an update, select the extension's **Reload**
button on `chrome://extensions`, then reload the Chess.com tab.

## Shortcuts

- `Space` confirms the move.
- `Escape` cancels the move.

The extension handles a shortcut only when the corresponding visible and
enabled confirmation or cancellation button is present. It ignores key events
inside form controls, text fields, editable elements, and shortcuts combined
with modifier keys.

## Supported pages

The content script runs only on:

- `https://www.chess.com/play/*`
- `https://www.chess.com/game/*`
- `https://www.chess.com/analysis/game/*`

## Troubleshooting

- Reload the Chess.com tab after installing or updating the extension.
- Verify that move confirmation is enabled in your Chess.com settings.
- Open the page console and look for
  `[Chess.com Confirm Move Hotkeys] Initialized.`
- Confirm that the current page URL matches one of the supported patterns.

## Security and privacy

The extension requests no additional permissions, makes no external network
requests, and does not collect or transmit data. It runs only on the listed
Chess.com URLs.
