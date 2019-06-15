# Distributed Systems-Networks

The purpose of the exercise is to gain experience of coding RMI and UDP as well as to compare them
for relative reliability and ease of use.
For each case a simple client was written that passes a specified number of messages to a
server. Each message contains a message sequence number and the total number of messages to
be sent. The server keeps track of the messages received and, when there are no more messages, outputs
a summary of the number of messages received and also which ones were lost.


When the clients and servers for each communication mechanism are working, some experiments were ran
on 2 computers in different parts of a lab at Imperial College London (i.e., not physically near each other), sending increasing
numbers of messages (e.g., from 20-100 with increments of 20, then, 200, 300 and 400) and the
situations in which messages are lost were identified.
