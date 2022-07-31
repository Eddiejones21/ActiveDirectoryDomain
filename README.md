# ActiveDirectoryDomain
VM Ware Fusion
Server 1
Created a virtual server using VM Ware 
* Downloaded And installed VM ware fusion 
* Created a virtual machine of a Window server 2016. 
* I added the Iso file to the CD/DVD SATA drive. 
* I configured a bridge network adapter to connect to my local wifi. 
* Started the VIrtual machine up. 
* Chose a custom install to select my virtual disk. 
* I viewed the automatically assigned IP address via the command prompt using IPconfig. 
*  I assigned a static IP address by going to the network and sharing center, change adapter options, right clicked on the adapter and went into properties where I selected IPV4 (internet Protocol version 4) then clicked properties. 
* I selected use the following IP address then entered the same I received from IPconfig in the command prompt.
* I made the subnet mask 255.255.255.0
* Then made the default gateway 10.0.0.1, the address to my home router.
* Made the DNS (Domain Name Server) to match the IP address
* In server manager I selected manage then add roles and features. 
* I then added active directory domains. 
* Promoted the server to a new domain controller by adding it as a new forest. 
* I opened the active directory computers and users tools and added a new user to the domain admin group 
Server 2
* Then I started another new virtual machine and configured the same as the first VM.  
* On the second virtual machine I added a role as a domain controller using the user credentials that I made in the first domain controller and not as a new forest. 


Windows 10
* I stood up a Windows 10 virtual machine, I configured a bridge network adapter to connect to my local wifi.
* I assigned a static IP address by going to the network and sharing center, change adapter options, right clicked on the adapter and went into properties where I selected IPV4 (internet Protocol version 4) then clicked properties. 
* I selected use the following IP address then entered the same I received from IPconfig in the command prompt.
* I made the subnet mask 255.255.255.0
* Then made the default gateway 10.0.0.1, the address to my home router.
* Made the DNS (Domain Name Server) to match the IP address of server 1 the first initial domain controller.
* Then I went to This PC, properties, advanced, then I went to change name and added Jonesway.local as a domain, signed in using credentials of the domain admin user. Successfully added to domain.
