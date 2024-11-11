PRODIGY_CS_05
Packet Sniffer
This project is a simple packet sniffer written in C++ using the libpcap library. It captures network packets from a specified interface, analyzes them, and displays important details like source/destination IP addresses, ports, protocol, and the packet payload in hexadecimal format.

Features Captures live network traffic on a specified device. Supports IP, TCP, and UDP packet analysis. Displays source and destination IP addresses and ports. Extracts and displays the packet payload (if available). Requirements libpcap (Packet capture library) g++ (C++ compiler) Installation Installing Dependencies on Linux On Ubuntu/Debian: bash Copy code sudo apt-get install libpcap-dev On Fedora/RHEL: bash Copy code sudo dnf install libpcap-devel Compilation To compile the program, use the following command in your terminal:

bash Copy code g++ -o packet_sniffer packet_sniffer.cpp -lpcap Running the Program Run the program with sudo to capture packets: bash Copy code sudo ./packet_sniffer The program will start capturing live traffic and display packet details on the default network device. Example Output The program will output details like:

Source IP: 192.168.0.10 Destination IP: 192.168.0.1 Protocol: TCP Payload in hexadecimal. Troubleshooting Permission issues: Ensure the program is run with sudo. Missing dependencies: Install libpcap-dev if not already installed. No packets captured: Check that the network interface is active and there is network traffic.
