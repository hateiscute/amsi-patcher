
# AMSI (Antimalware Scan Interface) Patching in PowerShell Processes

## Introduction

This repository contains a C# program that patches the Antimalware Scan Interface (AMSI) in all running PowerShell processes on a Windows system. AMSI is a Microsoft interface that allows antivirus and antimalware solutions to integrate with and scan PowerShell scripts for malicious content. By patching AMSI, you can bypass script scanning, which may be useful for research or testing purposes.

## Features

- Scans all running PowerShell processes.
- Dynamically loads the target process, AMSI library, and AMSI function addresses.
- Patches AMSI in-memory to disable script scanning.

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/hateiscute/amsi-patcher.git
   cd amsi-patcher
   ```

2. Build the C# project using Visual Studio or any C# compiler.

3. Run the compiled executable as an administrator:

   ```bash
   .\AmsiPatcher.exe
   ```

4. The program will search for running PowerShell processes and attempt to patch AMSI in each of them.

## Requirements

- Windows operating system
- Administrator privileges

## Disclaimer

This tool is provided for educational and research purposes only. It is essential to respect all relevant laws and regulations when using this code. Unauthorized tampering with system components may violate terms of service agreements or laws in your jurisdiction.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

This project was inspired by the original C code created by an anonymous author and was adapted to C# by [Your Name].

## Contributing

Contributions are welcome! If you find a bug or have suggestions for improvement, please open an issue or create a pull request.
