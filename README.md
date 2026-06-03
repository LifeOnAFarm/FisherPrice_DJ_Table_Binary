# Fisher Price DJ Table Firmware Binaries

This project contains binary firmware images for the Fisher Price DJ Table toy.

## About This Project

This project is an archival effort to preserve the Fisher Price DJ Table toy and enable self-repair. As the toy becomes increasingly difficult to find and support becomes unavailable, this firmware collection ensures that owners with sufficient technical knowledge can repair and restore their devices. By maintaining accessible copies of the original firmware, we support device longevity and prevent e-waste.

## Disclaimer

**The owners and contributors of this project are not responsible for any damage you may cause to your device through flashing or modification.** Working with flash memory and hardware modification carries risk, including but not limited to device bricking, electrical damage, or personal injury. Proceed only if you fully understand these risks and accept full responsibility for any consequences.

## Firmware Options

### Single Language

Single Language toys use a **N25Q032** (4MB SOIC 8) flash memory chip, with each binary holding a single language.

- **English**
  - File: DJTable-English.bin
  - SHA256: `cd481903fefcd58f0cac10b9ff9f80e8459589b6f3e88273c091b6b91368f1e3`

- **German**
  - File: DJTable-German.bin
  - SHA256: `7eb70257593da06f682a3ddda54a9d260d4fc514f645237f5ca74b08f8da61a6`

### Multi Language

Multi Language toys use a larger **N25Q064** chip and feature an additional button to toggle between languages.

**Note:** The MultiLan binary is too large to fit on the N25Q032 chip used in Single Language toys, it requires the N25Q064 or larger chip.

- **MultiLan**
  - DJTable-MultiLan.bin
  - SHA256: `7eb70257593da06f682a3ddda54a9d260d4fc514f645237f5ca74b08f8da61a6`

## Flashing Guidelines

### Requirements

To successfully flash a new firmware binary, you will need:

- **Technical Experience**: Familiarity with flashrom and SPI flash operations
- **Hardware**: An SPI flash programmer device (e.g., CH341A USB Flash reader/writer)
- **Optional but Recommended**: Soldering skills to safely remove and reattache the chip from the board

### Notes

This project provides guidelines and firmware binaries for repair purposes only. We are not providing direct step-by-step flashing instructions—we assume that anyone attempting this has existing knowledge of flashrom, SPI flash operations, and hardware modification. If you are unfamiliar with these tools and techniques, we recommend learning through external resources before proceeding.

While it is possible to perform this operation without soldering experience by using adapters or chip clips, physically removing the chip from the board provides the best success rate and minimizes risk of damage to the device.
