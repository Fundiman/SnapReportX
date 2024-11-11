# SnapReportX

**SnapReportX** is a powerful system reporting tool created by Fundiman. It generates an extensive system report containing detailed information about your machine's hardware, software, network configuration, processes, and more. Whether you're troubleshooting, auditing, or just curious about your system, SnapReportX is designed to provide a thorough snapshot.

## Features

- **System Information**: Displays kernel version, system architecture, and general system stats.
- **CPU & Memory Info**: Gives detailed information about your CPU cores, memory usage, and more.
- **Storage & GPU**: Lists available storage devices, disk partitions, and GPU details.
- **Network Info**: Shows network interfaces, IP addresses, routing tables, and more.
- **Packages & Processes**: Lists installed packages and running processes.
- **Logs & Configuration**: Provides access to logs, system services, and configuration files.
- **Power Management**: Displays information about power settings and battery status.
- **Security**: Includes firewall rules, SELinux status, and available security updates.

## Requirements

- Linux-based operating system (tested on Ubuntu, Fedora, Debian)
- `sudo` privileges (for accessing certain system information)
- Installed utilities:
  - `lscpu`, `free`, `df`, `lsblk`, `lspci`, `uname`, `top`, `htop`, `sensors`, etc.
  - Package managers like `apt`, `dnf`, `yum`, `pacman`, etc.

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/Fundiman/SnapReportX.git
   ```

2. Make the script executable:
   ```
   chmod +x snapreportx
   ```

3. Run the script:
   ```
   ./snapreportx
   ```

## Usage

Once the script is executed, you will be prompted to enter an output file name. SnapReportX will begin collecting and processing system information. Depending on the system's complexity, this may take a few minutes or hours. After completion, the report will be saved in the specified output file.

**Example output**:

```
SnapReportX by Fundiman on Linux
Please enter the output file name: system_report.txt
Started recording report on Sun Nov 11 12:34:56 UTC 2024...
Please wait for SnapReportX to collect info to create the report...
This may take few hours...
Till that time, Sit back and relax and let the process happen...
```

The report will contain sections including:

- System Information
- Distro Information
- CPU, Memory, Storage, and GPU details
- Network configuration and active devices
- Running processes and system logs
- Available security updates and more

## Supported Commands

- **System Info**: `uname`, `hostnamectl`, `lsblk`, etc.
- **Package Managers**: Detects and lists installed packages using common package managers.
- **Network Management**: Shows details of network interfaces, IPs, and routing.
- **Security & System Configuration**: Includes firewall status, SELinux, and AppArmor details.

## Contributing

Feel free to contribute by forking the repository and submitting a pull request for bug fixes or new features.

## License

SnapReportX is open-source software licensed under the MIT License. See the LICENSE file for more details.
