# .NET Core IoT Libraries

.NET Core can be used to build applications for [IoT](https://en.wikipedia.org/wiki/Internet_of_things) devices and scenarios. IoT applications typically interact with sensors, displays and input devices that require the use of [GPIO pins](https://en.wikipedia.org/wiki/General-purpose_input/output), serial ports or similar hardware.

This repository contains the [System.Device.Gpio](https://www.nuget.org/packages/System.Device.Gpio) library and implementations for various boards like [Raspberry Pi](https://www.raspberrypi.org/) and [Hummingboard](https://www.solid-run.com/nxp-family/hummingboard/).

The repository also contains [IoT.Device.Bindings](https://www.nuget.org/packages/Iot.Device.Bindings), a growing set of community-maintained [device bindings](src/devices/README.md) for IoT components.

**NOTE**: This repository is still in experimental stage and all APIs are subject to changes.

# How to Install

You can install the latest daily pre-release build of the .NET Core System.Device.Gpio and IoT.Device.Bindings NuGet packages from the blob feed.
  
## NuGet.exe
~~~~
nuget install System.Device.Gpio -PreRelease -Source https://dotnetfeed.blob.core.windows.net/dotnet-iot/index.json
nuget install IoT.Device.Bindings -PreRelease -Source https://dotnetfeed.blob.core.windows.net/dotnet-iot/index.json
~~~~
### Official Build Status
![BuildStatus](https://dev.azure.com/dnceng/internal/_apis/build/status/dotnet/iot/dotnet.iot-official?branchName=master)

## .NET CLI
~~~~
dotnet add package System.Device.Gpio --source https://dotnetfeed.blob.core.windows.net/dotnet-iot/index.json
dotnet add package IoT.Device.Bindings --source https://dotnetfeed.blob.core.windows.net/dotnet-iot/index.json
~~~~

# Getting Started

After installing, please see the following areas to learn more:

* [Documentation](Documentation/README.md) - Resources related to electronics, devices, vendors, software and other IoT topics.
* [Samples](samples/README.md) - Step-by-step instructions on building your first app.
* [Roadmap](Documentation/roadmap.md) - Areas planned or currently being worked on.

## Tutorials

* [Web service using SenseHat by Dawid Borycki (Aug 2019)](https://msdn.microsoft.com/magazine/mt833493)

# Community 

This project has adopted the code of conduct defined by the [Contributor Covenant](https://contributor-covenant.org/)
to clarify expected behavior in our community. For more information, see the [.NET Foundation Code of Conduct](https://www.dotnetfoundation.org/code-of-conduct).

# Contributing

Please contribute. We are primarily interested in the following:

* Improving quality and capability of the drivers for supported boards.
* Implementations for additional boards.
* [.NET device bindings](src/devices) for a wide variety of sensors, chips, displays and other components.
* Request a device binding or protocol that you need for your project ([file an issue](https://github.com/dotnet/iot/issues)).
* Links to blog posts or tweets that showcase .NET Core being used for great IoT scenarios ([file an issue](https://github.com/dotnet/iot/issues)).

# License

.NET Core (including the iot repo) is licensed under the [MIT license](LICENSE).
