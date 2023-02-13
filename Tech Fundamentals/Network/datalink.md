# Data Link (Layer 2)
![Layer 2](../images/switch.webp)

## Frame
Requires a functional `layer 1` network to operate.
`Frames` are a format for sending information over a `layer 2` network. It also introduces a unique hard address, called a `MAC` address for every device on the network.

## MAC Adress
* 48 bits in hex. eg: (3e:22:fb:b9:5b:75)
* 24 bits for manufacturer
* Frames can be addessed to destination or broadcast (ALL F's)

## Frame Breakdown
Is a container. 1-4 make up what is known as the `MAC HEADER`.<br>
The `PAYLOAD` is the data the frame carries from the `source` to the `destination`. It's generally provided by `Layer 3` and the `EtherType (ET)`.

1. PREAMBLE | 56 Bits | SFD 8 Bits (Allow devices to know its the start of the frame)
2. Destination MAC Address
3. Source MAC Address
4. ET | 16 Bits (Specify which layer protocol is putting its data inside the frame.)
5. Payload (46 - 1500 BYTES)
6. FCS | 32 bits