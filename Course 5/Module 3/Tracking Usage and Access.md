- **Accounting** is the final component of the AAA (Authentication, Authorization, and Accounting) security framework, **focusing on keeping records of user activities and resource usage**.
- **Accounting systems** are **responsible for logging and tracking the resources and services** accessed by users and capturing their actions within the system.
- **Auditing is an important aspect of accounting**, involving the review of these records to ensure compliance, detect anomalies, and identify any unauthorized or suspicious activities.
- The specifics of what accounting systems track depend on their purpose and intent. For example, a TACACS+ server primarily focuses on user authentication, tracking the devices they authenticate to and the commands they execute during their session.
- TACACS+ is commonly used for device access control, managing user access to network devices and monitoring their activities.
- Cisco's AAA system, which incorporates TACACS+, supports accounting of individual commands executed, connections to and from network devices, privileged mode operations, network services usage, and system events such as configuration reloads or reboots.
- On the other hand, RADIUS (Remote Authentication Dial-In User Service) focuses on network access control and tracks details like session duration, client location, and resource usage during the session.
- RADIUS accounting starts with the network access server (NAS) sending an accounting request packet to the accounting server, containing an event record to be logged. This initiates the accounting session on the server.
- The accounting server responds with an accounting response to acknowledge the receipt of the message. The NAS continues sending periodic accounting messages with session statistics until an accounting stop packet is received.
- RADIUS accounting can be utilized for billing purposes by Internet Service Providers (ISPs) as it records session duration and the amount of data transmitted and received by the user.
- This data can also be used to enforce data or time quotas, limiting session durations or restricting the amount of data that can be transferred.
- However, accounting information in RADIUS is not detailed and typically does not include specific information about the user's activities during the session, such as visited websites or used protocols.

In summary, accounting within the AAA framework is crucial for maintaining records of user activities, resource usage, and system events. It helps monitor and track user access, detect anomalies, and can be utilized for billing and quota enforcement purposes.

#accounting #auditing #course5-module3 