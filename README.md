# bannerme
### Nmap banner grabbing in style!
<img width="200" alt="bannerme" src="https://github.com/user-attachments/assets/5e9e29b9-a25a-4137-8bf6-7696b7c1cc2e" />

# Description
The tool bannerme was designed to make the banner grabbing a little prettier. It simply ingests any '.nmap' file, attempts nmap banner grabbing using -A scan and presents the information in a nice table.

# Install
```
sudo wget https://github.com/DaddyBigFish/bannerme/raw/refs/heads/main/bannerme -O /usr/local/bin/bannerme; sudo chmod +x /usr/local/bin/bannerme
```

# Example
```
bannerme *.nmap

10.10.10.3
┏━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Port ┃ Service     ┃ Banner                                          ┃
┡━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
│ 21   │ ftp         │ vsftpd 2.3.4                                    │
│ 22   │ ssh         │ OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0)    │
│ 139  │ netbios-ssn │ Samba smbd 3.X - 4.X (workgroup: WORKGROUP)     │
│ 445  │ netbios-ssn │ Samba smbd 3.0.20-Debian (workgroup: WORKGROUP) │
└──────┴─────────────┴─────────────────────────────────────────────────┘

10.10.10.4
┏━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Port ┃ Service     ┃ Banner                                          ┃
┡━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
│ 22   │ ssh         │ OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0)    │
└──────┴─────────────┴─────────────────────────────────────────────────┘
```
