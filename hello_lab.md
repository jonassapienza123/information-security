# Hello Lab  

## x)  
### Karvinen 2021: Install Debian on VirtualBox (Updated 2024)  
- explains how to install Debian inside VM safely without modyfying the cost computer  
- Virtual machines are useful for learning hacking because they are isolated and easy to reset.  
- Debian is recommended because it is stable, widely used, and well documented.
- My question: How does virtualization affect performance compared to installing Linux directly on hardware?
 ### Karvinen 2020: Command Line Basics Revisited   
-Introduces basic Linux command-line usage and common commands.  
-Shows how networking, files, and processes can be inspected from the terminal  
-The command line is essential for security work and system administration.  

  ## a)  
 I first tested networking while the Internet connection was enabled. I ran command ping 1.1.1.1 and received replies. This showed that packets were successfully sent and received, proving that the network connection was working. I used Ctrl+C to stop the command.  
Next, I disabled the network using command sudo nmcli networking off. After that, I ran command ping 1.1.1.1 again.This time I did not receive any replies and the output showed that the network was unreachable. This shows that packets could not go through when networking was disabled.  
The ping command sends small test packets to another computer. The address 1.1.1.1 is a public DNS server that is normally always reachable. When replies are received, the network is working. When no replies are received, it shows that networking is disabled.  
disabling networking prevents packets from going through.  

  ## b)  
I worked inside my Debian VirtualBox machine and made sure I only scanned my own computer, which is the only legal and safe way to practice port scanning. First, I installed the scanning tool by running sudo apt update and sudo apt install nmap.  

After installing it, I disabled the network using sudo nmcli networking off so the virtual machine had no Internet connection. I verified this by running ping 1.1.1.1, which returned no replies, confirming the machine was offline. I stopped the ping with Ctrl+C.  

Next, I scanned my computer using the command sudo nmap -sT -p- localhost.   
sudo runs the command with administrator privileges.    
nmap is a port scanning tool.   
-sT performs a TCP connect scan.  
-p- scans all ports.  
localhost targets my own computer.    

The scan showed that port 631/tcp with service ipp was open.

Conclusion:  
I successfully identified services on my local machine while it was disconnetcted from the internet, ensuring it was safe and legal.

  ## c)  
First, I performed a port scan on localhost without installing a new daemon to see the baseline state of the system. I disabled the Internet connection with sudo nmcli networking off and ran sudo nmap localhost. The scan showed that port 631/tcp (ipp), the printing service, was open by default.  
I then installed a daemon by enabling the network and running sudo apt update and sudo apt install openssh-server. After installation, I disabled the network again and repeated the scan with sudo nmap localhost. This time the scan showed a new open port: 22/tcp (ssh).  
Conclusion: Fewer ports were open before installing daemon. After installing OpenSSH, port 22 appeared because the SSH service was running and listening for connections. This shows that port scanning can reveal which server applications are active on a system.  
## d)  
I did not manage doing this task



