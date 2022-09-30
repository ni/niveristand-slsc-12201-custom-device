# SLSC-12201 DIO Plugin Custom Device

The **SLSC-12201 DIO Plugin Custom Device** enables access to properties, commands, and physical channels of the [SLSC-12201 33 V Digital I/O Conditioning Module](https://www.ni.com/en-ph/support/model.slsc-12201.html) within VeriStand.

## Using the Custom Device

- Download the latest release package from the [Releases page](https://github.com/ni/niveristand-slsc-12201-custom-device/releases).
- See the [User Guide](Docs/User%20Guide.md) for a walkthrough of using the Custom Device.

## LabVIEW Source Code Version

LabVIEW 2019

## Dependencies

### Running the custom device

- [VeriStand 2019 or later](https://www.ni.com/en-us/support/downloads/software-products/download.veristand.html)

### Developing or building from source

- [LabVIEW 2019 or later](https://www.ni.com/en-us/support/downloads/software-products/download.labview.html)
- [LabVIEW Real-Time Module](https://www.ni.com/en-us/support/downloads/software-products/download.labview-real-time-module.html)
- [NI R Series Multifunction RIO](https://www.ni.com/en-us/support/downloads/drivers/download.ni-r-series-multifunction-rio.html)
  - Required for FPGA-based loopback test, not a direct dependency of the Custom Device
- [VeriStand Custom Device Development Tools](https://github.com/ni/niveristand-custom-device-development-tools)
  - Install the latest package from the [release page](https://github.com/ni/niveristand-custom-device-development-tools/releases)
- [VeriStand Custom Device Testing Tools](https://github.com/ni/niveristand-custom-device-testing-tools)
  - Install the latest package from the [release page](https://github.com/ni/niveristand-custom-device-testing-tools/releases)

## Git History & Rebasing Policy
Branch rebasing and other history modifications will be listed here, with several notable exceptions:
- Branches prefixed with `dev/` may be rebased, overwritten, or deleted at any time.
- Pull requests may be squashed on merge.

## License

The SLSC-12201 DIO Plugin Custom Device is licensed under an MIT-style license (see LICENSE). Other incorporated projects may be licensed under different licenses. All licenses allow for non-commercial and commercial use.
