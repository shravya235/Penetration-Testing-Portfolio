# SSH Access via Brute Force – Metasploitable2 

##  What I Did
Targeted an exposed **SSH service (port 22)** on a vulnerable machine. Used `medusa` to perform a brute-force login attack with a list of common usernames and passwords. Successfully gained admin access, then accessed `/etc/passwd` to confirm full login.

---

## Tools Used
- Metasploitable2 (target machine)
- `nmap` 
- `medusa` 

---

## Screenshot – `/etc/passwd` Access via SSH  
![ssh](../images/ssh.jpg)

---

## Steps

### 1. Scanned the target to confirm SSH is running  
Used a service scan to detect open Port 22 and confirm it was SSH.

### 2. Created Username & Password Lists  
Manually created files for usernames and passwords

### 3. Ran Medusa for SSH Brute Force  
Executed `medusa` to attempt all combinations from the wordlists. 

Login was successful — no lockouts or rate-limiting in place.

---

### 4. Gained Remote SSH Access  
Logged in using the valid credentials over SSH. Used specific options to ensure older key exchange algorithms (`ssh-rsa`) were accepted — a useful trick for older VMs like Metasploitable2.

---

### 5. Verified Full Shell Access  
Once inside, navigated the file system and read `/etc/passwd` to confirm user-level access. This validated a complete compromise of the target’s SSH service.

---

## Fixes:

### 1. **Disable SSH for Root**
   Restrict login to specific users only

### 2. **Rate Limiting**
   Enable fail2ban or sshguard to prevent brute-force attacks

### 3. **Use Strong Passwords**
   Prevent dictionary attacks using basic wordlists

### 4. **Audit Logs Regularly**
   Monitor `/var/log/auth.log` for repeated failed attempts

