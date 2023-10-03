# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/0a65409a-5ed5-47fa-90c8-120a99097ce4)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/043a5fa7-ad6a-4f05-8b67-edaae65b58a3)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/73092e5d-4d07-4a0b-a087-6a4c98ad51ff)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/fa3124b1-d6a5-414e-8bb3-cdb6e7b84fc4)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/a27c097f-b0b3-40ee-bba5-e4444540701a)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/d2f2fe75-9dd6-402a-b4ca-1bfd8ec13ab5)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/49a5fce5-1eac-4b11-9027-09e746c8c40d)

#DNS Enumeration

##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/97216cb7-e147-411e-b590-3fa802a72990)
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/355da3de-cf5a-42a3-9524-0283d35edaa8)

##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/22aa968b-e813-44d9-b0a0-a25210359a1c)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/a4c68c73-15d2-4d15-aefd-24b52bb87b3f)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/7f1acac1-074f-480b-b279-37da1e913cd5)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## OUTPUT:
 ![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/271f1eaf-dcc7-4298-89e1-82e4f486040e)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![image](https://github.com/Udhayasankaran04/Enumeration/assets/119393933/48979bde-5b8e-4bc4-9a7b-7a320bef035a)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

