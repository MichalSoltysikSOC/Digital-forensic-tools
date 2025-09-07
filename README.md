-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Author: Michał Sołtysik

Cybersecurity Analyst & Consultant | Deep Packet Inspection Analyst | Digital Forensics Examiner | SOC Trainer | CyberWarfare Organizer

Official website: https://michalsoltysik.com/

LinkedIn: https://www.linkedin.com/in/michal-soltysik-ssh-soc/

Cybersecurity content: https://www.youtube.com/playlist?list=PL0RdRWQWldOAAKBqOVEutxKMP-a6CNoLY

Accredible: https://www.credential.net/profile/michalsoltysik/wallet

Credly: https://www.credly.com/users/michal-soltysik

Email: me@michalsoltysik.com

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Originally written in Windows Batch, then rewritten in C# (based on the .NET Framework 4.x).

Compiled into an .exe executable file with an MZ file header.

License: Free for personal and commercial use.

<br>

Tool name: USBWriteBlocker.exe

<br>

Summary:

The application performs the following functions:

(1) runs as a console application requiring administrator privileges to perform system-level operations;
(2) displays console messages with color coding: green for standard information, red for warnings and best practices, blue for status and system feedback;
(3) presents a sequence of educational screens describing the three primary types of data acquisition: cold (performed on a powered-off system), live (performed on a running system), and logical (focused on selected files or partitions rather than the full disk); it also outlines best practices for handling digital evidence and standards and guidelines RFC 3227 and ISO/IEC 27037:2012 concerning digital evidence handling and maintaining the chain of custody;
(4) retrieves a list of all system volumes using WMI (Windows Management Instrumentation) and displays details including drive letter, type (Removable - removable media, Fixed - fixed disk, Network - network drive, CDROM - CD/DVD drive, RAMDisk - RAM disk), filesystem, volume label, size, and free space in gigabytes;
(5) enables management of the Write Protection mechanism for USB devices - this is a Windows feature that prevents writing data to connected USB media and protects their original content from modification; the user can enable, disable, or check the current status of this mechanism;
(6) enforces logging of all actions to a chosen USB drive - the log includes creation time, every user action (enable or disable protection, status check), and precise timestamps; the log file is named using the format usb_write_blocker_log_YYYY-MM-DD_HH-MM.txt, for example usb_write_blocker_log_2025-09-07_18-15.txt;
(7) informs the user that Write Protection changes apply only to newly connected USB devices, while already mounted devices are not affected;
(8) provides safe termination - displays a summary, confirms log saving, allows the user to decide whether to exit, and closes with a 20-second countdown.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
