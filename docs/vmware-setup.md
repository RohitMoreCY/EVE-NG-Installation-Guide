# VMware Workstation 17 Pro Setup Guide

This document covers VMware settings required to run EVE-NG smoothly.

---

## 🔧 Enable Virtualization (IMPORTANT)

Before installing:

1. Restart your laptop  
2. Enter BIOS (F2 / Delete / F10 depending on brand)  
3. Enable:
   ```
   Intel VT-x
   AMD-V
   Virtualization Support
   ```
4. Save & Exit

---

## 🧰 Recommended VM Settings for EVE-NG

| Component | Setting |
|----------|---------|
| CPU      | 4–8 cores |
| RAM      | 12–16 GB |
| Disk     | 60 GB SSD |
| Network  | Bridged Adapter |
| Graphics | Accelerated (optional) |

---

## 🔌 Improve VM Performance

### 1. Increase Memory for the VM
Settings → Memory → Drag slider to **12–16 GB**

### 2. Increase CPU Cores
Settings → Processors → Set to **4 or more**

### 3. Disable Unnecessary Background Apps

### 4. Keep VMware Updated

---

## 📡 Network Modes Explanation

### **Bridged Mode**
- VM gets an IP directly from your router  
- Best for labs, firewalls, SOC tools  
- EVE-NG devices can talk to your local network  

### **NAT Mode**
- VM shares your host’s IP  
- Not ideal for networking labs  

### **Host-Only Mode**
- Isolated network  
- Useful for malware testing or sandboxing  

---

## 🎯 Summary
Using the correct VMware settings ensures:

- Faster EVE-NG boot  
- Better stability  
- Smooth multi-device labs  

