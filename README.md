# bannerme
### Pure python banner grabbing
<img width="200" alt="bannerme" src="https://github.com/user-attachments/assets/5e9e29b9-a25a-4137-8bf6-7696b7c1cc2e" />

# Description
The tool bannerme was designed to make the banner grabbing a little prettier. It simply ingests any '.nmap' file, attempts banner grabbing purely in python and presents the information in a nice table.

# Install
```
sudo wget https://github.com/DaddyBigFish/bannerme/raw/refs/heads/main/bannerme -O /usr/local/bin/bannerme; sudo chmod +x /usr/local/bin/bannerme
```

# Example
```
bannerme *.nmap

10.10.10.3
┏━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Port ┃ Service     ┃ Banner                                ┃
┡━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
│ 21   │ FTP         │ 220 (vsFTPd 2.3.4)                    │
│      │             │ 530 Please login with USER and PASS.  │
│ 22   │ SSH         │ SSH-2.0-OpenSSH_4.7p1 Debian-8ubuntu1 │
│ 139  │ NETBIOS-SSN │ -                                     │
│ 445  │ SMB         │ SMBv1 (Signing is Enabled)            │
└──────┴─────────────┴───────────────────────────────────────┘
```
