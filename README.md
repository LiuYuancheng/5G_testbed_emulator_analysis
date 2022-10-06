# 5G testbed components 

Reference link: 

https://futurenetworks.ieee.org/topics/5g-testbed

https://www.digi.com/blog/post/5g-network-architecture

https://www.sdxcentral.com/5g/definitions/key-elements-5g-network/5g-network-slicing/

https://www.keysight.com/us/en/products/modular/reference-solutions/5g-waveform-generation-analysis-testbed-reference-solution.html

https://www.ericsson.com/en/5g/5g-networks

### 5G physical testbed feature:

Normal test bed features:

- Faster data transmission speed, up to multi-Gigabit/s speeds.
- Greater capacity, fueling a massive amount of IoT devices per square kilometer.
- Lower latency, down to single-digit milliseconds, which is critically important in applications such as [connected vehicles in ITS applications](https://www.digi.com/blog/post/5g-iot-and-the-future-of-connected-vehicle) and autonomous vehicles, where near instantaneous response is necessary. 
- Support low, mid and high-band spectrum – from licensed, shared and private sources: 5G high-band (mmWave), 5G mid-band operates in the 2-6 GHz range, 5G low-band operates below 2 GHz.

![](5g1.png)





### 5G testbed core network components

The 5G core uses a cloud-aligned service-based architecture (SBA) to support authentication, security, session management and aggregation of traffic from connected devices, all of which requires the complex interconnection of network functions.

the components of the 5G core network architecture include:

- User plane Function (UPF) [**NCL**: we may provide]
- Data network (DN), e.g. operator services, Internet access or 3rd party services [**NCL**: we can provide]
- Core Access and Mobility Management Function (AMF) [**NCL**: we may provide]
- Authentication Server Function (AUSF) [**NCL**: we may provide]
- Session Management Function (SMF) [**NCL**: we may provide]
- Network Slice Selection Function (NSSF) [**NCL**: we may provide]
- Network Exposure Function (NEF) [**NCL**: difficult]
- Network Function Repository Function (NRF) [**NCL**: let customer/researcher add ]
- Policy Control function (PCF)[**NCL**: we may provide]
- Unified Data Management (UDM) [**NCL**: we may provide]
- Application Function (AF) [**NCL**:  let customer/researcher add]

![](5g2.png)



Here's how the components works:

- **User Equipment (UE)** like 5G smartphones or 5G cellular devices connect over the 5G New Radio Access Network to the 5G core and further to **Data Networks (DN)**, like the Internet.
- The **Access and Mobility Management Function (AMF)** acts as a single-entry point for the UE connection.
- Based on the service requested by the UE, the AMF selects the respective Session Management Function (SMF) for managing the user session.
- The **User Plane Function (UPF)** transports the IP data traffic (user plane) between the User Equipment (UE) and the external networks.
- The **Authentication Server Function (AUSF)** allows the AMF to authenticate the UE and access services of the 5G core.
- Other functions like the **Session Management Function (SMF)**, the **Policy Control Function (PCF)**, the **Application Function (AF)** and the **Unified Data Management (UDM)** function provide the policy control framework, applying policy decisions and accessing subscription information, to govern the network behavior.



Network Slicing [We may be able to provide 5G network slicing simulation] : 

A 5G network operator may offer one slice that is optimized for high bandwidth applications, another slice that's more optimized for low latency, and a third that's optimized for a massive number of IoT devices. Depending on this optimization, some of the 5G core functions may not be available at all. For example, if you are only servicing IoT devices, you would not need the voice function that is necessary for mobile phones. And because not every slice must have exactly the same capabilities, the available computing power is used more efficiently.

![](5g3.png)

5G test bed example:



- **5G RuralFirst**—tested spectrum sharing and other networking technologies in hard-to-reach [remote areas](https://futurenetworks.ieee.org/home/sitemap/13-education/214-5g-networks-for-rural-and-remote-areas-applications)
- **5G Smart Tourism**—demonstrated virtual reality and augmented reality technologies to enhance visitor experiences at museums and festivals
- **Worcestershire 5G Consortium**—used robotics, augmented reality, and data analytics to optimize manufacturing
- **Liverpool 5G Testbed**—deployed 5G technology to elderly people living independently to address loneliness and improve communication with hospitals
- **AutoAir**—explored 5G technology in autonomous vehicles as well as air and rail transportation
- **5G Rural Integrated Testbed**—connected residents in rural communities and tested drones and machine learning to optimize farming



Use OpenStack as cloud/edge computing solutions: https://5ginfire.eu/university-of-bristol-5g-testbed/