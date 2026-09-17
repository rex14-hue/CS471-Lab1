# CS471 – Web Technologies
## Lab 1: The Internet Protocols
### Wireshark – HTTP, TCP/IP and UDP Analysis

---

## Part 1: Capturing HTTP Traffic

### HTTP Request
The HTTP GET request was captured using Wireshark.

![HTTP Request](images/01_HTTP_Request.png)

### HTTP Response
The server returned an HTTP 200 OK response.

![HTTP Response](images/02_HTTP_Response.png)

---

## Part 2: Analyzing TCP/IP Traffic

### Follow TCP Stream
The TCP stream shows the communication between the client and the server.

![TCP Stream](images/03_TCP_Stream.png)

### TCP Three-Way Handshake
The connection was established using SYN, SYN-ACK, and ACK.

![TCP Handshake](images/04_TCP_Handshake.png)

### Sequence and Acknowledgment Numbers
The SYN-ACK packet shows relative Sequence Number = 0 and Acknowledgment Number = 1.

![TCP Sequence and ACK](images/05_TCP_Seq_Ack.png)

### TCP Data Transfer
The captured TCP segment contains 1300 bytes of data.

![TCP Data Transfer](images/06_TCP_Data.png)

### TCP Termination
FIN-ACK and ACK packets were observed during connection termination.

![TCP Termination](images/07_TCP_Termination.png)

---

## Part 3: Capturing and Analyzing UDP Traffic

The selected UDP packet contains the following information:

| Field | Value |
|---|---|
| Source Port | 8803 |
| Destination Port | 59253 |
| UDP Length | 158 bytes |
| UDP Payload | 150 bytes |

![UDP Analysis](images/08_UDP_Analysis.png)

---

## Part 4: Comparing TCP and UDP

### Table 1: TCP or UDP? Provide Reasons

| Feature | TCP or UDP | Reasons |
|---|---|---|
| Reliability and Connection Establishment | TCP | TCP establishes a connection using a three-way handshake and provides reliable delivery through acknowledgments and retransmissions. |
| Data Integrity and Ordering | TCP | TCP uses checksums to detect errors and sequence numbers to deliver data in the correct order. |

### Table 2: Use Cases and Performance

| | TCP | UDP |
|---|---|---|
| Use Cases | Web browsing, email, and file transfer. | Online gaming, VoIP, and live streaming. |
| Performance | More overhead due to connection setup, acknowledgments, and retransmissions. | Lower overhead and no connection setup, making it suitable for real-time applications. |


