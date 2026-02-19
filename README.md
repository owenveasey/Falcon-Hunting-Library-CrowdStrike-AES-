🦅 Falcon-Hunting-Library (CrowdStrike AES)
This repository contains high-fidelity Advanced Event Search (AES) queries for CrowdStrike Falcon, organized by the MITRE ATT&CK® Framework.
🎯 What is MITRE ATT&CK?
MITRE ATT&CK is a globally accessible knowledge base of adversary tactics and techniques based on real-world observations. Instead of looking for "bad files," these queries look for bad behaviors across the different stages of an attack:

Initial Access: How they get in (e.g., Phishing).

Execution: Running the malicious code.

Persistence: Staying in the system after a reboot.

Defense Evasion: Hiding from security tools.

Discovery: Exploring the network.

Exfiltration: Stealing the data.

🛠️ How to Use These Queries
Each folder in this library corresponds to a specific MITRE phase. To use them:

Select a Tactic: Choose the folder for the phase you want to hunt in (e.g., 01_Initial_Access).

Copy the Query: Open the .fql file and copy the code.

Run in Falcon: * Log into your CrowdStrike Falcon Console.

Navigate to Investigate > Advanced Event Search.

Paste the query and adjust the time range (e.g., Last 24 hours or Last 7 days).

Tune the Results: I have included // --- NOISE FILTERING --- sections in the queries. You may need to add your own company’s safe software to these filters to "zero in" on real threats.

🚀 Key Highlights
Behavioral Detection: Catches 0-day threats that traditional Antivirus misses.

Noise-Canceled: Pre-tuned to filter out common enterprise "noise" like Slack, Teams, and Microsoft updates.

Incident Tested: Includes the specific logic used to successfully identify a real-world "ClickFix" malware attempt.
