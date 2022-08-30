# Day 2:

**Windows domain and what does it do?**

Usually used on large networks, Windows domains aren't something you'll encounter at home unless you have a laptop provided by your employer or school. Computers are isolated entities meaning you control the settings and user accounts on the computer while a computer joined to a domain is different, the settings are controlled by a domain controller.

With the Windows domain administrators can manage a large number of PCs and control them from one place. Domain controllers, which are one or more servers, have control over the domain and the computers on it. Typically domains are made up of computers on the same local network, however, using a VPN or an internet connection computers on the same domain can continue communicating using the domain controller. This allows businesses and schools to remotely manage laptops they provide to their employees and students
 
A computer doesn't use its own local user accounts when joining the domain, the domain controller will manage the user account and password. When you log into a computer on a domain the computer will authenticate the user account name and password to the domain controller meaning one can log in with the same username and password on any computer that is on the domain
 
Group Policy settings can be changed on the domain controller. computers on the domain get the settings from the domain controller and these settings override any local settings used specifically on the PCs. 
With the settings being controlled from one single place this locks down the computer, meaning you won't be able to change hardly any of the system settings on the computer if it is joined to a domain 


Only Windows Professional and Enterprise versions can join a domain, as home PCS aren't meant to be utilized on domains.
 
One can quickly check if their computer is on a domain by going to the control panel, click systems and securities category, click system. Look at computer name, domain and working group settings. If you see “domain” followed by the name of a domain your computer is joined to a domain. If you see “work group” followed by the name of the work group, your computer is joined to a workgroup instead of a domain. What is the difference? I hear you ask,well read ahead.



If your Windows computer is not on a domain then it is on a work group. A work group is a group of computers on the same local network. Workgroup computers have no control over each other; they are all joined together as equals, and work groups don't require a password.
 
Previously work groups were used for home file and printer sharing with older versions of windows, now one can use home groups to easily share files and printers between PCS at home. One just has to leave the work group name of the work group and set up homegroup file sharing. 
It's not using a locked down PC one can use administrator access to leave a domain if you have the local administrator access on your PC. If you do not have local administrator access then leaving or joining a PC won't really be up to you it will be up to the company and ministrator to handle that
 
 

## DNS:

One of the most popular protocols on the internet, domain name system, is used to translate human-readable names into IP addresses so our computers know where we're trying to go. 

With it being done as a hierarchy, organizing the DNS is very easy making it a very distributed database with various different DNS servers. there are (for instance) 13 route server clusters primary, which are the root servers for everything on the internet and over a thousand servers providing redundancy across the internet as a whole.This allows us to have top level domains, or TLDs, that may be generic such as the .com, .org, or .net addresses we may be familiar with. But there are also country codes that can be used as top level domains. Things like .US, .CA, and .UK are associated with individual countries.



There are several other teal these such as mail which would come before the address and even east and west and within East and West you could have other servers creating a hierarchy that tells exactly what servers are associated with what particular area the video really goes in-depth on those I'm going to skip ahead in my notes

So utilizing an FQDN (fully qualified domain name) one may not only be able to identify what device it is, but also where it is located. 
Typically we will be utilizing an internal DNS on our own network oh, and it would be running on our own internal services.
