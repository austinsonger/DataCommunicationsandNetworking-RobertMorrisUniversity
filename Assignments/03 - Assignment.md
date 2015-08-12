# Austin Vern Songer #

## Data Communications and Networking ##
     Chapter 2

     Robert Morris University 



----------

### R1. 

List five nonproprietary Internet applications and the application-layer
protocols that they use.

The Web: HTTP; file transfer: FTP; remote login: Telnet; Network News: NNTP;
e-mail: SMTP.

----------

### R2

What is the difference between network architecture and application
architecture?

Network architecture refers to the organization of the communication process into
layers (e.g., the five-layer Internet architecture). Application architecture, on the
other hand, is designed by an application developer and dictates the broad
structure of the application (e.g., client-server or P2P)


----------

### P1 

True or false?

a. A user requests a Web page that consists of some text and three images.
For this page, the client will send one request message and receive four
response messages.

b. Two distinct Web pages (for example, www.mit.edu/research.html
and www.mit.edu/students.html) can be sent over the same persistent
connection.

c. With nonpersistent connections between browser and origin server, it is possible
for a single TCP segment to carry two distinct HTTP request messages.

d. The Date: header in the HTTP response message indicates when the
object in the response was last modified.

e. HTTP response messages never have an empty message body.


----------

### P2

Read RFC 959 for FTP. List all of the client commands that are supported by
the RFC

Access control commands:
USER, PASS, ACT, CWD, CDUP, SMNT, REIN, QUIT.
Transfer parameter commands:
PORT, PASV, TYPE STRU, MODE.
Service commands:
RETR, STOR, STOU, APPE, ALLO, REST, RNFR, RNTO, ABOR, DELE,
RMD, MRD, PWD, LIST, NLST, SITE, SYST, STAT, HELP, NOOP.


----------

### P3. 

Consider an HTTP client that wants to retrieve a Web document at a given URL. The IP address of the HTTP server is initially unknown. What transport
and application-layer protocols besides HTTP are needed in this scenario?

Application layer protocols: DNS and HTTP
Transport layer protocols: UDP for DNS; TCP for HTTP