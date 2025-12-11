# EVE-NG Installation Guide (VMware Workstation 17 Pro)

This guide will walk you through installing **EVE-NG Community Edition** on VMware Workstation 17 Pro.

---

## 📥 Step 1 — Download EVE-NG ISO

Download from the official page:

👉 https://www.eve-ng.net/index.php/download/

File example:
```
EVE-NG-Community-4.x.x.iso
```

---

## 🖥 Step 2 — Create a New VM in VMware

1. Open VMware Workstation → **Create a New Virtual Machine**
2. Choose **Typical** configuration
3. Select **Installer disc image file (ISO)** → Choose the EVE-NG ISO
4. OS Type:
   - **Linux**
   - **Ubuntu 64-bit**

---

## ⚙ Step 3 — Configure Hardware

### CPU
```
4 cores (recommended: 6 cores)
```

### RAM
```
8 GB minimum
16 GB recommended
```

### Network Adapter
```
Bridged Mode (best for labs)
```

### Storage
```
60 GB (store as a single file)
```

Click **Finish**.

---

## 🚀 Step 4 — Install EVE-NG

1. Start the VM  
2. Select **Install EVE-NG Community**  
3. Choose **Auto Install**  
4. Let the setup complete  
5. Reboot when prompted  

---

## 🔧 Step 5 — First Boot Configuration

You will be asked:

### Hostname:
```
eve-ng
```

### Domain:
```
local
```

### DHCP:
```
Yes
```

### Root Password:
(choose your own)

---

## 🌐 Step 6 — Access EVE-NG Web GUI

After reboot, the VM will display an IP such as:

```
https://192.168.1.50
```

Open it in your browser (ignore HTTPS warning).

### Login:
```
Username: admin
Password: eve
```

---

## 🎉 Installation Complete
Your EVE-NG server is now ready to run:

- Cisco routers  
- Firewalls (FortiGate, pfSense, Palo Alto)  
- Linux & Windows VMs  
- SOC + Blue Team Labs  

