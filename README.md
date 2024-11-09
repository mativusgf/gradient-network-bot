<h1 align="center">Gradient Network Bot</h1>

<p align="center">
  <img src="https://img.shields.io/badge/python-3.8%2B-blue" alt="Python version">
  <img src="https://img.shields.io/badge/selenium-latest-green" alt="Selenium">
  <img src="https://img.shields.io/badge/undetected--chromedriver-latest-orange" alt="undetected-chromedriver">
</p>

<p align="center">
  An automated bot for farming in the Gradient Network using browser emulation and Chrome extension.
</p>

<h2>📋 Table of Contents</h2>

<ul>
  <li><a href="#-project-description">Project Description</a></li>
  <li><a href="#-project-structure">Project Structure</a></li>
  <li><a href="#-requirements">Requirements</a></li>
  <li><a href="#-installation">Installation</a></li>
  <li><a href="#-configuration">Configuration</a></li>
  <li><a href="#-usage">Usage</a></li>
  <li><a href="#-precautions">Precautions</a></li>
  <li><a href="#-troubleshooting">Troubleshooting</a></li>
  <li><a href="#-contributing">Contributing</a></li>
</ul>

<h2 id="-project-description">🚀 Project Description</h2>

<p>
  Gradient Network Bot is a script designed to automate farming processes in the Gradient Network. It uses Selenium and undetected-chromedriver to emulate multiple Chrome browser instances with an installed extension, allowing interaction with the network without detection.
</p>

<h2 id="-project-structure">📁 Project Structure</h2>

<pre>
gradient-network-bot/
│
├── main.py
├── config.json
├── farm.txt
├── proxy.txt
├── requirements.txt
├── README.md
└── extension/
    └── [Chrome extension files]
</pre>

<ul>
  <li><code>main.py</code>: Main script for running the bot</li>
  <li><code>config.json</code>: Configuration file with bot settings</li>
  <li><code>farm.txt</code>: List of accounts for farming</li>
  <li><code>proxy.txt</code>: List of proxy servers</li>
  <li><code>requirements.txt</code>: Python dependencies</li>
  <li><code>extension/</code>: Directory containing Chrome extension files</li>
</ul>

<h2 id="-requirements">📋 Requirements</h2>

<ul>
  <li>Python 3.8 or higher</li>
  <li>Google Chrome (pre-installed)</li>
  <li>Dependencies listed in <code>requirements.txt</code></li>
</ul>

<h2 id="-installation">⚙️ Installation</h2>

<ol>
  <li>Clone the repository:
    <pre><code>git clone https://github.com/mativusgf/gradient-network-bot.git
cd gradient-network-bot</code></pre>
  </li>
  <li>Install the required dependencies:
    <pre><code>pip install -r requirements.txt</code></pre>
  </li>
  <li>Ensure Google Chrome is installed on your system.</li>
</ol>

<h2 id="-configuration">🔧 Configuration</h2>

<ol>
  <li>Open <code>config.json</code> and set up the bot parameters:
    <pre><code>{
    "num_threads": 5,
    "accounts_file": "farm.txt",
    "proxies_file": "proxy.txt",
    "session_interval": 1200
}</code></pre>
  </li>
  <li>
    Add account credentials to <code>farm.txt</code>, one per line:
    <pre><code>username1:password1
username2:password2</code></pre>
  </li>
  <li>
    Add proxy servers to <code>proxy.txt</code>, one per line:
    <pre><code>http://login:password@ip:port
###or###
socks5://...</code></pre>
  </li>
</ol>

<h2 id="-usage">🖥️ Usage</h2>

<p>Run the bot with the following command:</p>

<pre><code>python main.py</code></pre>

<p>The bot will:</p>
<ol>
  <li>Launch multiple Chrome instances based on the <code>num_threads</code> setting.</li>
  <li>Load accounts from the specified <code>accounts_file</code>.</li>
  <li>Use proxies from the <code>proxies_file</code> for each instance.</li>
  <li>Perform farming actions for each account.</li>
  <li>Maintain sessions for the duration specified by <code>session_interval</code>.</li>
</ol>

<h2 id="-precautions">🔒 Precautions</h2>

<ul>
  <li><strong>NEVER</strong> share your account credentials or private keys.</li>
  <li>Use this bot at your own risk and in compliance with Gradient Network's terms of service.</li>
  <li>Be aware of and respect rate limits to avoid potential account restrictions.</li>
  <li>Use reliable proxies to minimize the risk of detection.</li>
</ul>

<h2 id="-troubleshooting">🔍 Troubleshooting</h2>

<table>
  <tr>
    <th>Issue</th>
    <th>Solution</th>
  </tr>
  <tr>
    <td>Chrome fails to launch</td>
    <td>Ensure Chrome is installed and the path is correct in your system's PATH variable</td>
  </tr>
  <tr>
    <td>Proxy connection issues</td>
    <td>Verify that the proxies in <code>proxy.txt</code> are active and correctly formatted</td>
  </tr>
  <tr>
    <td>Account login failures</td>
    <td>Check the credentials in <code>farm.txt</code> and ensure they are correct and active</td>
  </tr>
</table>

<h2 id="-contributing">👥 Contributing</h2>

<p>Contributions are welcome! To contribute:</p>

<ol>
  <li>Fork the repository</li>
  <li>Create a new branch (<code>git checkout -b feature/amazing-feature</code>)</li>
  <li>Commit your changes (<code>git commit -m 'Add some amazing feature'</code>)</li>
  <li>Push to the branch (<code>git push origin feature/amazing-feature</code>)</li>
  <li>Open a Pull Request</li>
</ol>
