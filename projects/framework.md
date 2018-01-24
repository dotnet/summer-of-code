## Prototype .NET HttpClient over QUIC protocol

**Complexity:** Hard

QUIC is emerging network protocol, which provides performance wins compared to TCP+TLS stack. Managed HttpClient is built-in .NET library, implemented in C# over TCP+TLS.
The goal is to prototype QUIC protocol implementation in C#, using low-level language primitives and features for high performance, and no-allocations. The next step will be to plug in the transport protocol into managed HttpClient implementation.

**Deliverables:** Library which can send and receive data via HttpClient using QUIC protocol.

**Mentors:** Karel Zikmund

## Create portable ILDasm library

**Complexity:** Medium

Having a portable ILDasm library would allow people on non-windows machines to disassembly IL code. We already have a library that sets the foundations of this in CorefxLabs.
The work would require creating an object model on top of the Metadata Reader work that another one of our interns did.

**Deliverables:** Library which can be used to disassemble a given managed assembly 

**Mentors:** Alexandru Ghiondea
