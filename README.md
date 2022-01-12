
# Uptime-Kuma deployment with Ansible and Docker-Compose

Uptime-Kuma is a open source, lightweight (but powerful), self-hosted monitoring tool. 

## Tested with: 

| Environment | Application | Version  |
| ----------------- |-----------|---------|
| WSL2 Ubuntu 20.04 | Ansible | v2.9.6 |

## Prerequisites. 

# Prerequisite:

Install [sshpass](https://linux.die.net/man/1/sshpass) and [Ansible](https://www.ansible.com/).

Ubuntu:
```bash
sudo apt-get install sshpass && sudo apt-get install ansible -y
```

macOS:
```bash
# Ansible:
CFLAGS=-Qunused-arguments CPPFLAGS=-Qunused-arguments pip install --user ansible

# sshpass
brew install hudochenkov/sshpass/sshpass
```

## Deployment How-To:

1. Clone this repository to your local machine.
2. cd into the project folder.
3. Edit vars.yml adding your server IP and User.
4. Make install.sh executable. 

    ```bash
    chmod +x install.sh
    ```
4. Run it.
    ```bash
    ./install.sh
    ```
5. Go to: http://YourServerIP:3001

## Author:

- [@JManzur](https://jmanzur.com.ar)

## Documentation:

- [Uptime-Kuma Official Repository](https://github.com/louislam/uptime-kuma)