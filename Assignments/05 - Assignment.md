# Austin Vern Songer #

## Data Communications and Networking ##
     Chapter 7

     Robert Morris University 


----------

R2

There are two types of redundancy in video. Describe them, and discuss how
they can be exploited for efficient compression.






----------

R4

Multimedia applications can be classified into three categories. Name and
describe each category.


Figure 6.1: simple, doesn’t require meta file or streaming server; Figure 6.2: allows
media player to interact directly with the web server, doesn’t require a streaming
server; Figure 6.3: media player interacts directly with a streaming server, which has
been designed for the specific streaming application.

----------
R5


Streaming video systems can be classified into three categories. Name and
briefly describe each of these categories.


----------

R6


List three disadvantages of UDP streaming.


----------

R9


CDNs typically adopt one of two different server placement philosophies.
Name and briefly describe these two philosophies.


----------

R11

Besides network-related considerations such as delay, loss, and bandwidth
performance, there are many additional important factors that go into designing
a cluster selection strategy. What are they?


Reception report packets: includes info about fraction of packets lost, last sequence
number, inter-arrival jitter; sender report packets: timestamp and wall clock time of
most recently generated RTP packet, number of packets sent, number of bytes sent ;
source description packets: e-mail address of the sender, the sender’s name, the
application that generates the RTP stream.

----------

R13

Why is a packet that is received after its scheduled playout time considered
lost?

In non-preemptive priority queuing, the transmission of a packet is not interrupted
once it has begun. In preemptive priority queuing, the transmission of a packet will be
interrupted if a higher priority packet arrives before transmission completes. This
would mean that portions of the packet would be sent into the network as separate
chunks; these chunks would no longer all have the appropriate header fields. For this
reason, preemptive priority queuing is not used.