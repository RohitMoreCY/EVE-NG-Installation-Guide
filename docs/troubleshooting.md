# EVE-NG Troubleshooting Guide

This document covers the most common issues and fixes.

---

## ❌ Issue 1 — EVE-NG Web UI Not Opening

### ✔ Fix:
Restart nginx:
```
systemctl restart nginx
```

Check VM IP:
```
ifconfig
```

---

## ❌ Issue 2 — Node Not Starting (Router/Firewall)

### ✔ Fix 1: Wrong folder name  
Ensure folder naming is correct, ex:
```
qemu/paloalto-v10
```

### ✔ Fix 2: Permissions  
Run:
```
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

---

## ❌ Issue 3 — VM Too Slow

### ✔ Fix:
- Increase RAM to **12–16 GB**  
- Increase CPU cores to **6**  
- Close unnecessary programs  
- Use SSD storage  

---

## ❌ Issue 4 — Import Errors When Uploading Images

### ✔ Fix:
Image must be `.qcow2` format  
Rename files to lowercase  

---

## ❌ Issue 5 — No IP on Boot

### ✔ Fix:
Change network from **NAT → Bridged**  

---

# ✔ You're Good To Go!
If you experience any issue, open a GitHub Issue tab for this repo.  

