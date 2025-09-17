# Cybersecurity Lab Setup Instructions

This guide walks you through downloading and installing the required software, creating virtual machines, and running basic commands.

---

## Step 1: Install VirtualBox

1. Go to [https://www.virtualbox.org](https://www.virtualbox.org).
2. Download the latest version for your operating system.
3. Run the installer and accept the license agreement.
4. Use default settings (click **Next** through the wizard).
5. Allow the network change warning by clicking **Yes**.
6. Finish the installation and launch VirtualBox.

---

## Step 2: Create a Windows 11 Virtual Machine

1. Download the Windows 11 Enterprise ISO from [Microsoft Eval Center](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-11-enterprise).
2. Register with your information to access the free ISO (use a disposable email if you prefer).
3. Choose your language and CPU version (64-bit recommended).
4. In VirtualBox, go to **Machine > New**.
5. Name the VM `Windows11-Lab` and select the downloaded ISO image.
6. Choose **Unattended Install** and set a username/password.
7. Set resources:
   - Memory: at least **4 GB**
   - CPUs: at least **1**
   - Disk size: at least **80 GB**
8. Click **Finish**.
9. Start the VM to install Windows 11 (automatic installation).

---

## Step 3: Create a Kali Linux Virtual Machine

1. Download the **Kali Linux VirtualBox OVA** from [Kali.org](https://www.kali.org/get-kali/) → **Virtual Machines**.
2. Select the VirtualBox version and download it.
3. In VirtualBox, click **Add**, select the OVA file, and click **Open**.
4. Start the Kali VM.
5. Log in with:
   - Username: `kali`
   - Password: `kali`

---

## Step 4: Verify Network Connectivity

1. On Windows VM, open Command Prompt (`Win + R`, type `cmd`, press Enter).
   - Run `ipconfig` and note the **IPv4 address**.

2. On Kali VM, open Terminal (`Ctrl + Alt + T`).
   - Run `ping <Windows_IP>` to confirm connectivity.

---

## Step 5: Run Basic Commands

### On Windows VM (Command Prompt)
- `whoami` → shows logged-in user.
- `cd \` and `dir` → navigate and list directories.
- `systeminfo` → view system details.
- `tasklist` → list running processes.
- `netstat -an` → view network connections.

### On Kali Linux VM (Terminal)
- `whoami` → shows current user.
- `ip a` → list network interfaces and IPs.
- `ping <Windows_IP>` → test connection to Windows VM.
- `ps aux` → list running processes.
- `sudo apt update` → update software repositories.

---

✅ You now have a working cybersecurity lab with Windows and Kali Linux VMs!