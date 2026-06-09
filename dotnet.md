# C#/.NET project setup

## JetBrains Rider
Download JetBrains Rider `.tar.gz` from:

https://www.jetbrains.com/rider/download/

Unpack the `.tar.gz`
```bash
tar -xzvf JetBrains.Rider-2026.1.2.tar.gz
```

Test: run Rider from the unpacked folder
```bash
$ cd JetBrains Rider-2026.1.2
$ ./bin/rider
```

## Install .NET

Some Linux distributions publish their own `dotnet` packages (install via `apt-get`), including **Debian**.

Follow the instructions here:

https://learn.microsoft.com/en-us/dotnet/core/install/linux-debian?tabs=dotnet10

to install **.NET SDK**

For other distributions (e.g. Linux Mint), use the script based install procedure:

https://learn.microsoft.com/en-us/dotnet/core/install/linux-scripted-manual#scripted-install

```bash
$ wget https://dot.net/v1/dotnet-install.sh -O dotnet-install.sh
$ chmod +x ./dotnet-install.sh
$ ./dotnet-install.sh --version latest
```
