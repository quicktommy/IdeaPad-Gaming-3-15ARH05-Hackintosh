# Lenovo IdeaPad Gaming 3 15ARH05 – macOS Tahoe EFI

An OpenCore EFI configuration for running **macOS Tahoe** on the Lenovo IdeaPad Gaming 3 15ARH05 (AMD Ryzen).

This project is based on the original macOS Sequoia EFI by [@aman71711](https://github.com/aman71711/Lenovo-IdeaPad-Gaming-3-15ARH05-Hackintosh-EFI-), which was adapted for macOS Tahoe and further modified to include Intel AX210 Wi-Fi and Bluetooth support.

## Hardware Specifications

| Component | Specification |
|---|---|
| Laptop | Lenovo IdeaPad Gaming 3 15ARH05 |
| CPU | AMD Ryzen 5 4600H |
| Integrated GPU | AMD Radeon Vega 6 |
| Dedicated GPU | NVIDIA GeForce GTX 1650 Ti Mobile |
| RAM | 24 GB (although any decent amount of ram works) |
| Wi-Fi | Intel Wi-Fi 6 AX210 NGW |
| Bluetooth | Intel AX210 Bluetooth |
| Storage | UMIS CT1000P25508 – 1 TB NVMe (not mandatory, just my own) |
| BIOS | FCCN21WW |

## EFI Configurations

Two separate EFI configurations are provided.

### 1. Recovery EFI

A minimal EFI configuration intended for:

- Booting into macOS Recovery.
- Initial macOS installation.
- Recovery and troubleshooting purposes.

This configuration prioritizes installation compatibility over having every hardware feature enabled.

### 2. Full EFI

The complete EFI configuration intended for everyday use after macOS installation.

Includes additional hardware configurations and support, including:

- Intel AX210 Wi-Fi support.
- Intel AX210 Bluetooth support.
- Full system configuration for the installed operating system.

**Important:** Use the Recovery EFI for installation and the Full EFI for normal system booting.

## Graphics Compatibility

The AMD Radeon Vega 6 is the integrated graphics solution used for macOS graphics.

The NVIDIA GTX 1650 Ti Mobile is unsupported by macOS and cannot provide native graphics acceleration.

## Wireless Connectivity

Unlike the original configuration, this EFI includes support for a non-stock Intel AX210 NGW wireless card.

Both Wi-Fi and Bluetooth configurations have been added to the Full EFI.

**Note:** This configuration assumes the Intel AX210 wireless card is installed. Other wireless cards may require different configurations.

## Original Project & Credits

This project wouldn't exist in its current form without the original work by:

- [@aman71711 – Lenovo IdeaPad Gaming 3 15ARH05 Hackintosh EFI](https://github.com/aman71711/Lenovo-IdeaPad-Gaming-3-15ARH05-Hackintosh-EFI-)

The original project provided the macOS Sequoia EFI, which served as the foundation for this macOS Tahoe adaptation.

Additional acknowledgements:

- [OpenCore](https://github.com/acidanthera/OpenCorePkg)
- [Dortania OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [AMD-OSX](https://github.com/AMD-OSX)

## Disclaimer

This project is provided for educational and experimental purposes.

Hardware compatibility may vary between individual laptop configurations.

Always generate your own SMBIOS identifiers before using this EFI. Never reuse another person's serial numbers, MLB, ROM or SystemUUID.

No guarantee of compatibility with other hardware configurations or macOS versions is provided.

---

**macOS Tahoe | AMD Ryzen 5 4600H | OpenCore | Intel AX210**
