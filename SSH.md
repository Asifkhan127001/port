  # SSH 
   
   The Secure Shell Protocol is a cryptographic network protocol for operating network services securely over an unsecured network. Typical applications include remote command-line, login, and remote command execution, but any network service can be secured 


    
## Port Version
   
    nmap -A -p22 -sV IP
       
## Nmap Script
    
    ssh2-enum-algos.nse
    ssh-brute.nse
 
## Metasploit auxiliary 
    
    auxiliary/scanner/ssh/ssh_enumusers
    auxiliary/scanner/ssh/ssh_version
    auxiliary/scanner/ssh/ssh_login 
    auxiliary/scanner/ssh/ssh_login_pubkey
    
## BANNER GRABBING
     
     nmap -sV — script=banner  IP
     telnet IP 22
     nc IP 22

     
## Search Exploit
    
    google
    searchsploit
    github
    exploitdb
    cve
    
  ## SSH LOGIN
    
    ssh IP
    SSH -i key Login
    
 ## Brute Force  
 
    hydra -l user -P passlist.txt ftp://192.168.0.1
