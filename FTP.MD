
 ## FTP 

The File Transfer Protocol is a standard communication protocol used for the transfer of computer files from a server to a client on a computer network. FTP is built on a client–server model architecture using separate control and data connections between the client and the server.

[Port Version](#Port-Version)

[Anonymous Login](#Anonymous-Login)

[Nmap Script](#nmap-script)

[Metasploit auxiliary](#metasploit-auxiliary)

[Banner grabbing](#Banner grabbing)

[Search exploit](#search-exploit)

[Ftp Login](#ftp-login)

[Brute Force](#brute-force)

[Downlods file in ftp server](#Downlods-file-in-ftp-server)

[FTP CONFIG FILE ](#FTP-CONFIG-FILE)

  
 ##  Port Version
    
    nmap -A -p21 IP
   
 ##  Anonymous Login 

    ftp-anon.nse
    
 ## Nmap Script
  
 
    ftp-anon.nse
    ftp-brute.nse
    tftp-enum.nse
    ftp-syst.nse
    etc.....    
     
  ## Metasploit auxiliary  
  
    auxiliary/scanner/ftp/anonymous
    auxiliary/scanner/ftp/ftp_version
    auxiliary/scanner/ftp/ftp_login
    etc....
    
  ## Banner grabbing
     
     telnet IP 21
     nmap -sV --script=banner IP
     nc IP 21
    
  ## search exploit
  
    google.com
    searchsploit
    cve
    github
    etc.....
    
  ## Ftp Login
    
    ftp Ip
    
  ## Brute Force 
  
     hydra -l user -P passlist.txt ftp://192.168.0.1
     
  ## Downlods file in ftp server
       
     get file.txt
   
 ## FTP CONFIG FILE 
 
    /etc/vsftpd.conf
