# Finalcat

Self-contained server binary for Finalcat. Distributed via [GitHub Releases](https://github.com/lich99/finalcat/releases).

## Install

```bash
# Auto-detect architecture and download
ARCH=$(uname -m | sed 's/x86_64/x64/' | sed 's/aarch64/arm64/')
curl -fSL -o ~/.local/bin/finalcat \
  https://github.com/lich99/finalcat/releases/latest/download/finalcat-linux-${ARCH}
chmod +x ~/.local/bin/finalcat
```

## Usage

```bash
finalcat start       # Start daemon
finalcat stop        # Stop daemon
finalcat status      # Check status
finalcat logs -f     # Follow logs
finalcat --version   # Print version
```

Server runs on `http://127.0.0.1:4800` by default.
