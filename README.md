# 🛡️ Guardian Shield - An Advanced Blue Team Platform

Guardian Shield is a comprehensive, cross-platform graphical user interface (GUI) application designed for blue teams and cybersecurity professionals. It centralizes a wide range of open-source security tools into a single, intuitive platform, streamlining defensive tasks from network monitoring and log analysis to incident response and digital forensics.

## ✨ Features

  - **Integrated Tool Suite:** Access a variety of powerful command-line tools for reconnaissance, network monitoring, endpoint security, forensics, and more, all from a unified interface.
  - **Efficient Task Management:** Run multiple commands simultaneously without freezing the application, thanks to multithreading.
  - **Centralized Logging:** All command outputs are streamed to a single, searchable log.
  - **Process Control:** Monitor the status of all running tasks and terminate them as needed.
  - **Automated Tool Installation:** Guardian Shield can automatically detect and install missing command-line tools on your system (requires `sudo` and a supported package manager).
  - **Case Management:** Create and save detailed notes for your investigations directly within the application, stored in a local SQLite database.
  - **Professional Reporting:** Generate a clean, professional PDF report of your analysis with a single click.
  - **AbuseIPDB Integration:** Right-click on any IP address in the output log to instantly check its reputation via the AbuseIPDB API.
  - **Customizable UI:** Choose between a modern dark theme and a classic light theme.

## 📦 Installation

\<p align="center"\>
\<img src="[https://i.imgur.com/your-image-id.png](https://www.google.com/search?q=https://i.imgur.com/your-image-id.png)" alt="Guardian Shield Screenshot" width="800"\>
\</p\>

Guardian Shield requires Python 3 and several libraries.

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/anjanl0g/guardian-shield.git
    cd guardian-shield
    ```

2.  **Create and activate a virtual environment:**

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the dependencies:**

    ```bash
    pip3 install PyQt5 requests fpdf shlex or
    pip3 install -r requirements.txt
    ```

4.  **Run the application:**

    ```bash
    python3 blueteam.py
    ```

**Note:** For some tools like `nmap`, `lynis`, or `rkhunter`, you may need to install them via your system's package manager if the auto-installer fails.

## 🛠️ Usage

The application is organized into several tabs, each corresponding to a different domain of blue teaming:

  - **Info Gathering & Recon:** For initial reconnaissance and host discovery.
  - **Network Monitoring:** For live packet analysis and network scans.
  - **Log Analysis:** For searching and filtering system logs.
  - **Endpoint Security:** For auditing system configurations and checking for rootkits.
  - **Incident Response:** For analyzing live processes and network connections.
  - **Forensics:** For digital forensics tasks using tools like Volatility and The Sleuth Kit.
  - **Vulnerability Scanning:** For scanning systems and web applications for weaknesses.
  - **Cloud & Container Security:** For security checks in cloud environments and container images.
  - **Settings:** To manage themes and API keys.
  - **Case Management:** To save and load case-specific notes.

To run a command:

1.  Navigate to the relevant tab.
2.  Select the desired command variant from the dropdown menu.
3.  Fill in any required arguments in the text box (e.g., `<target_range>`, `<domain>`).
4.  Click the **Run** button.

## 📝 Configuration

  - **API Keys:** To use the AbuseIPDB feature, go to the **Settings** tab and enter your API key.
  - **Themes:** Change the application's appearance between dark and light mode in the **Settings** tab.

## 🤝 Contributing

Contributions are welcome\! If you have suggestions for new features, bug reports, or want to contribute code, please open an issue or a pull request.

## 📄 License

This project is licensed under the MIT License.
