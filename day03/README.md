![Internet](../avatar.jpg)

## Day 03 of 90 
In our [previous](../day02) session, we discussed HTTP and its  role in Websites. Today, we will have a look at what DNS is and why is it important. 

## Intro
I'm pretty sure I speak for everyone when I say that it is easier to find your friends number in your phonebook by searching their name rather than having to remember their phone number. DNS is the phonebook of the internet. It maps domain names to the respective IP addresses, so that users dont have to remember the complex IP address of websites and just remember the domain names instead.  Web servers where websites are hosted have addresses known as IP addresses to identify them (an example is google.com  whose IP address is 172.217.170.206). You can copy and paste the adress directly into your browser and you will be taken to [Google's](https://google.com) home page.

 Since the addresse are really complex, DNS helps us by giving us the chance to remeber the domain (google.com) instead of the  very complex numbers. It takes care of translating the domain names into their respective addresse. Cool Right?

 ## Resources 
 
 1. [What is a domain name](https://www.cloudflare.com/en-gb/learning/dns/glossary/what-is-a-domain-name/)
 2. [What is DNS](https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/)
 3. [How does DNS work](https://www.youtube.com/watch?v=Y4cRx19nhJk)
 4. [Youtube](https://www.youtube.com/results?search_query=how+DNS+works)
 5. [Google](https://www.google.com/search?q=how+DNS+works)
 6. [Mess with DNS - DNS playground](https://messwithdns.net/)
 7. [How DNS works (comic)](https://howdns.works/ep1/)
 8. [DNS records](https://www.youtube.com/watch?v=7lxgpKh_fRY)
 9. [Glue Records](https://www.youtube.com/watch?v=e48AyJOA9W8)
 10. [All about DNS records](https://www.youtube.com/watch?v=YV5tkQYcvfg)
 11. [Authoritative v/s Recusive DNS servers](https://umbrella.cisco.com/blog/what-is-the-difference-between-authoritative-and-recursive-dns-nameservers)

 ## Learning objectives
 After going through the above resources, you should be able to explain the following concepts to a five year old

 * [X] What is a domain
 * [X] The parts of a domain name
 * [X] Difference between domain name and URL
 * [X] What the heck is DNS and how does it work
 * [X] The DNS query pipeline
 * [X] Recusive DNS lookup VS iterative lookup
 * [X] The four servers involved in a DNS lookup ( assuming the address is not cached)
 * [X] What is a CNAME record
 * [X] How does  resolution for subdomains happen?
 * [X] What is DNS caching 
 * [X] What are A records
 * [X] What are MX records 
 * [X] What are TXT records and some examples of it
 * [X] What are NS records
 * [X] Security concerns associated with DSN

 ## Wrapping up
 - DNS is the phonebook of the internet
 - Nameservers make up the DNS, they hold dns records and map domain names to IP addresses
 - The four DNS servers are 
    - __DNS resolver__  (operated by the ISP) which is like the midleman between the end user and the other DNS servers. It also checks for cached records, and caches and stores results of DNS queries 
    - __Root Nameserver__ - Theres really not alot of these, around 13 or so in the whole world
    - __TLD Nameserver__ 
    - __Authoritave Nameserver__ - This stores the actual domain records
- DNS records ares instructions living in the authoritative nameserver that  provide information about a domain.Some of the most common DNS records include: 

    - __A record__ - For IP address lookup and [DNSBL](https://www.google.com/search?q=dnsbl)(more on this letter). Thanks to this, we can visit websites we dont even know their IP addresses :) 
    - __AAAA record__ - It's like the A record, except is points to the IPv6 addresses
    - __CNAME record__ - Which points a domain name (alias) to another domain name. Mostly used in subdomains
    - __NS record__ - Specifies the authoritative nameserver for a domain
    - __MX record__ - Specifies where the emails for a domain should be routed, making it possible to direct emails to a mail server
    - __TXT records__ - For verification and security. Include SPF records and DKIM records which helps identify your domain as a trusted source for email systems. This helps your emails from being treated as spam


Thats it for today, see you in the [next](../day04) session