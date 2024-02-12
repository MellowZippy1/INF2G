A ping (Packet internet or Inter-Network Groper) is a basic internet program that allows a user to test and verify if a particular destination IP address exists.
It is essentially a combination of [Internet Control Message Protocol](ICMP.md) echo requests and response messages.

### How does ping work?

The ping command **first sends an echo request packet to an address, then waits for a reply**. The ping is successful only if: the echo request gets to the destination, and. the destination is able to get an echo reply back to the source within a predetermined time called a timeout