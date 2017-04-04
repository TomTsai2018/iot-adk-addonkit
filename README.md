# iot-adk-addonkit
This project contains command line scripts for package creation and image creation process. Users are expected to have ADK and WDK installed to make use of this. In addition, this project also contains samples for iot products based on RPi2/MBM. To be able to create images, Users should get Windows 10 IoT Core OS Packages from MSDN. Target audience is OEM’s and Maker Pro’s who want to manage multiple images and updates.

This project has adopted the [Microsoft Open Source Code of Conduct](http://microsoft.github.io/codeofconduct). For more information see the [Code of Conduct FAQ](http://microsoft.github.io/codeofconduct/faq.md) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Branch Overview

## Master Branch
This branch supports the lastest Windows 10 IoT Core release available ( currently 1607, version number 10.0.14393.x )

## Develop Branch
This branch contains the active development contents, mostly addressing the upcoming release features.

## Older Versions
* [10586_v1.0 release](https://github.com/ms-iot/iot-adk-addonkit/releases/tag/v1.0) for Windows 10 IoT Core Release 1511 (version 10.0.10586.x).


# References

## User Guides
* [IoT Core Manufacturing Guide](https://msdn.microsoft.com/windows/hardware/commercialize/manufacture/iot/iot-core-manufacturing-guide)
    * [Windows ADK IoT Core Add-Ons Overview](https://go.microsoft.com/fwlink/p/?LinkId=735029)
    * [IoT Core Add-Ons command-line options](https://msdn.microsoft.com/windows/hardware/commercialize/manufacture/iot/iot-core-adk-addons-command-line-options)
    * [IoT Core feature list](https://msdn.microsoft.com/windows/hardware/commercialize/manufacture/iot/iot-core-feature-list)
* [Learn how to build on Windows 10 IoT Core](https://developer.microsoft.com/windows/iot/Docs)
    * [Windows Device Portal](https://developer.microsoft.com/windows/iot/docs/deviceportal)

## Downloads

* IoT Core OS Packages
    * [Version 1607](https://www.microsoft.com/en-us/download/details.aspx?id=53898) **Now available for free**
    * [Version 1511](https://msdn.microsoft.com/subscriptions/downloads/default.aspx#FileId=67415)
* [Windows Assessment and Deployment Kit](https://developer.microsoft.com/windows/hardware/windows-assessment-deployment-kit#winADK)
    * [ADK Version 1607](https://go.microsoft.com/fwlink/p/?LinkId=526740)
    * [ADK Version 1511](https://go.microsoft.com/fwlink/p/?LinkId=823089)
* [Windows Driver Kit - WDK](https://go.microsoft.com/fwlink/p/?LinkId=526733)
* [Windows 10 IoT Core Dashboard](https://developer.microsoft.com/windows/iot/docs/iotdashboard)

## BSPs

### Raspberry Pi BSP

  The drivers required for the Raspberry Pi are available in the github project : [ms-iot/bsp](https://github.com/ms-iot/bsp)

  Steps to create the drivers :
    1. check out ms-iot/bsp project
    2. Build the bcm2386 solution
    3. Go to the tools folder and run
        binexport Release/debug <target folder> eg. binexport release c:\rpibsp
    4. In IoTCoreShell, run C:\rpibsp\build.cmd
  The required cabs will be created in the output folder.

  You can also download the prebuilt binaries available in the release : [rpibsp.zip](https://github.com/ms-iot/iot-adk-addonkit/releases/download/RPiBSP/rpibsp.zip)

### Intel BSPs
  
  See below links for the Intel platforms.
  
* Bay Trail [IO Drivers](https://downloadcenter.intel.com/download/25618), [Graphics Drivers](https://downloadcenter.intel.com/download/25606)

* [ApolloLake](http://www.intel.com/content/www/us/en/embedded/products/apollo-lake/mr2-best-known-configuration.html)

* [Joule](https://downloadcenter.intel.com/)


### Qualcomm BSP

Contact [Qualcomm](mailto:pahwang@qti.qualcomm.com) for the BSPs.




    
  
  

