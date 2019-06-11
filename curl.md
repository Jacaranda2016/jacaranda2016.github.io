
# What is "Curl"?
> cURL (pronounced as curl) is a tool to transfer data from and to a server, using one of the supported protocols(DICT, FILE, FTP, FTPS, 
> GOPHER, HTTP, HTTPS, IMAP, IMAPS, LDAP, LDAPS, POP3, RTMP, RTSP, SCP, SFTP, SMB, SMBS,SMTP, SMTPS, TELNET and TFTP). The command is 
> designed to work without interface. 


       curl offers a busload of useful tricks like proxy support, user authen-
       tication, FTP upload, HTTP post, SSL connections, cookies, file  trans-
       fer  resume,  Metalink,  and more. As you will see below, the number of
       features will make your head spin!

       curl is powered by  libcurl  for  all  transfer-related  features.  See
       libcurl(3) for details.

## What is URL?
The URL syntax is protocol-dependent. e.g.
- http://site.{one,two,three}.com
- ftp://ftp.example.com/file[1-100].txt

If you specify URL without protocol:// prefix, curl will attempt to guess what protocol you might want. It will then default to HTTP but try other protocol based on often-used host name prefixes. 

## Get information about curl
* curl --help
* curl --manual

## Main purpose of curl
- it makes the requests
- it gets the data
- it sends the data
- it retrieves the informaiton



[CURL AND HTTP](https://curl.haxx.se/docs/httpscripting.html)
