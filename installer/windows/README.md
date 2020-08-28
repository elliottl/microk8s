# MicroK8s Installer

## Windows
Uses the NSIS package to create the installer.  

### Prerequisites

* Requires [NSIS 3](https://nsis.sourceforge.io/Download).
* Requires the [EnVar plug in](https://nsis.sourceforge.io/EnVar_plug-in) to compile.

### Building

2 files must be placed in the working directory before compiling the installer.  These are:

* `microk8s.exe`:  This is the file generated by PyInstaller.
* `multipass.exe`:  This is the Multipass installer exe, which is run at install time.

Use the following command to compile the installer.

```
makensis microk8s.nsi
```