Useful scripts while completing CTFs on various platforms

# CVE-2021-43798
This Python script automates the exploitation of a Grafana directory traversal vulnerability, allowing for the extraction of user hashes from the Grafana database. The extracted hashes are converted into a format compatible with Hashcat for password cracking.

## Features

- Exploits the Grafana CVE to download the `grafana.db` file.
- Extracts user credentials (login, password hashes, and salts).
- Converts hashes into a Hashcat-compatible format.
- Streamlined one-click operation.

## Prerequisites

- Python 3.x
- sqlite3
- `curl` command-line tool
- Required Python libraries: `argparse`, `requests`

## Usage
`python3 grafana_exploit.py <TARGET_IP> --port <TARGET_PORT>`

## Credit
- Thanks to Persees for the decoding function
https://github.com/persees/grafana_exploits/blob/main/decoder.py
