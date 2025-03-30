# VirusCheckerPy
A simple Python Script Using VirusTotal API 
VirusTotal Integration: Uses VirusTotal API for malware detection (requires API key)

Multiple Hashes: Calculates MD5, SHA-1, and SHA-256 hashes

Quarantine: Moves detected malware to a quarantine directory instead of deleting

Behavior Analysis: Basic check for suspicious file attributes

Real-time Monitoring: Uses watchdog to monitor directory changes

File Type Scanning: Focuses on suspicious file extensions

Logging: Comprehensive logging to file

To use:
bash
# Regular scan
python malware_scanner.py /path/to/scan

# Real-time monitoring
python malware_scanner.py /path/to/scan --realtime


Requirements:
pip install requests watchdog


Notes:
Replace "YOUR_VIRUSTOTAL_API_KEY" with a real VirusTotal API key

VirusTotal API has rate limits (free tier: 500 requests/day)

Behavior analysis is basic and could be expanded with more sophisticated checks

Real-time monitoring requires the script to keep running

Quarantine directory is created in the script's working directory

This is still a simplified version compared to commercial antivirus software but provides a robust foundation for malware detection and handling.

