# Cisco Automation Project

This project automates various tasks using Cisco's DNA Center and Meraki APIs through Ansible playbooks and modules.

## Project Structure

## Setup

1. **Clone the repository:**
    ```sh
    git clone <repository-url>
    cd cisco-automation
    ```

2. **Set up the virtual environment:**
    ```sh
    python -m venv myenv
    source myenv/Scripts/activate  # On Windows
    source myenv/bin/activate      # On Unix or MacOS
    ```

3. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

## Configuration

1. **Ansible Configuration:**
    - Update `ansible.cfg` with your specific configurations.
    - Update `inventory.ini` with your inventory details.

2. **Environment Variables:**
    - Set up necessary environment variables for Cisco DNA Center and Meraki API keys.

## Usage

1. **Verify Connectivity:**
    ```sh
    ansible-playbook playbooks/01_verify_connectivity.yml
    ```

2. **Basic Configuration:**
    ```sh
    ansible-playbook playbooks/02_basic_config.yml
    ```

3. **VLAN Configuration:**
    ```sh
    ansible-playbook playbooks/03_vlan_config.yml
    ```

4. **Backup Configuration:**
    ```sh
    ansible-playbook playbooks/04_backup_config.yml
    ```

## Documentation

- [Network Diagram](documentation/network_diagram.md)
- [Testing Results](documentation/testing_results.md)