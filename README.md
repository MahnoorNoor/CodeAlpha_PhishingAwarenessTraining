## Basic Network Sniffer (Task 1)

Files:
- `simple_sniffer.py` : Python sniffer script (Scapy-based).
- `sniff_output.txt` : Sample console output from a sniffing session.
- `capture.pcap` : (Optional) Saved packet capture file (open in Wireshark).
- `analysis_sniffer.py` : Script to summarize captured traffic by protocol.
- `sniffer_analysis.txt` : Result of the analysis script (protocol counts).

Summary:
A simple Python program that captures and analyzes network packets. It displays source/destination IPs, protocol type (TCP/UDP), and a preview of packet payloads. An additional script summarizes the captured packets by protocol count.

How to run:
1. Install Scapy  
   - On Kali/Linux: `sudo apt install python3-scapy`  
   - Or inside venv: `pip install scapy`
2. Capture packets and save output:  
   `sudo python3 simple_sniffer.py 50 > sniff_output.txt`
3. (Optional) Save a `.pcap` file:  
   `sudo python3 simple_sniffer.py 0 wlan0 capture.pcap`
4. Analyze protocol counts:  
   `python3 analysis_sniffer.py capture.pcap > sniffer_analysis.txt`

---

