
---

# Network Troubleshooter

A Python script to troubleshoot network connectivity issues by performing ping tests, port scans, and traceroutes.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)


## Installation

Follow these steps to set up the project on your local machine.

### Prerequisites

Ensure you have the following installed on your machine:

- Python 3.6+
- `pip` (Python package installer)
- `git` (version control system)

### Steps

1. **Clone the repository**:

    Open your terminal and run:
    ```sh
    git clone https://github.com/yourusername/network-troubleshooter.git
    cd network-troubleshooter
    ```

2. **Create a virtual environment**:

    This step is optional but recommended to avoid dependency conflicts.
    ```sh
    python3 -m venv venv
    source venv/bin/activate   # For MacOS/Linux
    # .\venv\Scripts\activate  # For Windows
    ```

3. **Install dependencies**:

    Run the following command to install the required Python packages:
    ```sh
    pip install -r requirements.txt
    ```

    If you don't have a `requirements.txt` file yet, you can create one with the following content:
    ```plaintext
    ping3
    scapy
    ```

## Usage

After setting up the environment and installing the dependencies, you can run the script.

1. **Run the script**:

    In the terminal, navigate to the project directory and execute:
    ```sh
    python network_troubleshooter.py
    ```

2. **Input the target host**:

    When prompted, enter the hostname or IP address you want to test. The script will perform the following actions:
    - **Ping Test**: Check if the target is reachable.
    - **Port Scan**: Check if specific ports (22, 80, 443) on the target are open.
    - **Traceroute**: Perform a traceroute to identify where the connection is failing.

### Example

```sh
Enter the host to test: example.com
example.com is reachable. Ping time: 0.023 seconds
Port 22: Closed
Port 80: Open
Port 443: Open
Traceroute:
  1 192.168.1.1  0.438 ms
  2 10.0.0.1    10.567 ms
  

---

Copy and paste this content into a `README.md` file in your project directory. This will help users understand how to set up, use, and contribute to your network troubleshooter project.
