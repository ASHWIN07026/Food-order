**EX.NO: Configure VirtualBox with Ubuntu/Fedora on Windows 7**

**Date:**

---

## Aim:
To configure the VirtualBox with Ubuntu / Fedora of the Linux operating system on top of the Windows 7 operating system.

---

## Procedure:

1. Download and install **VirtualBox** from www.virtualbox.org
2. Download **Ubuntu/Fedora ISO** file from their official website.
3. Open VirtualBox, click **"New"**, enter name, select Type as **Linux** and Version as **Ubuntu/Fedora**.
4. Allocate **RAM (1024 MB or 2048 MB)** and click Next.
5. Create a **Virtual Hard Disk** of 20 GB (VDI, Dynamically allocated).
6. Go to **Settings → Storage**, attach the downloaded ISO file.
7. Click **Start** to boot and follow the on-screen installation steps.
8. Set username, password and complete the installation.
9. Restart the virtual machine after installation.

---

## Program:
```bash
uname -a
lsb_release -a
df -h
free -m
ping google.com -c 4
```

---

## Output:
```
Linux ubuntu 5.15.0-25-generic x86_64 GNU/Linux
Ubuntu 22.04 LTS
Filesystem: 20G  Used: 5.2G
Memory: 2048MB
4 packets transmitted, 0% packet loss
```

---

## Result:
Thus, VirtualBox was successfully configured with Ubuntu/Fedora Linux operating system on top of Windows 7 and verified successfully.
