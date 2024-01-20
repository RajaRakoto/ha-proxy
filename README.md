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

**📜 Start proxy configuration**: Starts automatic proxy configuration for HTTP, Git, VSCode, and SSH.

```bash
ha-proxy --start
```

**📜 Stop proxy configuration**: Unsets all proxy configurations.

```bash
ha-proxy --stop
```

**📜 Check current proxy status**: Displays the current status of proxy configurations.

```bash
ha-proxy --status
```

**📜 Restart proxy configuration**: Restarts proxy configuration by stopping and then starting it.

```bash
ha-proxy --restart
```

**📜 Copy proxy information**: Copies proxy server information to the clipboard.

```bash
ha-proxy --clip
```

**📜 Check script**: Checks for required variables and dependencies.

```bash
ha-proxy --check
```

**📜 Set env variables**: Sets environment variables using a text editor.

```bash
ha-proxy --env
```

**📜 Generate new SSH key**: Generates a new SSH (private|public) key.

```bash
ha-proxy --ssh
```

**📜 Display script version**: Display current version of ha-proxy

```bash
ha-proxy --version # or -v
```

**📜 Display help message**: Displays a help message with usage examples.

```bash
ha-proxy --help # or -h
```

---

## 📌 Notes

- Make sure to set the required environment variables in the `$HOME/.ha_env` file.
- Ensure that the necessary dependencies `akory`, `xxd`, `jq`, `git`, `xclip`, `corkscrew`, `gedit` and `bat` are installed.
