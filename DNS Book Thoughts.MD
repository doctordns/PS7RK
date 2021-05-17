# Mastering DNS with PowerShell 7

## Scope

This book describes Microsoft's Windows Server's Domain Name Server (DNS feature.
It provides and in-depth explanation of what DNS is, and how to deploy,manage, and troubleshoot DNS.
Includes coverage of the commands and IT Pro can use to manabe DNS.
The book also describes the DNS protocol and includes network captures showing DNS in action.

The book looks at deploying DNS in each of the three reference architectures.

## Suggested Chapters

1. Background and Introduction
   1. Brief history - hosts.txt -> jeeves to BIND
   2. AD in Server 2000 uses DNS to locate DCs
   3. Improved since - added EDNS, DNSSEC, etc
   4. Introducing the reference architecture for this book and build scripts
2. How Does DNS Work?
   1. A global hierarchy of domains
   2. Zones
   3. Resource Records
   4. DNS Client resolution
3. Name server types
   1. primary domain servers
   2. secondary domain servers
   3. caching only name servers
   4. forwarders and slaves
4. The DNS Server and DNS Client PowerShell module
   1. Explain both modules
   2. Group the commands to explain the later sections of this book
   3. This should cover core cmdlets in client and server modules
5. Deploying DNS with PowerShell
   1. Create a DC with DNS integrated
   2. Create a stand alone DNS Windows Server
   3. Setup a BIND Server in WSL
6. DNS Zones and resource records
   1. Zone types - forward reverse
   2. Zone storage - files vs AD
   3. Core Resource Records and syntax
      1. NS, SOA records
      2. A, AAAA records
      3. PTR records
      4. SRV records
      5. TXT records
      6. MX records
      7. Others??
   4. Domain delegation
   5. Root servers and the cache file
7. DNS Active Directory-integrated zones
   1. AD domain vs forest partitions
   2. Using AD integrated zones
   3. Secure dynanic update
8. DNS and Email
   1. The MX record
   2. Priorities - I'm at a loss as to how to test this however!
9. DNS and anti-spam
10. DNS Security
11. Single label name resolution
12. Name resolution Policy and NRPT
13. Scaling DNS in the enterprise
    1. Split-brain
    2. Conditional forwarders and stub zones
14. DNS Security and DNSSEC
    1. General DNS security issues and recommendations
    2. What is DNSSec
    3. Deploying DNSSec
    4. 
15. DNS and DHCP - a chapter both in this and the DHCP book?
    1. DHCP and DNS integration
    2. Configuring DNS with DHCP.
16. DNS over HTTP
    1. What is it?
    2. How to configure?
    3. Get-DNSClientDOHServerAddress
17. DNS in Azure
    1.  Describe the DNS features of Azure
    2.  SH
18. DNS Troubleshooting
    1. Resolve-DNSName
    2. DNS event logs
    3. DNS logging
19.IPAM (IP Address Management) - possibly a shared chapter with DHCP booK?
20. The DNS protocol and protocol messages
    1. See TFL's TCP/IP book for some ideas on what  such a section could look like.
    2. SXhould include wireshark traces shoing key eventsd: registration, lookup, zone transfer, etc.