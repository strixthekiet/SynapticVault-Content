---
mindmap-plugin: basic
tags:
  - CompSci/network/term
aliases:
  - DNS
---
# Domain naming service, DNS
### Description:
- Translate internet hostnames to [[IP address]]es
- Computer reads domain from right to left, \www.sub.example.com.
	- www. is subdomain
	- example is 2nd level domain
	- .com is top level domain
	- . is root domain
- A record is a mapping between a DNS resource and a domain name. 
	- Each individual DNS record has a type (name and number), an expiration time (time to live), and type-specific data.
- There are levels: root server, domain server, name server
- https://cloud.google.com/dns/docs/records-overview
### DNS zone:
- A section of a domain name space that a certain administrator has been delegated control over.
	- sub1.example.com
- 
### Resource record:
- A
	- Address record to resolve domain name to [[IPv4 address]]
- AAAA
	- Address record to resolve domain name to [[IPv6]] address
- CNAME
	- Canonical name
	- Resolve a domain or subdomain to another domain name
		- Alias of one name to another
		- the DNS lookup will continue by retrying the lookup with the new name.
		- Point subdomain to domain, fpt.example.com to example.com
- MX
	- Mail exchanger
- SOA
	- Start of authority
	- Stores administrative information about a [[#DNS zone]]
	- MNAME: primary name server
	- Name: email address of the administrator for the zone where second dot is @
	- Serial: represents a version in a zone
- NS:
	- Name server
- SRV
	- Service record