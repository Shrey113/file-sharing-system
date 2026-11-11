# File Sharing System

Professional peer-to-peer file and data transfer software engineered for high-throughput, zero-cloud local area network exchange across Windows, macOS, Linux, Android, and web platforms.

---

## Overview

File Sharing System is a secure, decentralized local communication utility designed for high-speed file and clipboard synchronization without relying on external cloud infrastructure, internet connectivity, or remote intermediate relays. 

All communications occur strictly within the boundaries of the local area network (LAN) or direct wireless access point, ensuring enterprise-grade privacy, zero bandwidth metering, and transmission speeds bounded only by physical network hardware.

---

## Key Capabilities

### High-Throughput Data Transmission
Transfers raw files, documents, and media at maximum physical interface throughput over local Wi-Fi, Ethernet, and direct wireless connections utilizing optimized native multithreaded socket pipelines.

### Automated Local Peer Discovery
Discovers neighboring devices on the subnet automatically through industry-standard Zero-Configuration Networking (mDNS/DNS-SD). Devices broadcast their availability and identify peers without manual IP configuration.

### Batch Processing and Selective Approval
Supports simultaneous dispatch of multiple files and structured payloads. Receiving parties are presented with an itemized verification prompt, permitting selective approval or refusal of individual items before writing to storage.

### Real-Time Text and Hyperlink Dispatch
Enables instantaneous transmission of clipboard text, secure notes, and URLs across platforms with direct action triggers, including single-action clipboard copying and direct browser navigation.

### Zero-Installation Browser Client
Includes an embedded HTTP server enabling any web-enabled platform without installed client software to participate in transfers via modern web browsers through direct local address access or optical matrix (QR) pairing.

### Network Adapter Isolation
Automatically detects and selects active physical network interfaces, isolating transmission from virtual machine bridges, container virtualization adapters, and tunneling interfaces to ensure reliable routing.

### Background Resident Operation
Features an unobtrusive system status interface and background execution mode, allowing long-running transfers to persist without active window focus.

---

## Supported Platforms and Deliverables

Pre-compiled production deliverables are provided for each supported operating system:

| Platform | Target Architecture | Distribution Format |
|---|---|---|
| **Windows** | x86_64 / x64 | Standalone Portable Executable (`.exe`) / ZIP |
| **Android** | ARM64-v8a / armeabi-v7a / x86_64 | Android Package Kit (`.apk`) |
| **macOS** | Universal Binary (Apple Silicon & Intel) | Signed Application Bundle (`.app` / `.zip`) |
| **Linux** | x86_64 / x64 | Portable Standalone Binary (`.tar.gz`) |
| **Web** | Cross-Platform (All Modern Browsers) | Embedded HTTP Portal (Port 9876) |

---

## Deployment and Usage

### Desktop (Windows, macOS, Linux)

1. Download the designated release archive for your operating system.
2. Extract the archive contents to your preferred system directory.
3. Launch the application executable.
4. Ensure your firewall grants inbound and outbound UDP/TCP permissions on local subnet ranges for network discovery and file transport.

### Android

1. Download the application package (`.apk`) directly to the device.
2. Grant permission for installation from your file manager when prompted.
3. Open the application and grant the requested local network and storage permissions required for foreground background transfers.

### Web Browser Client

1. Ensure the desktop or Android client application is actively running on the host device.
2. Locate the displayed host address or scan the displayed optical pairing code.
3. Navigate to the indicated local endpoint (`http://<HOST_IP>:9876`) within any standard web browser on the client device.
4. Upload files or send text directly through the responsive web interface.

---

## Security and Data Privacy Architecture

- **Subnet Confinement**: All transmissions remain entirely within the local broadcast domain. No telemetries, analytics, or payload packets are transmitted to external servers.
- **Physical Interface Pinning**: Socket operations bind directly to physical network adapters, preventing accidental transmission through virtual adapters or VPN tunnels.
- **Mandatory Consent Protocol**: Incoming transfers require explicit recipient confirmation prior to initiating filesystem write operations.

---

## Proprietary License Agreement

Copyright (c) 2026. All rights reserved.

This software and associated binary distributions are proprietary and confidential.

### Permitted Use
Permission is granted to download, install, and execute the pre-compiled binary releases (.exe, .apk, and related system packages) solely for personal or internal organizational use.

### Prohibited Activities
1. **No Source Code Access**: Source code is proprietary, confidential, and not licensed under this agreement.
2. **No Reverse Engineering**: Decompilation, disassembly, reverse engineering, decryption, or extraction of underlying source code, protocols, or architecture is strictly prohibited.
3. **No Modification or Derivative Works**: Modification, adaptation, translation, patching, or creation of derivative works based on this software is strictly prohibited.
4. **No Redistribution or Reselling**: Redistribution, sublicensing, leasing, renting, hosting as a paid commercial service, or commercial resale of the software binaries without express written authorization is strictly prohibited.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY ARISING FROM OR IN CONNECTION WITH THE SOFTWARE OR ITS USE.
