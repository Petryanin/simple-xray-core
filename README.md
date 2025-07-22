# Simplified Xray Core Management

This repository provides a set of scripts to simplify the installation and management of the Xray core, allowing you to run a personal VPN without needing a control panel. The main advantages of this approach are minimal resource usage and no requirement for a domain name or TLS certificates.

## Scripts Overview

- **`xray-install`**: Automates the entire setup process. It installs the Xray core, configures it with a primary user, and creates a single management script (`xray-manager`) for all user-related tasks.
- **`xray-uninstall`**: Completely removes the Xray core and all associated configuration files and scripts from your server.

## Installation

To install Xray, run the following command. The script will prompt you to enter a domain (optional) and a label for your first user.

```sh
wget -qO- https://raw.githubusercontent.com/Petryanin/simple-xray-core/main/xray-install | bash
```

## User Management

After installation, a single command, `xray-manager`, is available for all user management tasks. Here’s how to use it:

**List all users:**

```sh
xray-manager list
```

**Add a new user:**

```sh
xray-manager add
```

**Remove a user:**

```sh
xray-manager remove
```

**Get the connection link for a specific user:**

```sh
xray-manager link
```

**Get the link for the first (main) user:**

```sh
xray-manager mainlink
```

A help file with these commands will also be created at `~/xray-help`.

## Uninstallation

To completely remove Xray and all related files, use this command:

```sh
wget -qO- https://raw.githubusercontent.com/Petryanin/simple-xray-core/main/xray-uninstall | bash
```

## Useful Links

- [Xray Core GitHub Repository](https://github.com/XTLS/Xray-core)
- [Official Documentation](https://xtls.github.io/en/)

## Recommended Client Apps

Here are some recommended client applications for connecting to your Xray server:

### Windows

- [Nekoray](https://github.com/MatsuriDayo/nekoray)
- [v2rayN](https://github.com/2dust/v2rayN)
- [Furious](https://github.com/LorenEteval/Furious)
- [Invisible Man - Xray](https://github.com/InvisibleManVPN/InvisibleMan-XRayClient)

### Android

- [v2rayNG](https://github.com/2dust/v2rayNG)
- [X-flutter](https://github.com/XTLS/X-flutter)
- [SaeedDev94/Xray](https://github.com/SaeedDev94/Xray)

### iOS & macOS arm64

- [Streisand](https://apps.apple.com/app/streisand/id6450534064)
- [Happ](https://apps.apple.com/app/happ-proxy-utility/id6504287215)
- [OneXray](https://github.com/OneXray/OneXray)

### macOS arm64 & x64

- [V2rayU](https://github.com/yanue/V2rayU)
- [V2RayXS](https://github.com/tzmax/V2RayXS)
- [Furious](https://github.com/LorenEteval/Furious)
- [OneXray](https://github.com/OneXray/OneXray)

### Linux

- [Nekoray](https://github.com/MatsuriDayo/nekoray)
- [v2rayA](https://github.com/v2rayA/v2rayA)
- [Furious](https://github.com/LorenEteval/Furious)
