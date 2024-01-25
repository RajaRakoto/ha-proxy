# HA Proxy Tunneler

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/for-you.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-git.svg)](https://forthebadge.com) [![forthebadge](https://github.com/RajaRakoto/github-docs/blob/master/badge/build-by.svg?raw=true)](https://forthebadge.com) 

![Git](https://img.shields.io/badge/-Git-777?style=flat&logo=git&logoColor=F05032&labelColor=ffffff) ![Gitub](https://img.shields.io/badge/-Gitub-777?style=flat&logo=github&logoColor=777&labelColor=ffffff)

`HA Proxy Tunneler` alias `ha-proxy` is a script designed to streamline the configuration and management of proxy tunnels, leveraging HA Tunnel Plus for services like HTTP, Git, VSCode, and SSH. 🖧

**Version: 1.1.5**

> **Disclaimer:** This documentation is provided for informational purposes only. Use this script responsibly and at your own risk. The author is not responsible for any misuse or damage caused by the script.

---

## 📌 Install

Run the following command to install ha-proxy in your machine (Linux only):

```bash
curl https://raw.githubusercontent.com/RajaRakoto/ha-proxy/master/setup > setup && chmod +x setup && ./setup
```

To uninstall ha-proxy:

```bash
sudo rm -r "$HOME/.ha_env" /usr/local/bin/ha-proxy && echo "ha-proxy uninstallation ... [done]"
```

---

## 📌 Features

```bash
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

**📜 Copy proxy information**: Copies proxy information to the clipboard.

```bash
ha-proxy --getProxy
```

**📜 Copy encoded proxy information**: Copies encoded proxy information to the clipboard.

```bash
ha-proxy --getProxyEncoded
```

**📜 Copy proxy server information**: Copies proxy server information to the clipboard.

```bash
ha-proxy --getProxyServer
```

**📜 Copy encoded proxy server information**: Copies encoded proxy server information to the clipboard.

```bash
ha-proxy --getProxyServerEncoded
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

**📜 Fix env file**: Repair .ha_env file by regenerating it again in your home.

```bash
ha-proxy --fix
```

**📜 Display script version**: Display the current version of ha-proxy.

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
