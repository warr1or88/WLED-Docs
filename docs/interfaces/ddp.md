---
title: DDP protocol
hide:
  # - navigation
  # - toc
---

# Distributed Display Protocol

NOT TO BE CONFUSED WITH UDP.

DDP is a protocol designed by 3waylabs outlined [here on their website](http://www.3waylabs.com/ddp/).

WLED listens for DDP packets on port 4048, as outlined by the protocol.
Check the [DDP documentation](http://www.3waylabs.com/ddp/) for more info about packet structure.

**Notice*
WLED does not read the optional timecodes in DDP packet headers. 
If you are implementing the protocol to send packets to WLED, do not bother implementing it

## Example implementations

 - [ddp-rs](https://github.com/coral/ddp-rs) A Rust library for sending (and even receiving) DDP packets.
 - [LedFX/devices/ddp.py](https://github.com/LedFx/LedFx/blob/main/ledfx/devices/ddp.py) LedFX's implementation for sending DDP packets to WLED