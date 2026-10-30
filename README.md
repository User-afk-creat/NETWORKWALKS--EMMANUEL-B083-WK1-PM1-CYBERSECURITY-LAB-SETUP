Objective: Setup a localized cybersecurity testing lab environment using Kali Linux as the primary attacking machine, configured on a custom NAT network (10.0.0.0/24) with specific IP assignments and host accessibility.

1. Operating System Installation & Environment

The Kali Linux virtual machine has been successfully imported, booted, and configured within the hypervisor environment. Virtual machine tools are active, allowing for desktop interaction, clipboard sharing, and host-to-guest file integration.

Proof of Kali Linux running successfully:
![alt text](<image copy 5.png>)

2. Network Configuration (NAT Network)

The hypervisor's virtual network was configured to use a custom NAT network on the 10.0.0.0/24 subnet. The Kali Linux network interface was manually assigned the required IP address of 10.0.0.2 with a /24 (255.255.255.0) subnet mask and a gateway of 10.0.0.1.

Proof of proper IP assignment in Kali Linux:
![alt text](<image copy 3.png>)

3. Network Connectivity & Ping Verification

To ensure the custom NAT network allows proper communication between machines on the same subnet (as well as routing out to the internet), a ping test was conducted. Another machine on the network successfully reached the Kali Linux attacking machine.

Proof of successful ICMP communication to Kali (10.0.0.2):
![alt text](<image copy 4.png>)

Conclusion: All parameters for the Week 1 Project Module 1 task have been met. The Kali Linux attacking machine is stabilized at 10.0.0.2 and is ready for future module deployments.
