rwi_grazer
==========

RunwHiteyI network information gathering solution

Purpose: To find IP's used by "company" on the Internet, determine OS and application version, and also check any SSL certificates.

Goals:

1. Run digg using a list of domain names to generate a file containing all DNS records.

2. Read a file containing the internet facing IP's assigned to "company" and create a file conaining only IP's that respond

3. Read the output file from goal #2 and do a fast port scan to identify the IP's that have responding IP's and write the data to a file.

4. Read the output file from goal #3 and scan the IP's that have open ports to identify the OS and the services running to a file.

5. Read the file from goal #4 and create a file containing only IP's that have 443  (HTTPS) running. Read this new file to get information from the IP's on the SSL certificate being used (CA, expiration, strength), and create a report.

6. Read the file from goal #4 containing IP's of systems running HTTP. Read the IP's in the new file to run a Nikto scan. 

Output to a pretty report for mass consumption

