# Reverse Engineering

## What Is Reverse Engineering?

Reverse engineering is the process of analyzing a compiled program (usually without source code) to understand its structure, logic, and functionality. It's often used in cybersecurity to analyze malware, uncover software vulnerabilities, or solve CTF challenges.

---

## Goals of Reverse Engineering

- Understand how a binary works
- Recover source-like logic
- Analyze malicious behavior (e.g., malware)
- Find hidden logic or secrets (e.g., flags or serial keys)

---

## Typical Reverse Engineering Tasks

- Analyze control flow and logic
- Understand algorithms (e.g., encryption, compression)
- Bypass software protections
- Extract hardcoded secrets

---

## Common Tools

- `Ghidra`: A powerful open-source reverse engineering suite from the NSA.
- `IDA Free/Pro`: Industry-standard disassembler and debugger.
- `Radare2` / `Cutter`: Open-source reverse engineering tools.
- `x64dbg` (Windows): For debugging and analyzing PE binaries.
- `strings`, `ltrace`, `strace`: Command-line tools for basic binary inspection.

---

## File Types and Targets

- Executable and Linkable Format (ELF) - Linux
- Portable Executable (PE) - Windows
- Firmware dumps
- Android APKs

---

## Learning Resources

- [Malware Unicorn RE101](https://malwareunicorn.org/workshops/re101.html)
- [Ghidra Reverse Engineering Wiki](https://ghidra-sre.org/)
- [OpenSecurityTraining.info](https://opensecuritytraining.info/)
- YouTube channels: LiveOverflow, OALabs
