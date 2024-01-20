# HA Proxy Tunneler

`HA Proxy Tunneler` alias `ha-proxy` is a script designed to streamline the configuration and management of proxy tunnels, leveraging HA Tunnel Plus for services like HTTP, Git, VSCode, and SSH. 🖧

**Version: 1.0.0**

> **Disclaimer:** This documentation is provided for informational purposes only. Use this script responsibly and at your own risk. The author is not responsible for any misuse or damage caused by the script.

---

## 📌 Install

Run the following command to install ha-proxy in your machine (Linux only):

```bash
curl https://raw.githubusercontent.com/RajaRakoto/ha-proxy/master/setup > setup && chmod +x setup && ./setup
```

---

## 📌 Features

### 📜 Start Proxy Configuration

```bash
ha-proxy --start
```

Starts automatic proxy configuration for HTTP, Git, VSCode, and SSH.

### 📜 Stop Proxy Configuration

```bash
ha-proxy --stop
```

Unsets all proxy configurations.

### 📜 Check Current Proxy Status

```bash
ha-proxy --status
```

Displays the current status of proxy configurations.

### 📜 Restart Proxy Configuration

```bash
ha-proxy --restart
```

Restarts proxy configuration by stopping and then starting it.

### 📜 Copy Proxy Information to Clipboard

```bash
ha-proxy --clip
```

Copies proxy server information to the clipboard.

### 📜 Check for Required Variables and Dependencies

```bash
ha-proxy --check
```

Checks for required variables and dependencies.

### 📜 Set Environment Variables

```bash
ha-proxy --env
```

Sets environment variables using a text editor.

### 📜 Generate New SSH Key

```bash
ha-proxy --ssh
```

Generates a new SSH (private|public) key.

### 📜 Display Script Version Information

```bash
ha-proxy --version
```

Displays script version information.

### 📜 Display Help Message

```bash
ha-proxy --help
```

Displays a help message with usage examples.

---

## 📌 Notes

- Make sure to set the required environment variables in the `$HOME/.ha_env` file.
- Ensure that the necessary dependencies `akory`, `xxd`, `jq`, `git`, `xclip`, `corkscrew`, `gedit` are installed.
