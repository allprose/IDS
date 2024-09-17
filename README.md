Intrusion Detection System (IDS)
The Intrusion Detection System (IDS) is a Python-based tool that monitors network traffic in real-time for suspicious activity. It detects SYN floods, ICMP floods, and multiple connection attempts, logging all intrusions in a log file. The tool is cross-platform and works on Windows, macOS, and Linux systems.

Key Features:
SYN Flood Detection: Monitors for excessive SYN packets, indicating potential SYN flood attacks.
ICMP Flood Detection: Detects excessive ICMP packets, which could indicate an ICMP flood (e.g., ping flood attacks).
Multiple Connection Attempt Detection: Monitors for brute force attempts or DoS attacks by tracking the number of connection attempts from a single IP.
Logging: All detected intrusions are logged in a file with timestamps and detailed information about each attack.
Automatic Dependency Installation: If the required dependencies are not installed, the tool will install them automatically.
Requirements:
Python 3.x
Scapy (automatically installed by the script)
Root/Administrator privileges for packet sniffing.
How to Run:
Download the script and save it as ids.py.

Run the script:

Linux/macOS (requires root privileges):
sudo python3 ids.py
Windows (requires Administrator privileges):
python ids.py
The script will automatically install dependencies like Scapy if they are missing.

Log Files:
Each IDS session will generate a log file named ids_log_YYYYMMDD_HHMMSS.log, where:

YYYYMMDD is the date of the scan.
HHMMSS is the timestamp when the IDS session started.
The log files contain detailed information about each detected intrusion, including the time of detection and the source IP address.

Author EY