# class 17 TCP Servers

the TCP is a protocol that uses to connect between servers and computers it uses to send a package of data with some rules and since the event used in server, the use of TCP become easer

## the structure of package

Byte 0: Source port
Byte 3: Destination port
Byte 4: Sequence number
Byte 8: Acknowledgement number
Byte 12: Data Offset, NS flag, and 3 undefined bits
Byte 13: CWR, ECE, URG, ACK, PSH, RST, SYN, and FYN flags
Byte 14: Window size
Byte 16: Checksum
Byte 18: Urgent pointer
Byte 20: Options


a 16 bit source port
a 16 bit destination port
a 32 bit sequence number that sets the initial sequence number and manages the accumulated sequence number
if ACK is set it contains a 32 bit acknowledgement number that is the next sequence number that the sender is expecting. It is used for acknowledging the bytes it has so far received
a 4 bit data offset specifies the size of the tcp header in 32 bit words.
9 flag bits
NS - an experimental feature for a nonce sum - a nonce is a random cryptographic number used to prevent people from lying about who they are (authentication)
CWR - used to acknowledge that a TCP segment with the ECE flag has been received, and the Window has been reduced to alleviate congestion
ECE - if SYN is 1 it indicates that the peer is ECN capable, other otherwise its used to indicate that there is network congestion.
URG - indicates that the Urgent pointer filed is significant
ACK - indicates that the ACK field is significant - all packets after the initial SYN should have this flag set
PSH - used to ask to push the buffered data to the receiving application.
RST - used to reset the connection
SYN - sent only on the first packet sent from each end to synchronize the sequence numbers
FIN - indicates the last package from a sender, and is used in closing a connection
a 16 bit window size
a 16 bit checksum used for error checking the header
if URG is set it contains a 16 bit urgent Pointer
a variable 0 to 320 bit (divisible by 32) options section

## Connection Establishment

also TCP use protocol to know of the package sent by receiving response

## Connection Termination

to make sure the session has been ended they sent segment to end it and wait to receive the ending response then end it