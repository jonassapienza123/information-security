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
 I first tested networking while the Internet connection was enabled. I ran command ping 1.1.1.1 was and received some replies. This showed that packets were successfully sent and received, proving that the network connection was working. I used Ctrl+C to stop the command.  
Next, I disabled the network using command sudo nmcli networking off. After that, I ran command ping 1.1.1.1 again.This time I did not receive any replies and the output showed that the network was unreachable. This shows that packets could not go through when networking was disabled.  
The ping command sends small test packets to another computer. The address 1.1.1.1 is a public DNS server that is normally always reachable. When replies are received, the network is working. When no replies are received, it shows that networking is disabled.  
disabling networking prevents packets from going through.  

  ## b)  
  


