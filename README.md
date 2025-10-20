# local_network_port_scan(elevate_labs)TASK1-

TASK OBJECTIVE:The task is to perform network reconnaissance on your local network by using the tool Nmap to conduct a TCP SYN port scan. The objective is to discover active devices and their open ports to understand your network's security exposure. The outcome requires you to analyze the scan results, identify the services running on those open ports.

METHODOLOGY:
This task utilized industry-standard tools and techniques for fundamental network reconnaissance to understand the exposure of local devices. The process was executed on a Windows operating system using the Nmap command-line utility.

1. Initial Host and Range Identification:-
To establish the boundaries for the scan,                                   
Tool Used: Windows Command Prompt (ipconfig)                               
Action: Identified the host's IP address (e.g., 192.168.1.10) to deduce the local network range (e.g., 192.168.1.0/24).

2. TCP SYN Scan Execution (Port Scanning):-
A TCP SYN scan was performed across the entire local subnet to identify active hosts and their open TCP ports.                             
Tool Used: Nmap (Network Mapper)
Command: nmap -sS 192.168.1.0/24 -oA local_network-scan                                    
Result: Generated the raw data files (local_network_scan.nmap, .xml, etc.) containing the state of the top 1000 common TCP ports for all active devices.

3. Data Analysis and Risk Assessment:-
The saved raw Nmap output (.nmap file) was examined to compile a definitive list of open ports and corresponding services for each active IP address.                          
Action: Used online resources(Goggle, DuckDuckGo) to research the common service associated with each open port (e.g., FTP on port 21, HTTP on port 80).                                
Risk Assessment: Based on the discovered services, a search was conducted to identify and document the potential security risks (e.g., clear-text passwords, known vulnerabilities, brute-force targets) associated with having those specific ports open and accessible.
