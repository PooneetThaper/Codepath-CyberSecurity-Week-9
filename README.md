# Codepath-CyberSecurity-Week-9

## Honeypot Deloyed:

I simply deployed the Dionaea honeypot on an instance on GCP.

## Issues Faced:

 - Had issues installing pyev when executing install.sh
   - Offending command was “pip install -e git+https://github.com/HurricaneLabs/pyev.git#egg=pyev” in install_hpfeeds.sh in the scripts folder.
   - Found an existing repo with pyev available (https://github.com/kbandla/pyev), forked it, and brought the content of pyev-0.9.0 to root in my own fork (https://github.com/PooneetThaper/pyev.git). Replaced the url in install_hpfeeds.sh with the link to my fork and it was able to install pyev successfully.
 - Accessing the admin console
   - I had attempted to access the console using the link to the external ip in the GCP interface. This used https rather than simply http. After switching to http, I was able to access the dashboard.
   
## Summary of data:

- Number of attacks:  	2427
- Payloads:             None

## Unresolved Questions:

Distribution of the attacks across the globe? (Seem to be many eastern european and coastal US attackers)
What type of attack they attempted?

