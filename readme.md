This is an experimental Splunk dashboard for tracking and baselining household IoT stuff.  
It is based on the DNS datamodel in the CIM and provides a three day look back and compares each days stats against the others.  
It also uses an inventory csv that has mac_addresses, ip addresses, type of host, and host names that is based on a static IP list, a MAC OUI lookup, and DHCP logs.  If you don't have an inventory, a coalesce statement should give you just the source IP.

This dashboard provides a couple of different ways to look at the hosts.
count of 2ld level domain DNS lookups
count of dest_ips
Experimental Dest Port Review
There is also a 'hipster's socks' type chart that visualizes bytes (from the All_Traffic datamodel) looking for anomolies.  
