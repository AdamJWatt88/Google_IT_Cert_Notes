- **TCP** is a **connection-oriented protocol** that establishes a connection and ensures that all data is properly transmitted through constant **acknowledgments**. This is important because the internet is a busy and unpredictable place where many things could go wrong during data transmission.
- If even a single bit is not transmitted properly, the resulting data can be incomprehensible for the receiving end. **Connection-oriented protocols** like **TCP** protect against this by forming connections and using acknowledgments.
- **Lower-level protocols** like **IP** and **Ethernet** use **check sums** to ensure that all received data is correct, but it's up to TCP to determine when to resend data that doesn't pass the check.
- TCP's use of **sequence numbers** allows for all the data to be put back together in the right order even if some segments arrive out of order due to errors at lower layers.
- **Connection-oriented protocols** like **TCP** have a lot of overhead as they require connection establishment, constant acknowledgments, and connection teardown. They are useful when it's critical to ensure that data reaches its destination.
- **UDP** is a connectionless protocol that doesn't rely on connections and doesn't support acknowledgments. It's useful for messages that aren't super important, such as streaming video.
- **UDP** allows for higher quality video as it eliminates the overhead of **TCP** and saves more bandwidth for actual data transfer.

#tcp #connection-oriented-protocols #udp #course2-module3 