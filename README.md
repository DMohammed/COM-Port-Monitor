# COM Port Monitor

A lightweight Windows utility that detects which application is holding a serial (COM) port. Built for developers, hardware engineers, and anyone who needs to quickly identify COM port conflicts.

![Screenshot](screenshot.png)

## Features

- **Auto-detects all COM ports** from Windows registry
- **Maps COM ports to NT device names** (e.g., `COM4` → `\Device\Serial15`)
- **Finds the owning process** using Sysinternals handle64.exe (embedded)
- **Dark mode UI** — easy on the eyes for long debugging sessions
- **Single-file executable** — no installation, no dependencies

## Use Case

You plug in a USB-to-Serial adapter, Windows assigns it `COM15`, but your app says "Access Denied."  
**COM Port Monitor** tells you exactly which process has it locked — in one click.

## Download

Get the latest release from the [Releases](../../releases) page.

## Requirements

- Windows 10/11 (64-bit)
- Administrator privileges (required for handle enumeration)

## How to Use

1. Download `COMPortMonitor.exe` from Releases
2. Run as Administrator
3. Click **Check All** or **Check** on any specific port
4. See which process owns it — instantly

## Built With

- C# / .NET 8
- Windows Forms (custom dark theme)
- Sysinternals handle64.exe (embedded)

## License

MIT License — free for personal and commercial use.
