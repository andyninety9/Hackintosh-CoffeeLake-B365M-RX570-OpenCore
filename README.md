# Hackintosh-CoffeeLake-B365M-RX570-OpenCore
Hackintosh macOS Ventura 13.2.1 in MSI B365M Pro-VH + Intel Core I3-9100F + Gigabyte Radeon RX 570

<img src="https://github.com/andyninety9/Hackintosh-CoffeeLake-B365M-RX570-OpenCore/blob/6fe7265b529d28c47aea2aee6b128b9ea6b99025/Screenshot%20Desktop.png" />

## Bootloader:
[OpenCore 0.9.0](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.0)

## Hardware:
- CPU: Intel Core I3-9100F (CoffeeLake)
- Mainboard: MSI B365M Pro-VH
- dGPU: AMD Radeon RX 570 4GB (Polaris 20)
- Wireless Card: Intel® Dual Band Wireless-AC 7260

## Bios Settings:

- Hotkey Bios: Delete
- Hotkey Boot Options: F11
- Change to __Advanced Mode__: F7
- __Save & Exit:__
    - Restore Defaults → Yes

- __Settings__

    - __Advanced__
        - PCI sub-system Settings:
            - Above 4G memory/Crypto Currentcy mining → __Enabled__
        - Integrated Peripherals:
            - SATA Configuration
                - SATA Mode → __AHCI Mode__
        - Intergrated Graphics Configuration
            - Integrated Grahics Adapter → __PEG__
            - Integrated Grahics Share Memory → 64MB
            - IGD Multi-Monitor → __Enabled (Card onboard)__
        - USB Configuration
            - XHCI Hand-off → __Enabled__
        - Super IO settings
            - Serial(COM) Port 0 Configuration
                - Serial Port → __Disabled__
        - Windows OS Configuration
            - MSI Fast boot → __Disabled__
            - Fast Boot → __Disabled__
    - __Boot__
        - Boot Option #1 → __UEFI USB Key: Name of your USB__
    - __OC (Overclocking)__
        - Extreme Memory Profile(X.M.P) → __Enabled__
        - CPU Features
            - Intel VT-D Tech → __Disabled__
            - CFG Lock → __Disabled__
        
    #### Note: 
        - To set default iGPU: 
            -Integrated Graphics Adapter → IGD
        - To turn-off iGPU (only dGPU):
            - IGD Multi-Monitor → Disabled

## Working:

- __Everything Working Normally Except Bluetooth USB (TP-Link UB500)__

## Credits:
### I appreciate your support! Your assistance was pivotal in the construction process.
- [Dortania](https://github.com/dortania)
- [OpenCore](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.0)