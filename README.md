 <h1 align="center">Port Scanner in Python</h1>

This is a basic **port scanner** developed in Python using the `nmap` library. The script allows you to scan a specific IP address across a range of ports, identifying the services running, the software version, and obtaining additional information about open ports.

## Features

- Port scanning using Nmap.
- Support for service and version detection.
- Fast and stealthy SYN scan.
- Operating system detection.
- Identification of products and services with extra information.

## Requirements

Before running the script, make sure you have the following components installed:

- **Python 3.x**: You can download it from [here](https://www.python.org/downloads/).
- **Nmap**: You must have Nmap installed on your system. You can download it from [here](https://nmap.org/download.html).
- **python-nmap**: Python library to interact with Nmap. You can install it by running:
  pip install python-nmap

## Usage

1. Clone this repository or download the files.
   git clone https://github.com/juanchacox/Port-Scanner.git
   cd repository-name

2. Run the `port_scanner.py` script with administrator privileges to get accurate results:
   sudo python port_scanner.py

3. The script scans the specified IP address (in this example, GitHub) for the first 1024 ports and displays the results on the screen.

### Example Usage

The following command performs a SYN scan (`-sS`) on the IP address `140.82.116.3` (a GitHub server), checking ports 1 to 1024, detecting versions and services, and obtaining additional information:

scaner.scan('140.82.116.3', '1-1024', '-v -sS -sV -sC -A -O')

The output will show:
- Scanned host.
- Open ports and their states.
- Services and versions.
- Extra information if available.

### Expected Output


* Host: 140.82.116.3
- [+] Port: http
- [+] Name: open
- [+] Version: Apache 2.4.41
- [+] Product: Apache HTTPD
- [+] Extra Information: Ubuntu


## Legal Considerations

Port scanning without authorization may be **illegal** in some countries or violate the terms of service of websites. Be sure to have **explicit permission** before scanning any network or server that you do not own.

## Contributions

If you wish to contribute to this project, feel free to create a **Pull Request** or open an **Issue** to discuss new ideas or report bugs.
