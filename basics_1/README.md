# Network Basics 1

This directory contains scripts for configuring network settings on Ubuntu servers.

## Files

- **0-change_your_home_IP**: Bash script that configures the `/etc/hosts` file to:
  - Make `localhost` resolve to `127.0.0.2` (instead of the default `127.0.0.1`)
  - Make `facebook.com` resolve to `8.8.8.8`

## Usage

Run the script with sudo privileges:

```bash
sudo ./0-change_your_home_IP
```

**Warning**: If you're running this script on a machine that you'll continue to use, be sure to revert `localhost` back to `127.0.0.1` after testing, otherwise many services may stop working.

## Topics Covered

- Hosts file configuration (`/etc/hosts`)
- DNS resolution and hostname mapping
- Network configuration on Ubuntu servers

