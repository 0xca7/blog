# Blog Articles

Extracted articles from [0xca7.github.io](https://0xca7.github.io), organized by section. Each folder contains the article markdown and all referenced images/PDFs with corrected relative paths.

---

## blogs/

| # | Folder | Article | Synopsis |
|---|--------|---------|----------|
| 01 | [01_libopencm3_project](blogs/01_libopencm3_project/libopencm3_project.md) | ARM Cortex-M3 libopencm3 Project | Documenting a mini-project on the STM32 Blue Pill using libopencm3: fixed-point arithmetic (Q11.4), I2C readout of a TMP102 temperature sensor, timer interrupts, USART output, and a moving average filter. |
| 02 | [02_ghidrathon_unicorn](blogs/02_ghidrathon_unicorn/ghidrathon_unicorn.md) | Ghidrathon + Unicorn Engine + Capstone | A Ghidra Python3 script combining Ghidrathon, the Unicorn emulator and Capstone to build a mini ARM32 emulator inside Ghidra: select code, set registers interactively, and trace execution instruction-by-instruction with register and stack dumps. |
| 03 | [03_aoma](blogs/03_aoma/aoma.md) | The Art of Malware Analysis – Course Review | Short review of Ahmed's "The Art of Malware Analysis" course: covers basic to intermediate malware analysis, x86 assembly, config extraction, YARA rules, and task automation with real-world samples. Rated 10/10. |
| 04 | [04_aarch64_cpp](blogs/04_aarch64_cpp/aarch64_cpp.md) | Reversing AARCH64 C++ Binaries | PDF note set covering reverse engineering of C++ binaries compiled for AArch64/ARM64: basic classes, pure virtual methods, abstract classes, templates, and stripped binaries. |
| 05 | [05_rustre1](blogs/05_rustre1/rustre1.md) | Rust Reversing – Iterators | Walkthrough of reversing Rust iterator-based XOR encryption in both debug and release builds using Ghidra, showing how `iter_mut`/`for_each`/`fold` patterns appear in assembly and how the compiler optimises them. |
| 06 | [06_bggp5](blogs/06_bggp5/bggp5.md) | BGGP5 | BGGP5 entry: a CMake-based file downloader (`CMakeLists.txt`, 283 bytes) that fetches the challenge URL and prints its contents using `FetchContent` and a bash `cat` command. |
| 07 | [07_rustre2](blogs/07_rustre2/rustre2.md) | Rust Reversing – obfstr Crate | Deep-dive into reverse engineering binaries compiled with the `obfstr` crate (v0.4.4): explains the XOR keystream generation, xref obfuscation, and how to statically recover obfuscated strings from both release and debug builds. |

---

## notes/

| # | Folder | Article | Synopsis |
|---|--------|---------|----------|
| 01 | [01_calling_conventions](notes/01_calling_conventions/calling_conventions.md) | Calling Conventions | Quick-reference overview of x86/x86_64 calling conventions on Windows (stdcall, x64 ABI) and Linux (System V AMD64 ABI), covering register usage, argument passing, and return values. |
| 02 | [02_docker](notes/02_docker/docker.md) | Docker Notes | Practical Docker cheat-sheet: installation, pulling images, running and managing containers, volumes, networking, and common commands for day-to-day use. |
| 03 | [03_mount_jffs2](notes/03_mount_jffs2/mount_jffs2.md) | Mount JFFS2 Filesystems | Shell script and step-by-step guide for mounting JFFS2 filesystem images extracted from firmware blobs via binwalk, using a simulated MTD flash device. |
| 04 | [04_virt-manager-arm](notes/04_virt-manager-arm/virt-manager-arm.md) | Debian ARM/aarch64 in virt-manager | Step-by-step guide for running a Debian ARM or AArch64 virtual machine on an x86-64 host using virt-manager and QEMU, including setup, installation, and network configuration. |
| 05 | [05_pq_lattice](notes/05_pq_lattice/pq_lattice.md) | Lattice Cryptography Notes | Personal study notes on lattice-based (post-quantum) cryptography, provided as a PDF. |
| 06 | [06_docker_emulation](notes/06_docker_emulation/docker_emulation.md) | Firmware Emulation with Docker | Guide to emulating foreign-architecture firmware (MIPS/ARM) inside Docker containers using QEMU user-mode static binaries, expanding on a conference talk with ARM-specific examples. |
| 07 | [07_mount_ubifs](notes/07_mount_ubifs/mount_ubifs.md) | Mounting UBIFS | Command sequence for mounting UBIFS images on Linux: simulating a NAND device with `nandsim`, formatting with `ubiformat`, attaching via `ubiattach`, and mounting. |
| 08 | [08_extract_cramfs](notes/08_extract_cramfs/extract_cramfs.md) | Extract cramfs | One-page reference for extracting cramfs filesystem images: detecting endianness with `file`, byte-swapping big-endian images with `cramfsswap`, and extracting with `fsck.cramfs`. |
| 09 | [09_crust_of_rust](notes/09_crust_of_rust/crust_of_rust.md) | Crust of Rust – Notes | Study notes from Jon Gjengset's "Crust of Rust" video series, covering memory ordering and atomics, lifetimes, and smart pointers with interior mutability. |

---

## malware/

| # | Folder | Article | Synopsis |
|---|--------|---------|----------|
| 01 | [01_malware_analysis](mw/01_malware_analysis/malware_analysis.md) | Collection of Malware Analysis Writeups | Index page linking to five PDF analysis reports: Blackguard (.NET infostealer), Redline Stealer, a Go-based Linux stealer, a Linux botnet, and STOP/DJVU ransomware unpacking. |
| 02 | [02_blackguard](mw/02_blackguard/blackguard.md) | Blackguard Stealer | Analysis of Blackguard, a .NET infostealer. Full writeup in the accompanying PDF. |
| 03 | [03_redline](mw/03_redline/redline.md) | Redline Stealer Analysis | Analysis of the Redline credential stealer. Full writeup in the accompanying PDF. |
| 04 | [04_golang_stealer](mw/04_golang_stealer/golang_stealer.md) | Golang Stealer | Analysis of a stealer written in Go that targets Linux systems. Full writeup in the accompanying PDF. |
| 05 | [05_linux_botnet](mw/05_linux_botnet/linux_botnet.md) | Linux Botnet Analysis | Analysis of a botnet targeting Linux systems. Full writeup in the accompanying PDF. |
| 06 | [06_stop_djvu](mw/06_stop_djvu/stop_djvu.md) | Stop/DJVU Analysis | Unpacking walkthrough for the STOP/DJVU ransomware, which bundles stealer malware. Full writeup in the accompanying PDF. |
| 07 | [07_pebwalk_notes](mw/07_pebwalk_notes/pebwalk_notes.md) | Notes on PEB Walking | Detailed notes on PEB (Process Environment Block) walking and API hashing as seen in the BLISTER loader: annotated assembly walkthrough of the technique and curated reference links. |
| 08 | [08_ca7vsapt](mw/08_ca7vsapt/ca7vsapt.md) | Battling with APT Malware | Replication notes for an AhnLab APT malware report, adding two original findings: a custom string obfuscation routine (beyond simple XOR) and additional reversing details on the dropper component. |
| 09 | [09_wineloader](mw/09_wineloader/wineloader.md) | Wineloader | Analysis notes supplementing the Zscaler SPIKEDWINE/Wineloader report: static decryption of the RC4-encrypted main payload, string decryption, and C2 URL recovery, with annotated code snippets aimed at beginners. |
| 10 | [10_latrodectus](mw/10_latrodectus/latrodectus.md) | Latrodectus | Analysis of the Latrodectus malware loader, focusing on its CRC32-based API hashing scheme used to hide imported Windows API functions. |
