# DRADON

## Overview

**MADE BY DRADE - DRADON** is a comprehensive script designed for advanced penetration testing. It automates the discovery of sensitive information about a website, including subdomains, technologies, HTTP headers, SSL/TLS configurations, directories, and hidden fields.

## Features

- **Subdomain Enumeration**: Identify subdomains using `subfinder` and `assetfinder`.
- **Technology Identification**: Detect technologies used by the website with `whatweb`.
- **HTTP Header Analysis**: Retrieve and analyze HTTP headers using `curl`.
- **SSL/TLS Configuration Analysis**: Scan for SSL/TLS vulnerabilities using `sslscan`.
- **Directory and File Bruteforcing**: Perform directory and file bruteforcing with `dradon`.
- **HTML Comments and Hidden Fields Extraction**: Extract comments and hidden fields from the website's HTML.
- **Sensitive File Detection**: Check for the presence of potentially sensitive files.

## Requirements

The script requires the following tools to be installed:

- `curl`
- `grep`
- `sed`
- `awk`
- `whatweb`
- `dradon`
- `sslscan`
- `assetfinder`

Ensure these tools are installed before running the script. You can install them using your package manager or from their respective repositories.

## Installation

1. **Clone the Repository**

   Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   cd yourrepository
   ```

2. **Make the Script Executable**

   Give execute permissions to the script:

   ```bash
   chmod +x comb.sh
   ```

## Usage

Run the script with the following command:

```bash
./comb.sh
```

You will be prompted to enter the following information:

- **Target Domain**: The domain to analyze (e.g., example.com).
- **Target URL**: The URL to analyze (e.g., https://example.com).
- **Path to Wordlist**: The path to the directory/file bruteforcing wordlist (e.g., common.txt).

The script will generate a report file with the results of the analysis.

## Report

The results are saved in a report file with a timestamp, containing sections for each type of discovery:

- Subdomain Enumeration
- Technology Identification
- HTTP Header Analysis
- SSL/TLS Configuration Analysis
- Directory and File Bruteforcing
- HTML Comments and Hidden Fields
- Sensitive File Detection

## Example

```bash
./comb.sh
Enter the target domain (e.g., example.com): example.com
Enter the target URL (e.g., https://example.com): https://example.com
Enter the path to the directory/file bruteforcing wordlist (e.g., common.txt): common.txt
```

