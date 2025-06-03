# Wireshark HTTP Traffic Analysis

This project explores basic HTTP traffic using a `.pcapng` file analyzed in Wireshark. It demonstrates how to inspect packets, analyze HTTP requests/responses, and understand the flow between a client and server.

- **Tool Used:** Wireshark
- **Trace File:** `Wireshark-HTTP-Overview.pcapng`
- **Target Host:** `gaia.cs.umass.edu`

---

## 🔍 Key Findings

### 1. Total Packets Captured
422 packets were captured in total during the browsing session.

<img src="https://i.imgur.com/6lh4gG5.png" />

---

### 2. HTTP Packets Identified
Using the display filter `http`, 8 HTTP packets were isolated.

<img src="https://i.imgur.com/0TsoqqK.png" />

---

### 3. Target Server IP
DNS lookup of `gaia.cs.umass.edu` returned `128.119.245.12`.

<img src="https://i.imgur.com/fD5v6eU.png" />

---

### 4. HTTP Packets Between Client and Server
Using the filter `http && ip.addr==128.119.245.12`, we isolate HTTP packets exchanged with the target server.

<img src="https://i.imgur.com/9zCGEBx.png" />

---

### 5. Favicon Not Found
The client requested a favicon, but the server responded with a 404 Not Found.

<img src="https://i.imgur.com/z4nJfXH.png" />

---

## 📁 Additional Screenshots & Analysis

For a complete walkthrough, including:
- Content-Length & Content-Type headers
- HTTP body preview
- All HTTP packet details

➡️ View the full image album here: [Imgur Album Link](https://imgur.com/a/VMJkhhU)

---

## 🧠 Skills Demonstrated

- Network packet filtering (`http`, `ip.addr`)
- DNS resolution and IP analysis
- HTTP header and payload interpretation
- Real-world client-server communication analysis

---

## 📌 Files

- `Wireshark-HTTP-Overview.pcapng` – Raw packet capture used in this analysis

---

## 🔐 Disclaimer

This project is for educational purposes and used publicly available capture files. No private data was inspected.
