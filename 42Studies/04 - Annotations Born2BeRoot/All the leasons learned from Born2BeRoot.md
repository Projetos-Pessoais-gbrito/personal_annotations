
## Diff between apt and aptitute

- Apt: apt is that apt does not have a inteface, its a tool packet manager
- Aptitute: is a tool packet manager without graphics.
## Paths to implement

	 1 - Is highly recommended to use Debian, because this version of linux requires less details than rocky linux.
	 2 - Usage of LVM, lvm is a tecnology that manages the volumn, it enables to create, redimension and manages the partition.
	 3 - I have to create at least 2 partitions cryptographic, its a good practice of security essential, specially in servers.
	 4 - It will be necessarry to create partitions like /home, swap (Its a memory area in disc used for system when RAM is full).
	 5 - The SSH service must be preprared to accept only connections by 4242 port
	 6 - It must be prrohibited to connect by SSH using root user
	 7 - firewall config with Debian
	 8 - Configuring a firewall for just 4242 port be opened
	 9 - The machine host name must be the 42 login followed by 42, like gserafio42
	 
```sh
 sudo hostnamectl set-hostname wil42
```

	10 - Stong password like
	
```sh
sudo chage -M 30 -m 2 -W 7 username
```

	10 - Change the prerequisite of password
	
```sh
password requisite pam_pwquality.so retry=3 minlen=10 minclass=3
```
