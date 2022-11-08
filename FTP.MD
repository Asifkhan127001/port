
 ## FTP 

The File Transfer Protocol is a standard communication protocol used for the transfer of computer files from a server to a client on a computer network. FTP is built on a client–server model architecture using separate control and data connections between the client and the server.
  
  
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
    
  ## BANNER GRABBING
     
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
