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

### `apt-get` (Debian)

Some Linux distributions publish their own `dotnet` packages (install via `apt-get`), including **Debian**.

Follow the instructions here:

https://learn.microsoft.com/en-us/dotnet/core/install/linux-debian?tabs=dotnet10

to install **.NET SDK**

### scripted install

For other distributions (e.g. Linux Mint), use the script based install procedure:

https://learn.microsoft.com/en-us/dotnet/core/install/linux-scripted-manual#scripted-install

```bash
$ wget https://dot.net/v1/dotnet-install.sh -O dotnet-install.sh
$ chmod +x ./dotnet-install.sh
$ ./dotnet-install.sh --version latest
```

Test run `dotnet --version`; if says command not found, find where `dotnet` was installed:

```bash
$ find / -namfind / -name "dotnet" -type f 2>/dev/null
```
and test run e.g.:
```bash
$ /home/mariia/.dotnet/dotnet --version
10.0.300
```
EAdd `dotnet` to `$PATH` in `.bashrc` so that it is "visible" to other programs like Rider. Example in this case, add this line:

```bash
$ export PATH=$PATH:$HOME/.dotnet
```
then
```bash
$ source ~/.bashrc
```
then test `dotnet --version`

## MVC Web App project

Create project:

Open Rider > New Solution > Select Project Type Web > Language C# > Web App (Model-View-Controller) > Create

### Test run

Open main view file: `Views` > `Home` > `Index.cshtml`

Click the green Run button or `F5` to build + run.

### Model-View-Controller structure

