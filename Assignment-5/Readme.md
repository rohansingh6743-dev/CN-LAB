Experiment 5 Design and simulate flow control and error control protocols such as Stop and Wait, Go-Back-N ARQ, and Selective Repeat ARQ using Cisco Packet Tracer. Compare their performance in terms of throughput and efficiency under varying network conditions.

In data communication, reliable transmission of data is very important. Two key mechanisms used to ensure reliability are flow control and error control.

Flow Control Flow control ensures that the sender does not send data faster than the receiver can handle. If data is sent too fast: • Receiver buffer may overflow • Packets may be lost Therefore, flow control maintains a balanced data transmission rate. Error Control Error control ensures that data is transmitted correctly without errors. Errors may occur due to: • Noise in the communication channel • Signal interference • Network congestion Error control techniques: • Detect errors • Retransmit lost or corrupted data

ARQ Protocols (Automatic Repeat reQuest) ARQ protocols are used for error detection and retransmission of lost or damaged frames.

Stop and Wait ARQ • Sender sends one frame at a time • Waits for acknowledgment (ACK) • If ACK not received → retransmit Advantages: • Simple and reliable Disadvantages: • Slow (low throughput)

Go-Back-N ARQ • Sender can send multiple frames continuously • Uses a window size • If one frame is lost: • All frames after it are retransmitted Advantages: • Faster than Stop and Wait Disadvantages: • Wastes bandwidth (retransmits many frames)

Selective Repeat ARQ • Sender sends multiple frames • Only incorrect or lost frames are retransmitted Advantages: • High efficiency • Better throughput Disadvantages: • More complex

Basic Setup Steps:

Build topology with: o 1 switch + 2 PCs Assign IPs (same network) Use Simulation Mode Start pings: o PC0 → PC1
