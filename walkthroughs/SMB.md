# SMB Enumeration – Metasploitable2 Lab

##  What I Did
Performed **SMB Enumeration** on a vulnerable Metasploitable2 target. Discovered open ports (139 & 445), listed available shares using `smbclient`, and explored shared directories both anonymously and using known credentials.

---

##  Tools Used
- `nmap`
- `Metasploitable2 (target system)`

---

## Steps

### 1. Scanned for Open Ports

- Port 139 → NetBIOS Session Service
- Port 445 → Microsoft-DS Active Directory / SMB

---

### 2. Connected Using `smbclient`

#### List available shares:

Got list of share names like `tmp`, `opt`

---

### 3. Accessed a Share

Anonymous login attempt:

```bash
smbclient //<target-ip>/<sharename> -N
```

---

## Screenshot – Logged into Share & Explored
![smb](../images/smb.jpg)

 Navigated directories, searched for `passwd`, or uploaded a test file.

---

## Fixes:

### 1. **Restrict Share Access**
   Remove anonymous access from sensitive shares.

### 2. **Least Privilege**
   Users should only see what they need. E.g., `tmp` instead of full `/`.

### 3. **SMB Signing + Encryption**
   Prevent MITM attacks on corporate networks.
