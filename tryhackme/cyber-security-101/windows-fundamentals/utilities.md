# Utilities

## System Configuration

System Configuration (MSConfig) is mainly used for advanced troubleshooting, like diagnose startup issues.

In the General tab, you can select devices and services to load upon boot. Normal, Diagnostic or Selective.

In Boot, you can define various boot options, like Safe, No GUI, and more.

Services tab lists all services configured for the system, regardless of their state. These are applications running in the background.

Startup just has a link to open Task Manager, to manage startup items.

Tools lists a variety of utilities to configure the OS further. This will also show the commands you can run to launch the corresponding tools through the run prompt.

## Tools

### Computer Management

One of the tools available is Change UAC settings, which lets you change or turn off UAC.

The Computer Management (compmgmt) utility has three primary sections:

1. System Tools
Task Scheduler lets you create common tasks for the computer to carry out automatically at specified times.

Event Viewer allows to view events that have occured on the computer. It's often used to diagnose problems and investige executed actions. There are five types that can be logged: Error, Warning, Information, Success Audit and Failure Audit.

Standard logs appear under Windows Logs. There's logs for Application, Security, System and CustomLog.

Shared Folders shows a complete list of shares and folders.

Sessions will show a list of users who are currently connected to the shares.

Open Files will show all folders and/or files that the connected users access.

Local Users and Groups is discussed earlier.

Performance has the utility Performance Monitor (perfmon). This shows performance data in real-time or from a log file. Useful for troubleshooting performance issues, local or remote.

Device Manager allows to view and configure the hardware attached to the computer.

2. Storage
Has Windows Server Backup and Disk Management. In the latter you can perform advanced storage tasks, such at setting up a new drive, extending/shrinking a partition, or assigning a drive letter.

3. Services and Applications
You can view more information about services, such as the properties. WMI (_Windows Management Instrumentation_) is configured by WMI Control. It's superseded by PowerShell, and thus deprecated in Windows 10.

### System Information

System Information (msinfo32) gathers information about the computer and displays a comprehensive view of the hardware, system components and software environment.

### Resource Monitor

Resource Monitor (resmon) displays per-process and aggregate CPU, memory, disk and network usage information. In addition to providing details about which processes are using individual file handles and modules.

It helps starting, stopping, pausing and resuming unresponsive applications. The process analysis feature helps identifying deadlocked processes and file locking conflicts.

It has four sections: CPU, Disk, Network and Memory.

### Command Prompt

The Command Prompt (cmd) lets you interact with the OS. A few commands include `hostname`, `whoami`, `ipconfig`. To get the help manual for a command, you use `/?`, as in `ipconfig /?`.

### Registry Editor

Windows Registry (regedit) is a central hierarchical database used to store information necessary to configure the system for one or more users, applications and hardware devices.

It contains information like:

- Profiles for each user
- Applications installed, and the documents it can create
- Propery sheet settings for folders and application icons
- Existing hardware on the system
- Ports being used
