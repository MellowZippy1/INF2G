---
PDU: Frame
---
- How to define a format to avoid misinterpretation?

The data link assumes that we can send bits correctly, because this is the [physical layer](01%20Physical)'s responsibility. The data link's main concern is formatting the message to avoid misinterpretation. This is called [framing](02%20Data%20Link#Framing). It has to make sure that the correct data is sent to the correct destination. It also has to make sure that all [bit errors](02%20Data%20Link#Error%20detection) are detected.

# Responsibilities

- It has to make sure that messages are [format](02%20Data%20Link#Framing) correctly.
- It has to make sure all [bit errors](02%20Data%20Link#Error%20Detection) are detected.
- It has to make sure that the correct data is delivered to the correct destination.

The data link layer transforms the [physical layer](01%20Physical) (a raw transmission facility) into a reliable link and makes the physical layer appear error-free to the upper layer.
# Framing

The data link layer gets **split data** and has to put this into **frames**. For each segment, some extra data (metadata) is added to define: 

1. Who is the sender
2. Who is the receiver
3. Length of the segment
4. Type of segment
5. Error checking codes

Data and metadata are put in a single message called a frame.

![[Pasted image 20240212164159.png]]
# Error detection

[Transmission](Transmission) channels are not always error-free. In case of an error it should be detected and the message should be re-transmitted, if possible.

Detecting these errors requires specific algorithms:
- [Parity bit](Parity%20Bits)
- [CRC](CRC)
