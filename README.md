# SubPooky Finder


![SubPooky Finder](Capture.png)

## Overview
SubPooky Finder is an advanced reconnaissance tool for discovering subdomains, extracting hidden APIs, detecting vulnerabilities, and hunting for API keys on a given target domain. The tool is designed for security researchers and penetration testers to enhance their reconnaissance capabilities.

## Features
- **Subdomain Discovery**: Gathers subdomains from multiple sources.
- **Live Subdomain Checking**: Identifies active subdomains.
- **API Key Hunting**: Searches for exposed API keys.
- **Hidden API Extraction**: Detects potential hidden/private API endpoints.
- **Directory Brute-Forcing**: Finds common directories on discovered subdomains.
- **Parameter Fuzzing**: Identifies vulnerable URL parameters.
- **Header Vulnerability Scanning**: Checks for missing security headers.
- **Asynchronous Execution**: Fast and efficient scanning with asyncio.

## Installation
### Prerequisites
- Python 3.8+
- `pip` package manager

### Install Dependencies
```sh
pip install -r requirements.txt
```

## Usage
Run the tool with a target domain:
```sh
python subpooky.py example.com
```

### Command-Line Arguments
- `domain` - The target domain to scan.

## Output
The tool generates multiple output files:
- `subdomains.txt` - List of discovered subdomains.
- `live_subdomains.txt` - List of active subdomains.
- `api_keys.txt` - Exposed API keys found.
- `hidden_apis.txt` - Hidden API endpoints.
- `directories.txt` - Discovered directories.
- `vulnerable_params.txt` - Parameters vulnerable to injection.
- `header_issues.txt` - Security header misconfigurations.

## Example Run
```sh
python subpooky.py example.com
```
Expected Output:
```
[+] Subdomains Found:
  - api.example.com
  - dev.example.com
[+] Live Subdomains:
  - api.example.com
[+] API Keys Discovered:
  - http://api.example.com: API_KEY_12345
...
```

## Disclaimer
This tool is intended for educational and security research purposes only. Unauthorized use on systems without permission is prohibited.

## License
MIT License

## Author
Developed by RedHydra.
