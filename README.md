# full-speed-usb-hub
4 port USB2.0 HUB limit by full speed (slow like 1.1)

## Motivation
My DIY USB hardware is susceptible to noise and cannot reliably carry high-bit-rate signals over inexpensive jumper wires.  
To work around this, I used a legacy USB 1.1 low-bit-rate device: by inserting a USB 1.1 hub I could force the link to downgrade, which solved the problem completely.  
Unfortunately, USB 1.1 devices are now out of stock, so I can no longer apply the same workaround.

I have recently found a USB 2.0 isolator chip. Although USB 2.0 normally operates at 480 Mbps (Hi-Speed), this chip limits the data rate to 12 Mbps or 1.5 Mbps while still conforming to the USB 2.0 protocol. Because the lower data rate uses lower signalling frequencies, it should mitigate the noise issues just as USB 1.1 did.

## Solution
- **ADuM4160** — USB 2.0 isolator chip  
- **CH334P** — USB 2.0 hub-controller chip

## Dependency Library
- [TLV73330PDBVR](https://www.snapeda.com/parts/TLV73330PDBVR/Texas%20Instruments/view-part/?ref=search&t=TLV73330PDBVR)

