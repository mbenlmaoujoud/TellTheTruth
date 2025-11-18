# TellTheTruth

TellTheTruth is a quick CLI helper that queries public feeds for CVEs and exploit references for a given technology and version.

## Requirements
- Python 3.8+
- Packages: `requests`, `termcolor`, `pyExploitDb`, `beautifulsoup4`
- Optional: `searchsploit` on your PATH for Exploit-DB lookups

Install the Python deps with:
```bash
pip install requests termcolor pyExploitDb beautifulsoup4
```

## Usage
Run the script and provide the product name and version when prompted:
```bash
python3 tellMe.py
```
The tool fetches matching CPEs from NVD, prints CVE details (severity, CWE, summary), and surfaces public exploit references from GitHub, Exploit-DB, Packet Storm, and marc.info when available.

## Notes
- Network access is required; API rate limits may apply.
- Results are for triage only—verify findings before acting on them.
