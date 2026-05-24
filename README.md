# NAT_Simulator

A browser-based simulator for understanding how **Network Address Translation (NAT)** works in computer networks.

Supports:
- Dynamic NAT
- Static NAT
- PAT (Port Address Translation)
---

## Features

- Real-time packet translation
- NAT translation table
- Private/Public IP validation
- Packet logs and statistics
- PAT port allocation & collision handling
- Automatic inbound packet simulation
- Downloadable NAT session report
- Interactive learning/help section
---

## Tech Stack

- HTML5
- CSS3
- JavaScript
- FileSaver.js
---

## How It Works

1. The user selects a NAT type and enters:
   - Source IP & Port
   - Destination IP & Port
   - Public IP

2. When a packet is sent:
   - The simulator checks the NAT table
   - Creates a translation entry if needed
   - Translates the private IP into a public IP
   - Allocates ports in PAT mode
   - Logs every translation step in real time

3. The simulator then:
   - Updates the NAT translation table
   - Tracks packet statistics
   - Simulates inbound response packets
   - Performs reverse NAT translation

4. NAT entries automatically expire after timeout.
---

## Supported Private IP Ranges

- `10.x.x.x`
- `172.16.x.x – 172.31.x.x`
- `192.168.x.x`

The simulator automatically detects:
- Private IPs
- Public IPs
- Invalid IP formats
---

## NAT Types

### Dynamic NAT
Temporary private-to-public IP mapping.

### Static NAT
Permanent one-to-one IP mapping.

### PAT
Multiple devices share one public IP using different ports.
---

## How to Run

1. Download or clone the repository
2. Open `index.html` in a browser

Or run using VS Code Live Server.
---
