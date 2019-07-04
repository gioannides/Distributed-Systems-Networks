<div align="center">
  <img src="net.jpg">
  <br>
</div>

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


# Instructions

Run install.sh (or install.bat on Windows) to obtain the appropriate build and execution scripts which are described below.

The class MessageInfo (in the common folder) provides a container for the data to be sent and
also has a constructor that extracts the data from a string representation. Outline code for each
of the client/server pairs can be found in the rmi and udp folders.

The file policy is a simple configuration file required for the RMI code. More constrained
policies are possible, but this should provide the lowest barrier to testing.

The Makefile allows Linux users to use make to compile the various parts of the exercise. It
can also be used to help configure the preferred development environment with the correct
commands, flags and parameters. Windows users can use the build.bat script to compile the
exercise in the same way. The other shell scripts (rmiclient (.bat or .sh) etc.) allow users to
execute the various parts of the exercise.
