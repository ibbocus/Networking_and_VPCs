## What is networking?

A computer network comprises two or more computers that are connected—either by cables (wired) or WiFi (wireless)—with the purpose of transmitting, exchanging, or sharing data and resources. You build a computer network using hardware (e.g., routers, switches, access points, and cables) and software (e.g., operating systems or business applications).

Geographic location often defines a computer network. For example, a LAN (local area network) connects computers in a defined physical space, like an office building, whereas a WAN (wide area network) can connect computers across continents. The internet is the largest example of a WAN, connecting billions of computers worldwide.

You can further define a computer network by the protocols it uses to communicate, the physical arrangement of its components, how it controls traffic, and its purpose.

Computer networks enable communication for every business, entertainment, and research purpose. The internet, online search, email, audio and video sharing, online commerce, live-streaming, and social
networks all exist because of computer networks.

## Computer network types

As networking needs evolved, so did the computer network types that serve those needs. Here are the most common and widely used computer
network types:

- **LAN (local area network):** A LAN connects
computers over a relatively short distance, allowing them to share data, files, and resources. For example, a LAN may connect all the computers in an office building, school, or hospital. Typically, LANs are
privately owned and managed.
- **WLAN (wireless local area network):** A WLAN is just like a LAN but connections between devices on the network are made wirelessly.
- **WAN (wide area network):** As the name implies, a WAN connects computers over a wide area, such as from region to region
or even continent to continent. The internet is the largest WAN, connecting billions of computers worldwide. You will typically see collective or distributed ownership models for WAN management.
- **MAN (metropolitan area network):** MANs are typically larger than LANs but smaller than WANs. Cities and government entities typically own and manage MANs.
- **PAN (personal area network):** A PAN serves one person. For example, if you have an iPhone and a Mac, it’s very likely you’ve set up a PAN that shares and syncs content—text messages, emails, photos, and more—across both devices.
- **SAN (storage area network):** A SAN is a specialized network that provides access to block-level storage—shared network or cloud storage that, to the user, looks and works like a storage drive
that’s physically attached to a computer. For more information on how a SAN works with block storage, see our video "[Block Storage vs. File Storage](https://youtu.be/5EqAXnNm0FE)" and "[Block Storage: A Complete Guide](https://www.ibm.com/cloud/learn/block-storage)."
- **CAN (campus area network):** A CAN is also known as a corporate area network. A CAN is larger than a LAN but smaller than a WAN. CANs serve sites such as colleges, universities, and business
campuses.
- **VPN (virtual private network):** A VPN is a secure, point-to-point connection between two network end points (see ‘Nodes’ below). A VPN establishes an encrypted channel that keeps a user’s
identity and access credentials, as well as any data transferred, inaccessible to hackers.

## Important terms and concepts

The following are some common terms to know when discussing computer networking:

- **IP address**: An IP address is a unique number assigned to every device connected to a network that uses the Internet Protocol for communication. Each IP address identifies the device’s host network and the location of the device on the host network. When one device sends data to another, the data includes a ‘header’ that includes the IP address of the sending device and the IP address of the
destination device.

    Addresses in IPv4 are 32-bits long. This allows for a maximum of 4,294,967,296 (232) unique addresses. Addresses in IPv6 are 128-bits, which allows for 3.4 x 1038 (2128) unique addresses.

    168.212.226.204 - This IPv4 address can be converted into a 32 bit number as seen below 

    [10101000]=168.[11010100]=212.[11100010]=226.[11001100]=204

    ### IPv4 address exhaustion

    The original IPv4 specification was designed for the DARPA network that would eventually become the internet. Originally a test network, no one contemplated how many addresses might be needed in the future. At the time, the 232 addresses (4.3 billion) were certainly considered sufficient. However, over time, it became apparent that as currently implemented, the IPv4 address space would not be big enough for a worldwide internet with
    numerous connected devices per person. The last top-level address blocks were allocated in 2011.

- **Nodes**: A node is a connection point inside a network that can receive, send, create, or store data. Each node requires you to provide some form of identification to receive access,
like an IP address. A few examples of nodes include computers, printers, modems, bridges, and switches. A node is essentially any network device that can recognize, process, and transmit information to any other network node.
- **Routers**: A router is a physical or virtual device that sends information contained in data packets between networks. Routers analyze data within the packets to determine the best way for the information to reach its ultimate destination. Routers forward data packets until they reach their destination node.
- **Switches**: A switch is a device that connects other devices and manages node-to-node communication within a network, ensuring data packets reach their ultimate destination. While a router
sends information between networks, a switch sends information between nodes in a single network. When discussing computer networks,
‘switching’ refers to how data is transferred between devices in a network. The three main types of switching are as follows:
    - *Circuit switching*, which establishes a dedicated communication path between nodes in a network. This dedicated path assures the full bandwidth is available during the transmission, meaning no other traffic can travel along that path.
    - *Packet switching* involves breaking down data into independent components called packets which, because of their small size, make fewer demands on the network. The packets travel through the
    network to their end destination.
    - *Message switching* sends a message in its entirety from the source node, traveling from switch to switch until it reaches its destination node.
- **Ports**: A port identifies a specific connection between network devices. Each port is identified by a number. If you think of an IP address as comparable to the address of a hotel, then
ports are the suites or room numbers within that hotel. Computers use numbers to determine which application, service, or process should
receive specific messages.
- **Network cable types**: The most common network cable types are Ethernet twisted pair, coaxial, and fiber optic. The choice of cable type depends on the size of the network, the arrangement of
network elements, and the physical distance between devices.

### Subnet masks

A single IP address identifies both a network, and a unique interface on that network. A subnet mask can also be written in dotted decimal notation and determines where the network part of an IP address ends, and the host portion of the address begins.

When expressed in binary, any bit set to one means the corresponding bit in the IP address is part of the network address. All the bits set to zero mark the corresponding bits in the IP address as part of the host
address.

The bits marking the subnet mask must be consecutive ones. Most subnet masks start with 255. and continue on until the network mask ends. A Class C subnet mask would be 255.255.255.0.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/410823cb-91fd-4fdd-a8a3-8e707bdbc963/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/410823cb-91fd-4fdd-a8a3-8e707bdbc963/Untitled.png)

**Class A**

In a Class A network, the first eight bits, or the first dotted decimal, is the network part of the address, with the remaining part of the address being the host part of the address. There are 128 possible Class A networks.

```
0.0.0.0 to 127.0.0.0
```

However, any address that begins with 127. is considered a loopback address.

**Example for a Class A IP address:**

```
2.134.213.2
```

**Class B**

In a Class B network, the first 16 bits are the network part of the address. All Class B networks have their first bit set to 1 and the second bit set to 0. In dotted decimal notation, that makes 128.0.0.0 to 191.255.0.0 as Class B networks. There are 16,384 possible Class B networks.

**Example for a Class B IP address**:

```
135.58.24.17
```

**Class C**

In a Class C network, the first two bits are set to 1, and the third bit is set to 0. That makes the first 24 bits of the address the network address and the remainder as the host address. Class C network addresses range from 192.0.0.0 to 223.255.255.0. There are over 2 million possible Class C networks.

**Example for a Class C IP address:**

```
192.168.178.1
```

**Class D**

Class D addresses are used for multicasting applications. Unlike the previous classes, the Class D is not used for "normal" networking operations. Class D addresses have their first three bits set to “1” and their fourth bit set to “0”. Class D addresses are 32-bit network addresses, meaning that all the values within the range of 224.0.0.0 – 239.255.255.255 are used to uniquely identify multicast groups. There are no host addresses within the Class D address space, since all the hosts within a group share the group’s IP address for receiver purposes.

**Example for a Class D IP address:**

```
227.21.6.173
```

**Class E**

Class E networks are defined by having the first four network address bits as 1. That encompasses addresses from 240.0.0.0 to 255.255.255.255. While this class is reserved, its usage was never defined. As a result, most network implementations discard these addresses as illegal or undefined. The exception is 255.255.255.255, which is used as a broadcast address.

**Example for a Class D IP address:**

```
243.164.89.28
```

**Overview: IP address classes and bit-wise representations**

```
Class A
  0.  0.  0.  0 = 00000000.00000000.00000000.00000000
127.255.255.255 = 01111111.11111111.11111111.11111111
                  0nnnnnnn.HHHHHHHH.HHHHHHHH.HHHHHHHH

Class B
128.  0.  0.  0 = 10000000.00000000.00000000.00000000
191.255.255.255 = 10111111.11111111.11111111.11111111
                  10nnnnnn.nnnnnnnn.HHHHHHHH.HHHHHHHH

Class C
192.  0.  0.  0 = 11000000.00000000.00000000.00000000
223.255.255.255 = 11011111.11111111.11111111.11111111
                  110nnnnn.nnnnnnnn.nnnnnnnn.HHHHHHHH

Class D
224.  0.  0.  0 = 11100000.00000000.00000000.00000000
239.255.255.255 = 11101111.11111111.11111111.11111111
                  1110XXXX.XXXXXXXX.XXXXXXXX.XXXXXXXX

Class E
240.  0.  0.  0 = 11110000.00000000.00000000.00000000
255.255.255.255 = 11111111.11111111.11111111.11111111
                  1111XXXX.XXXXXXXX.XXXXXXXX.XXXXXXXX
```

# IPv4 vs IPv6

- IPv4 is 32-Bit IP address whereas IPv6 is a 128-Bit IP address.
- IPv4 is a numeric addressing method whereas IPv6 is an alphanumeric addressing method.
- IPv4 binary bits are separated by a dot(.) whereas IPv6 binary bits are separated by a colon(:).
- IPv4 offers 12 header fields whereas IPv6 offers 8 header fields.
- IPv4 supports broadcast whereas IPv6 doesn’t support broadcast.
- IPv4 has checksum fields while IPv6 doesn’t have checksum fields
- IPv4 supports VLSM (Virtual Length Subnet Mask) whereas IPv6 doesn’t support VLSM.
- IPv4 uses ARP (Address Resolution Protocol) to map to MAC address whereas IPv6 uses NDP (Neighbour Discovery Protocol) to map to MAC address.

## Features of IPv4

- Connectionless Protocol
- Allow creating a simple virtual communication layer over diversified devices
- It requires less memory, and ease of remembering addresses
- Already supported protocol by millions of devices
- Offers video libraries and conferences

## Features of IPv6

- Hierarchical addressing and routing infrastructure
- Stateful and Stateless configuration
- Support for quality of service (QoS)
- An ideal protocol for neighboring node interaction


# How to set up a VPC on AWS
### Create a customer gateway
1. Create VPC
    1. Configuration 
1. Open the Amazon VPC console.
2. In the navigation pane, under VPN Connections, choose Customer Gateways.
3. Choose Create Customer Gateway.
4. Enter a meaningful name for the customer gateway.
5. Choose an option for Static or Dynamic routing.
6.Enter the public IP address of your customer gateway device.
(Optional) Enter your BGP ASN if you selected the option for dynamic routing.  
8.Choose Yes, Create.


### Create VPC
1. Ensure region is ``Ireland ``
2. Click on ```Your VPC```
3. Create VPc ```NOT``` from ```Launch Wizard``` . To ```create VPC``` click button. 
![Step1](images/step%201.png)
    #### Configuration 
    1. Configure the settings as seen below:
    ![Step 2](images/step 2.png)
    #### ```NOTE: The IP address can anything, 255 or below in first two numbers ``` 

### Create a Internet  gateway
1. In the Amazon VPC console, under VPN Connections, choose Virtual Private Gateways.
2. Choose Create Virtual Private Gateway.
3. Enter a meaningful name for the virtual private gateway.
4. Click Create Internet gateway
![step 3](images/step 3.png)
5. Select the new virtual private gateway and open the context (right-click) menu, and then choose Attach to VPC.

### Creating Public and Private Subnet
1. Click on subnets - create subnets
2. Give appropriate tag name
3. Select the VPC that was made earlier
4. Create ```IPv4 CIDR block*``` that slightly differs from the ```VPC CIDR``` as shown below:
![step 4](images/step 5.png)
5. ```REDO``` steps 1-4 but change public to private
#### ```NOTE: it is suggested to add just one more to the IPv4 CIDR block```

### Create a route table

1. check route table not assoicated with VPC already - keep for now - rename

2. Select route tables, create route table

3. Add tag =YourDepartmentNameAndID.YourName.Route.Public

4. Select your VPC

5. Create vpc

6. Edit Route - add 0.0.0.0/0 - target = internet gateway, choose your internet gateway

7. Subnet associations - edit subnet associations - add public subnet

### Security Group Rules - NACLs
#### Egress rules

- Defualt 0.0.0.0/0 auto set
- Allows everything to exit
- Ingress rules (rules for entry)
- NACLs for public
- By default outbound traffic is denied
- Rule numbers matter
- can deny IP as well as allow

    #### Ingress rules
    - port 22 from our IP
    - 80 for inter
    - 443
    - ephemeral on 0.0.0.0/0
    - 27017 to allow connection to private (db) subnet
    #### Egress rules
    
    - Allow all for now
    - Rules for public server

allow all outbound traffic to public server (245.20.1.0/24)xc
ingress 27017 from public server (245.20.1.0/24)
### Create NACL

![1st gif](images/1st%20gif.gif)

### Create Instance
1. Follow the gif to create the instance
![2nd gif](images/2nd%20gif.gif)

## Testing - Inside GitBash
1. create an ec2 instance with VPC of the one just created

2. ssh into the instance

3. run sudo apt-get install nginx

4. go onto your browser and insert the IP of the instance created

5. if VPC has been created effectively then you will Nginx install successful
