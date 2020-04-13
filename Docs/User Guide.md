## Overview

The SLSC-12201 DIO Plugin Custom Device allows a enables access to properties, commands, and physical channels of the [SLSC-12201 33 V Digital I/O Conditioning Module](https://www.ni.com/en-ph/support/model.slsc-12201.html) within VeriStand.

## Usage

The SLSC-12201 DIO Plugin Custom Device is added to VeriStand as a module in an SLSC Chassis under the desired controller. An example of this location is _Targets » Controller » Hardware » SLSC » SLSC Chassis » Modules_, as shown below.

![Add Module to System Definition](Support\Add%20Module%20to%20System%20Definition.png)

Once the module has been added, configurations for all board **Bank** and **Line** parameters are available. These properties are applied on deployment of the system definition.

![Module Configuration](Support/Module%20Configuration.png)

Each **Bank** and **Line** also has channels added to the system definition so board configuration can be changed while the system is deployed. The settings for these channels are only updated in the deployed system when a **Command** is sent. They are not updated when the channel value changes.

**Command** apply a specific command each time the channel value is changed from **0** to **1**. In order to change a channel configuration, use the **Update Channel Configuration** channel. For example, to enable _Line 0_ on _Port 0_, set the _Line 0_ **Enable** channel to **1** and then set the **Update Channel Configuration** channel to **1**. This will send a property change to the SLSC-12201 card and command to apply those changes.

**Diagnostic** channels are also provided to show the state of various parts of the board. **SLSC Mod Update Rate** and **SLSC Mod Loop Rate** provide information about the loop rate of the asynchronous loop in the custom device. The various **Power Fail** channels will remain set until the **Acknowledge Vsup Fail** command channel has been set.

![Diagnostic Channels](Support/Diagnostic%20Channels.png)

## References

[SLSC-12201 33 V Digital I/O Conditioning Module](https://www.ni.com/en-ph/support/model.slsc-12201.html)

[SLSC-12201 Getting Started Guide](https://www.ni.com/pdf/manuals/377035c.pdf)

[Legacy Release Notes](https://forums.ni.com/t5/NI-VeriStand-Add-Ons-Documents/NI-VeriStand-Add-on-SLSC-12201-DIO-Plugin-Custom-Device/ta-p/3690531)

[Legacy Support Forum](https://forums.ni.com/t5/NI-VeriStand-Add-Ons-Discussions/SLSC-12201-DIO-Plugin-Custom-Device/td-p/3690527)
