# Installing Qiskit and JupyterLab on Raspberry Pi 5

This guide will walk you through the process of installing Qiskit and JupyterLab on a Raspberry Pi 5. These instructions are suitable for a fresh installation on a Raspberry Pi running the latest version of Raspberry Pi OS.

## Prerequisites

- Raspberry Pi 5 with Raspberry Pi OS installed
- Internet connection
- Terminal access (either directly or via SSH)

## Installation Steps

1. Update your system:

   ```bash
   sudo apt update
   sudo apt upgrade -y
   ```

2. Install Python3 virtual environment:

   ```bash
   sudo apt install python3-venv
   ```

3. Create a new directory for your project:

   ```bash
   mkdir qiskit_project
   cd qiskit_project
   ```

4. Create a new Python virtual environment:

   ```bash
   python3 -m venv qiskit_env
   ```

5. Activate the virtual environment:

   ```bash
   source qiskit_env/bin/activate
   ```

6. Install JupyterLab:

   ```bash
   pip install jupyterlab
   ```

7. Install scientific Python packages:

   ```bash
   pip install numpy scipy matplotlib pandas
   ```

8. Install Qiskit:

   ```bash
   pip install qiskit
   ```

9. Install Qiskit IBM Runtime:

   ```bash
   pip install qiskit-ibm-runtime
   ```

10. Install Qiskit Visualization (for Jupyter notebooks) assuming using zsh shell:

    ```bash
    pip install 'qiskit[visualization]'
    ```

## Running JupyterLab

To start JupyterLab, ensure your virtual environment is activated, then run:

```bash
jupyter lab --no-browser 
```

This will start the JupyterLab server and open a new tab in your default web browser. Here, instead of web browser, I used Visual Studio to connect Pi 5 server via SSH.

## Notes

- If you're using a Zsh terminal instead of Bash, the activation command remains the same.
- You may need to install additional dependencies if you encounter any errors during the installation process.
- It's recommended to use this setup within the virtual environment to avoid conflicts with system-wide Python packages.

## Troubleshooting

If you encounter any issues with the installation:

1. Ensure your Raspberry Pi OS is up to date.
2. Check that you have sufficient free space on your SD card or storage device.
3. If you encounter permission errors, make sure you're not running pip with sudo inside the virtual environment.

For further assistance, consult the official Qiskit and JupyterLab documentation or seek help in their respective community forums.
