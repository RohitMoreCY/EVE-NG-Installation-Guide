# Uploading Router, Firewall & OS Images to EVE-NG

To run routers/firewalls inside EVE-NG, you must upload images manually.

---

# 📁 1. EVE-NG Image Folder Structure

All images go into:

```
/opt/unetlab/addons/
```

Inside this directory, there are folders like:

- `qemu/` → For firewalls, servers, Linux, Windows  
- `iol/` → For Cisco IOL images  
- `dynagen/` → For dynamips routers  

---

# 🔼 2. Uploading Files Using WinSCP

### Step 1 — Download WinSCP  
https://winscp.net

### Step 2 — Connect to EVE-NG  
Use:

```
Host: <eve-ng-ip>
Username: root
Password: <your-root-password>
```

### Step 3 — Navigate to:
```
/opt/unetlab/addons/qemu/
```

### Step 4 — Create a folder (examples):

| Device | Folder Name |
|--------|-------------|
| FortiGate | fortinet-FGT-v7 |
| Palo Alto | paloalto-v10 |
| pfSense | pfsense-v2 |
| Ubuntu | ubuntu-20.04 |
| Windows | win10 |

### Step 5 — Upload the `.qcow2` image

---

# 🛠 3. Fix Permissions (IMPORTANT)

After uploading images, run this command in EVE-NG terminal:

```
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

This is required or nodes will NOT start.

---

# 🎉 Supported Image Types

### Firewalls
- FortiGate  
- Palo Alto  
- pfSense  
- CheckPoint  

### Routers/Switches
- Cisco IOL  
- Cisco vIOS  
- Cisco ASA  

### Servers/OS
- Ubuntu Server  
- Kali Linux  
- Windows Server  
- Windows 10  

---

# 🎯 Summary
Correct image upload + permissions = stable EVE-NG labs.  

