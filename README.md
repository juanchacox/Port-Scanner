<h1>Port Scanner in Python</h1>
    <p>This is a basic <strong>port scanner</strong> developed in Python using the <code>nmap</code> library. The script allows you to scan a specific IP address across a range of ports, identifying the services running, the software version, and obtaining additional information about open ports.</p>
    
    <h2>Features</h2>
    <ul>
        <li>Port scanning using Nmap.</li>
        <li>Support for service and version detection.</li>
        <li>Fast and stealthy SYN scan.</li>
        <li>Operating system detection.</li>
        <li>Identification of products and services with extra information.</li>
    </ul>
    
    <h2>Requirements</h2>
    <p>Before running the script, make sure you have the following components installed:</p>
    <ul>
        <li><strong>Python 3.x</strong>: You can download it from <a href="https://www.python.org/downloads/">here</a>.</li>
        <li><strong>Nmap</strong>: You must have Nmap installed on your system. You can download it from <a href="https://nmap.org/download.html">here</a>.</li>
        <li><strong>python-nmap</strong>: Python library to interact with Nmap. You can install it by running:
            <pre><code>pip install python-nmap</code></pre>
        </li>
    </ul>
    
    <h2>Usage</h2>
    <ol>
        <li>Clone this repository or download the files.
            <pre><code>git clone https://github.com/your-username/repository-name.git
cd repository-name</code></pre>
        </li>
        <li>Run the <code>port_scanner.py</code> script with administrator privileges to get accurate results:
            <pre><code>sudo python port_scanner.py</code></pre>
        </li>
        <li>The script scans the specified IP address (in this example, GitHub) for the first 1024 ports and displays the results on the screen.</li>
    </ol>
    
    <h3>Example Usage</h3>
    <p>The following command performs a SYN scan (<code>-sS</code>) on the IP address <code>140.82.116.3</code> (a GitHub server), checking ports 1 to 1024, detecting versions and services, and obtaining additional information:</p>
    <pre><code>scaner.scan('140.82.116.3', '1-1024', '-v -sS -sV -sC -A -O')</code></pre>
    
    <h3>Expected Output</h3>
    <pre><code>
[+] Host: 140.82.116.3
[+] Port: http
[+] Name: open
[+] Version: Apache 2.4.41
[+] Product: Apache HTTPD
[+] Extra Information: Ubuntu</code></pre>
    
    <h2>Legal Considerations</h2>
    <p>Port scanning without authorization may be <strong>illegal</strong> in some countries or violate the terms of service of websites. Be sure to have <strong>explicit permission</strong> before scanning any network or server that you do not own.</p>
    
    <h2>Contributions</h2>
    <p>If you wish to contribute to this project, feel free to create a <strong>Pull Request</strong> or open an <strong>Issue</strong> to discuss new ideas or report bugs.</p>
