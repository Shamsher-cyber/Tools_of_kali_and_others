Got it 👍
Below is a **clean, professional, and corrected README** based on your original content. I’ve fixed:

* Grammar and spelling
* Command formatting
* Structure and flow
* Technical clarity
* Consistent Markdown style

I **did not change your intent or tools**, only made it professional and industry-standard.

---

# DVWA Installation on Kali Linux (Using PentestLab)

This guide explains how to install **Damn Vulnerable Web Application (DVWA)** on **Kali Linux** using the **PentestLab Docker framework**.

PentestLab allows you to quickly deploy multiple vulnerable web applications using Docker, making it ideal for penetration testing and practice labs.

---

## Prerequisites

* Kali Linux (x64)
* Internet access
* `git` installed
* Root or sudo privileges

---

## Step 1: Clone the PentestLab Repository

Clone the official PentestLab repository from GitHub:

```bash
sudo git clone https://github.com/eystsen/pentestlab
```

This repository contains scripts to install Docker and deploy multiple vulnerable applications.

---

## Step 2: Navigate to the PentestLab Directory

```bash
cd pentestlab/
```

---

## Step 3: Install Docker and Dependencies

Run the Docker installation script for Kali Linux (x64):

```bash
sudo bash install_docker_kali_x64.sh
```

This script will:

* Install Docker
* Install Docker Compose
* Configure required dependencies automatically

---

## Step 4: List Available Applications

To see all available vulnerable applications that can be installed, run:

```bash
sudo bash pentestlab.sh list
```

This will display a list of supported web applications (DVWA, Juice Shop, etc.).

---

## Step 5: Start DVWA (Localhost)

To install and start **DVWA** on your local machine:

```bash
sudo bash pentestlab.sh start dvwa
```

* DVWA will be deployed using Docker
* The application will be accessible on **localhost**
* Docker will automatically pull required images

---

## Step 6: Start DVWA on a Public IP (Optional)

If you want to expose DVWA on a **public IP** instead of localhost, use:

```bash
sudo bash pentestlab.sh startpublic dvwa
```

⚠️ **Warning:**
Only expose vulnerable applications on a public IP in controlled lab environments. Never expose them on production systems.

---

## Step 7: Stop DVWA

To stop the DVWA container:

```bash
sudo bash pentestlab.sh stop dvwa
```

---

## Notes

* The same method can be used to install **any other vulnerable application** supported by PentestLab.
* This setup is intended **only for learning, CTFs, and ethical hacking practice**.
* Do **not** use DVWA on production systems.

---

<!-- 
If you want, I can also:

* Add **screenshots section**
* Add **troubleshooting**
* Add **Docker networking explanation**
* Convert this into a **GitHub-grade README with badges**

Just tell me 🔥 -->


      
