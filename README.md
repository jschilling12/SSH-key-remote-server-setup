# 🐧 Remote Linux Server Setup & SSH Configuration

This guide walks you through setting up a remote Linux server, configuring SSH key authentication, and simplifying connections using an SSH config file.

https://roadmap.sh/projects/ssh-remote-server-setup

---

## 1️⃣ Register and Set Up a Remote Linux Server

Create a remote Linux server on any cloud provider.

- **Recommended:** [DigitalOcean Droplet](https://www.digitalocean.com/)
- **Alternative Providers:** AWS EC2, Google Cloud, Azure, etc.

> 💡 *DigitalOcean offers free credits for new users — perfect for testing this setup.*

---

## 2️⃣ Create and Add SSH Keys

Generate **two new SSH key pairs** and add both public keys to your remote server.

- 🔗 [Create SSH Keys with PuTTY](https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/create-with-putty/)
- 🔗 [Add SSH Keys to a DigitalOcean Droplet](https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/)

---

## 3️⃣ Connect to the Server via SSH

Once your keys are added, verify that both can connect successfully.

```bash
ssh -i <path-to-private-key> user@server-ip
