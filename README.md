## AUTOMATIC-RECON-FOR-WEB-APPS-RECON-OSIT

<img width="1405" height="744" alt="Screenshot 2026-02-12 alle 12 42 56" src="https://github.com/user-attachments/assets/1f0f8f73-819b-4ee9-90f8-dab6798ec7c6" />








## This script is used to perform advanced recon on web applications in an automated way, i.e. 
## the “information gathering” phase of a pentest / bug bounty.

## ANALYZE SECURITY HEADERS 

## [+] Check if the site uses important headers such as:
## [+] Content Security Policy
## [+] X-Frame Options
## [+] Strict transport safety





## FINGERPRINTS TECHNOLOGIES 
## Law:
## Server
## Powered by X
## template in HTML
## Try to understand if the site uses:
## WordPress, Drupal, Joomla
## Laravel, Django, ASP.NET, PHP
## React, Angular, etc.


## ENUMERATE SUBDOMAINNS 
##  With bruteforce DNS using a wordlist:
##  e.g. api.example.com, dev.example.com, admin.example.com…
## With crt.sh (certificate transparency):
## Retrieve subdomains from public SSL certificates.
## Useful for discovering additional, often less protected assets (dev, testing, staging).

## install command
```
python webrecon.py \
  -u https://example.com \
  -sw wordlists/subdomains_small.txt \
  -pw wordlists/common_paths.txt
```
