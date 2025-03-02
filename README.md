SubPooky - Advanced Recon & API Security Tool

SubPooky is an advanced reconnaissance and API security tool designed for ethical hackers, penetration testers, and security researchers. It performs subdomain enumeration, live checking, API key hunting, hidden API extraction, directory brute-forcing, parameter fuzzing, and header security analysis.

Features

Subdomain Enumeration: Collects subdomains from multiple sources.

Live Subdomain Checking: Identifies active subdomains.

API Key Hunting: Scans for exposed API keys in responses.

Hidden API Extraction: Detects private and hidden API endpoints.

Directory Brute-Forcing: Discovers common directories on live domains.

Parameter Fuzzing: Identifies potentially vulnerable GET parameters.

Header Security Analysis: Checks for misconfigurations in HTTP headers.

Installation

# Clone the repository
git clone https://github.com/root60/SubPooky.git
cd SubPooky

# Install dependencies
pip install -r requirements.txt

Usage

python subpooky.py <target-domain>

Example:

python subpooky.py example.com

Output

SubPooky generates several output files containing the scan results:

subdomains.txt - List of discovered subdomains

live_subdomains.txt - List of active subdomains

api_keys.txt - Exposed API keys found

hidden_apis.txt - Discovered hidden API endpoints

directories.txt - Identified directories

vulnerable_params.txt - Potentially vulnerable parameters

header_issues.txt - Security misconfigurations in headers

Dependencies

Python 3.x

httpx

tqdm

colorama

dns.resolver

Install missing dependencies with:

pip install -r requirements.txt

Disclaimer

This tool is intended for educational and ethical hacking purposes only. Use it responsibly and ensure you have permission to scan any domain.

License

This project is open-source and available under the MIT License.
