# Forensics

## What Is Digital Forensics?

Forensics in cybersecurity and CTFs refers to the analysis and investigation of digital artifacts to uncover hidden information, trace activity, or recover data. In CTF challenges, it's about digging into files, memory dumps, network traffic, or disk images to find flags or clues.

---

## Common Forensics Tasks in CTFs

- **Analyzing Images**: Using tools to extract metadata, hidden files, or steganography.
- **Inspecting Network Traffic**: Parsing `.pcap` files to find credentials, flags, or secret data.
- **File Carving**: Recovering files from raw binary or disk dumps.
- **Memory Dump Analysis**: Searching through RAM dumps for secrets or running processes.
- **Metadata Extraction**: Getting hidden info from file headers or properties.
- **Log Analysis**: Examining logs to trace attacker actions or find hidden messages.
- **Steganography**: Finding data hidden inside images, audio, or video files.

---

## Common Tools

- `binwalk`: Extracts embedded files from binaries or firmware.
- `strings`: Searches for readable ASCII/Unicode strings in files.
- `foremost` / `scalpel`: File carving tools.
- `exiftool`: Extracts metadata from images and documents.
- `Wireshark`: Analyzes network packet captures (`.pcap` files).
- `Volatility`: Memory forensics tool to inspect RAM dumps.
- `zsteg`, `steghide`, `stegsolve`: Tools for steganographic analysis.

---

## Common File Types in Forensics Challenges

- `.pcap` – Packet captures
- `.img`, `.bin` – Disk or memory images
- `.jpg`, `.png`, `.wav`, `.mp3` – Files possibly used for steganography
- `.docx`, `.pdf`, `.xlsx` – Metadata-heavy documents

---

## Tips and Techniques

- Check for hidden or embedded files using `binwalk` or `foremost`.
- Run `strings` to look for flags, passwords, or clues.
- Always inspect metadata with `exiftool`.
- In `.pcap` files, look for HTTP/FTP logins, DNS queries, or file transfers.
- Use hex editors to find signatures of hidden data (e.g., `HxD`, `010 Editor`, `hexed.it`).

---

## Learning Resources

- [Volatility Foundation](https://www.volatilityfoundation.org/)
- [Wireshark Documentation](https://www.wireshark.org/docs/)
- [CyberDefenders Forensics Challenges](https://cyberdefenders.org/challenges/)
- [HackTheBox Forensics](https://app.hackthebox.com/challenges)
- [OverTheWire – Bandit](https://overthewire.org/wargames/bandit/) – Good intro to Linux file analysis
- YouTube: John Hammond, LiveOverflow (Forensics & Stego playlists)

---

## Typical CTF Flag Formats

- Plain text flags hidden in files
- Flags in the form `picoCTF{example_flag}`
- Strings hidden in stego images or base64-encoded blobs

---

## Final Note

Forensics challenges reward patience and attention to detail. Don’t forget to try:
- Changing file extensions
- Unzipping unknown formats
- Viewing files in a hex editor
- Analyzing headers and tails

> "Every byte tells a story."
