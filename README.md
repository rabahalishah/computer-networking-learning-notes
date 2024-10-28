# Computer Networking Full Course
# Introduction to computer network & OSI model.
The main purpose of Computer network is to share the data. The data can be share once the connection is established. But the data which has sent from the sender and received by the receiver is in the same format as it supposed to be? Or receiver is being able to understand what does that shared data means? All these things are done by a protocol which is running on the both side. On sender and on receiver as well. 

Example:
You press a key on a keyboard and it displays on the screen. here the data is also get shared between the keyboard and screen via some connections and protocol. Here both sender and receiver both lies on the same device. Here it would be called inter process communication. Does this communication is deal by computer network? the answer is No. such type of communication is deal by operating system.

Computer network is basically here to deal with the data sharing between two separate device present at different location. Such as client and server. But the main purpose of the computer network is to provide such an environment to both client and server such that they feel like that both are present at same computer but in actual they are not.

So in our practical daily example of google. we send request to google server we get response so fast that we think both are at same computer. This is done by computer network.

********Functionality of Computer networks
There are two kind of functionality
1) Mandatory: These are functoinalities that we cannot ignore when client is sending request to ther server. 
	a) Error Control: Error handling functionalities like in case of any error at least I can get the error so I can fix it later.
	b) Flow Control: How much data should I send.
	c) Multiplex and Demultiplex: In case of several processes are running and several requests are being made. Then we have to check which request has 	sent for which process
2) Optional: 
	a) Cryptography (means Encryption, it is optional by implementing such algorithms my performance can compromise
	b) checkpoint: Checkpointing our data so that in case of downloading fail. The downloading should be resumed from where it had left.






************************Physical Layer
Physical layer as its name suggests it will deal with the hardware part. It is the last layer of OSI model.
It will be the last layer which will add its functionality on sender side. And it is the 1st layer which will add its functionality on receiver side.

All data converts into bits and then send to the receiver in the form of signal via a transmission medium and on receiver side this signal get converted back to bits

The conversion of signal from bits to signal and then it transmission to receiver and then again converting back into bits is all done by physical layer.

*********************Functinalities of Physical Layer:
1) cables and connectors: Which cable we are using as medium. Coaxial, copper, optical fiber etc. And which type of connectors we are using to connect the cables such as BNC, RJ, CAT, SC, 				LC etc.
2) Phyical Topology: How to connect various devices? such as star topology, bus topology, mesh topology, point-to-point configuration etc. All is deal by physical topology.
3) Hardware (Repeaters and hubs): Repeaters are used to give energy to the signal in case of noises. Hubs are used make multi connections or used to connect mutliple computers together 					etc.
4) Transmisson mode: What tranmission mode? one can send signal and cannot get signal in back. TV receives signal cannot send back. One way tranimission.
5) Multiplexing: Converting n number of signals in 1 signal and converting back 1 signals into n signals
6) Encoding: Different encoding methods such as analogue to analogue encoding etc. 


******************Manchester and differential manchester.
The data travels in analogue from so their conversion from digital data that is 0 1 to anaglogue is done by manchester.
There are some conventions like for 0 and 1 you can google those conventions and simply connect them.





---------------Physical Layer: Types of cables in computer network



*****************************************Computer Network

COMPUTER Full form

C: Commonly 
O: oriented 
M: machine 
P: particularly  
U: used for 
T: training
E: education and
R: research.


What is computer network?
computers connected together is a computer network and collection of the computer network is called internet.

***********How it all started?
**History:
Cold war was going on between US and soviet uninion (Russia). They were like who would be the firts one to launch the satellite and who would be the first one to land on moon and so on. In launching the first satellite Russia won. America didnt like that thing. he wanted to be the first so they created a department called ARPA. (Advance Research Projects Agency) later on in 1972 it was renamed as DARPA (Defense Advance Research Projects Agency). They created buildings then they thought the buildings are so far how would we communicate each other? They created a network called ARPANET. Let say 4 buildings MIT, Standford, VCLA, univeristy of Utah. They were connected to each other with TCP (Transmission contorl protocol). This was the first internet network model which was established. with the passsage of time more and more computers were added to this network. This was only researched oriented. The problem was that if there is a link in a document which is linked to the other document that cannot be access at that time (hyperlink concept was not there). This was missing at that time. So then Tim Berner introduced www world wide web to solve this link problem. www allows you to store data and link data. www is system where information is linked with other document via hyper links and are accessible over the internet. 

How do we search the pages? At the time you couldn't as there was not any search engine. You just have to go via hyperlinks from one page to another. Then later we had to develop search engine. Yahoo was the first search engine.

URLs (Uniform resource Locators)


****************Protocols and why we need them?
Protocols: Different tyeps of rules set by the humans to transfer data over the internet is called protocols. As we know that we are sending and receiving different type of data such as video text etc. there must be some set of rules which make sure that 100% data has been transfered as it was supposed to send. SO we need protocols. There are several protocols such as TCP/IP (When you want 100% of your data should be transferred such as email), UDP/IP (user datagram protocol: used when you do not care about 100% data transmission e.g, video call, frames can be droped), HTTP (used by browser in client-server architecture).

let say there are two persons in different country making their apps both have their own set of rules to communicate. Will they be able to communicate? NO! In order to communicate they must have same protocols to communicate.

Who is making these protocols and all that stuff? The internet society is responsible for all such protocols and stuff.

*************************Client server Architecture 
You write google.com on you computer and your computer sends request to the google server and then google server sending response back the your computer.

This is a general overview of client server architecture. There is a lot more inside this simple process. There are several protocols etc. 

Believe me all the continents are connected via wires. Internet is not in the cloud. It is under the sea.(https://www.submarinecablemap.com)

Packets: Everything on internet is send and receives in the form of chunks.

IP addresses: Every server on internet have an IP address. Its format something goes like (X.X.X.X) where X can vary between 0-255. Its same as we save a person phone number such as Mom. we just call mom and number will be dialed automatically here MoM is a name that we search on internet and number is its IP address. Its like phone book of internet.

you can check IP address of your ISp (Internet service provider) by this command
> curl ifconfig.me -s


*******************ISP, Global IP address, Local IP address

ISP (Internet service provider) is connected to the internet and ISP is connected with your modem/Router. This router will have a global IP address. All devices connected to this router will have same global IP address. Now internally to differentiate, the router will assign local IP address to each of the device/host connected to it using DHCP (Dynamic hosting configuration protocol). When let say Device 1 having IP1 address make a request to the google the router will make request to ISP and ISP will make request to google server. Here only Global address of your router will be displayed. Google will see only global ip address. Google will take all devices connected to the routers as one device. Then google send response to ISP and then ISP will forward it to your router and your router will decide to which device had made the request to whome this reponse has to send this is done via NAT (Network access translator). In india tier 1 ISP provider is TATA.

**Port numbers: 
Now let say you were runnning multiple online application in your computer or device. Once your device get the response then who will decide which application of this device request for this data? here comes the port number. As IP address helps in selecting the device and port numbers decide which application of this device requested for this response.

In short IP address will identify the devices and Port numbers will identify the application running within that device.


Port numbers are 16 bit numbers. Means 16 cells having 0 and 1. How many combinations can be made?
2^16 = 65,000

SO we can say each device can have 65000 ports numbers.

For all browsing stuff we use HTTP port = 80
For MongoDB we port = 27017
For SQL port = 1433

There are ports from 0 - 1023 which are reserved ports. You cannot use these ports for your application
and there are some other ports from 1024 - 49152
are reserved for some applications such as mongoDB, MySql applications etc. 
remaining ones you can use.

Mbps =  mega bits per second

sending data to other computer is called uploading and getting data from one computer to other computer is called downloading. You uploading and downloading speed depens on your ISP.


There are two type of communication one is guided and other is unguided.

Guided is one that using via cables that is defined. And unguided is like using wireless.

Physical wires:
Unshield twisted pair cable: 10BaseT, 100BaseT (due ot their low signal travel range we use them in LAN where long signal travel is not required)
Coaxial Cable: 10Base2, 100Base5
Fibre Optic: 100BaseFx (travles signal in the form of light)

here: 10, 100 means Mbps (Mega bits per second), Base means Base band means only one signal can travel at a time and T means 100 meters. 2 means 200 meters and 5 means 500 meters and FX means 2km

After their specified ranges the signal will attentaut. Attentuation means the energy of the signal will be down. Thereofore, we use repeaters after specific distances. 

Wireless: radio channels, wifi, bluetooth. These are all for short ranges. 3G, 4G and 5G are for long ranges.

why we used wires instead of satellite? the answer is speed. Wires are faster than satellite.

******************LAN, MAN, WAN
LAN: Local area network like home and room. Uses ethernet cables etc.
MAN: Metropolitin area network. Accross the city
WAN: Wide area network. Accross the country. using optical fiber cables.

Internet is basically a collection of LAN connecting to the MAN and collection of MAN connecting to the WAN creating the whole internet.
1) SONET (Synchronize optical network): This protocol transfer multiple bit streams synchronously.
2) Frame Relay: It is also a std WAN technology. Its basically a way to connect your LAN to WAN.


*********************What are routers

Routers/Modem are basically devices which converts analogue signals to digital signals and vice versa. 
Router routes the data packet on the basis of their IP address.

**********************************Topologies
Topologies simply tells us how to connect different devices together.
To connect devices we need cables and ports.
There are several arrangements to connect the devices such as Mesh, Star, Bus, Ring, Hybrid. 
The important point to here is that if the number of device which are supposed to be connected together are known then how can we tell how many cables and ports are required to connect them.

Let say there are 4 devices connected in mesh topology:
no. of cables = [n(n-1)]/2 = 6 cables would be required
no. of ports of each device = (n-1) = 3
Reliability: means if any of the device get failed is there any way to send its message to other device? In case of 4 devices connected in mesh topology configuration these devices the reliability is High. 
Cost: Is also high
Security: Is high. If one device A is contacting with device B then other devices will have no idea about their communication.

***************Mesh Topology 
Mesh topology supports point to point communication. In this combination each device is connected with every computer. It is expensive as many wires are used and when a new computer is added then it has to be connected with all other computer. It is scalability issue.

***************Tree topology
It is a combination of bus and star/hub topology.

*********Hub Topology
In case of hub topology many device are connected with hub
assume hub in center and other devices are connected with hub like server

Let say there are 4 devices connected in hub topology:
no. of cables = [n(n-1)]/2 = 6 cables would be required
no. of ports of each device = (n-1) = 3
total no. of ports = n(n-1) = 12
Reliability: means if any of the device get failed is there any way to send its message to other device? In case of 4 devices connected in huv topology configuration these devices the reliability is very low. In case of hub failure whole system will be failed no one would be able to communicate.
Cost: low
Security: low. As hub is to communicate in a broadcast way by default. On message sent by A device would be sent to all devices connected with the hub

*******Bus Topology 
In this configuration there is a straight wire called back bone wire of large bandwidth having multiple devices connected with it.
Imagine a stem having several leaves. Here stem is a back bone wire and leaves are devices.

Let say there are 4 devices connected in bus topology:
no. of cables = n+1 = 5 cables would be required
no. of ports of each device = n= 4
Reliability: reliability is very low. As if backbone wire fails whole system will be failed.
Security: security is also low. As all messages will be send through a single wire so all can access them. 

collision is problem in bus topology. As all devices at once sent a single so due to single back bone wire all signals can collide.

*******Ring Topology 
In this configuration there is a circular wire called back bone wire of large bandwidth having multiple devices connected with it.
Imagine a stem in circular ring shape having several leaves. Here stem is a back bone wire and leaves are devices.

Let say there are 4 devices connected in ring topology:
no. of cables = n+1 = 5 cables would be required
no. of ports of each device = n= 4
Reliability: reliability is very low. As if backbone wire fails whole system will be failed.
Security: security is also low. As all messages will be send through a single wire so all can access them. 

collision is problem in bus topology. As all devices at once sent a single so due to single back bone wire all signals can collide.

*************************Structure of the network: OSI Model
All the above discussed processes happen due to OSI model (Open systems interconnection model)
This model is a theoretical model. It has several layers. All messages that are either sending form the sender device or getting received by the receiver device must go through these OSI layers.

7 layers which are heart of OSI model are given below:

1) Application layer: This layer deals with the application stuff such as you messaging app and your browser. You are simply sending files and data etc. with this layer. This layer hands 		      over the data to presentation layer.

2) presentation layer: This layer converts your data such as texts, files etc. into machine representable binary format or you can say it converts from ASCII to EBCDIC. It is also 				responsible for encryption/dcryption or any other conversion of data if needed. It also do abstraction. It assumes that other layers will handle the data coming 			from it. It short this layer is like translation.

3) Session layer: This layer is used to establish the connections such as authentication, authorization etc.whether the required file is on server or not until the session is terminated. 		   Its simply like having an appointment session with a doctor. Session layer assumes that layers below it will do their job. its just have to set the session.

4) Transport layer: This layer deals with the tranfer protocol of data. In transport layer segmentation happens as we know data travels in the form of packets/chunks/segments and every 		packet has its sequence number and port number. Sequence number helps in reassemble the data and where as port number helps to reach it to the desired application. There is 		also a check some which gives the feedback whether the data is completely tranfered or not. TCP/IP for Connection oriented 100% data tranfer no loss of packets. UDP 			connectionless oriented loss of packets such as video calls and games. Flow control is also deal by this layer. a) Error Control: Error handling functionalities like in 		case of any error at least I can get the error so I can fix it later. b) Flow Control: How much data should I send.

5) Network layer: This layer deals with routing. Transmission of data from one computer to another. Here router lives in. This layer assigns IP to every packet from sender to receiver so 		  that each packet get reach to the right destination/device this is called logical addressing. Logical addressing is done by Network layer Each packet will contain 3 			  things in it. Senders IP, receivers IP and subnet mask.

6) Data Link layer: Here data has reached to the right device. This layer receives data packet from network layer containing IP addresses of both sender and receiver and subnet mask. Here 		   mac addresses are assign to senders and receivers data packet this is called physical addressing. Physical addressing is done in this layer so that each packet reaches 		   the right application in the device. Mac address is a 12 digit alphanumeric number. It is assigned to every network controller of your device. the bluetooth of your 		   device can have different mac address and wifi router can have different.

7) phyiscal layer: It is a hardware section. It converts your signal from digital to analogue and vice versa.

**NOTE**: the order will be reversed on receiver side

"AP STN DP"



***********************TCP/IP Protocol*****************
TCP/IP stands for Transmission control protocol/Internet Protocol. There are two models in TCP/IP. One have 5 layers and other 4 layers. In pratical 4 layer model is implemented.
The reason to introduce this protocol was that OSI model was only theoretical model whereas TCP/IP is a practical model. 

Application Layer: Here Application, Presentation and session layers are merged in application layer.
Transport Layer 
Network Layer
Data Link Layer
Physical Layer

"ATN DP"
TCP/IP supports both Client-server architechture (Where one server and several clients are sending request) and peer to peer (users are sending request to each other e.g chat app)

# OSI Model Top View:
![image](https://github.com/user-attachments/assets/142b4a89-c9f3-453b-83cc-f9cfbf56f183)

Before OSI Model there are two things that happen first. If any one of the thing get fails OSI Model layers won't be generated.
1) DNS Resolution (Is there any IP address exists for the request URL?)
2) TCP/IP Handshake (3 way, 2 way, 4 way handshake) (Hi-syn, Ack-Syn, Ack)

L7 - Application - HTTP/FTP Request got initiated
L6 - Presentation Layer - Encryption
L5 - Session Layer - Browser Session is maintained
L4 - Transport / Segmentation Layer - Data Segmentation or Data Packets And Which Protocol to use TCP/UDP
L3 - Networking Layer / Router - Choosing the shortest path, hopping from router to router.
L2 - Data Link Layer (Frames (MAC)) - Switches do not understand IP addresses so in each data packet we put MAC address as well along with the source and destination IP. Switches uses frames (MAC to identify the which component of the 
				      device is targeted
L1 - Physical Layer - optical fiber etc.

### TCP-IP Model
Since Layer 7, 6, and 5 are deal by the browser only. So, in TCP/IP Model we combine them and called it as 5 layer model.

***************Deep dive into the layers

Application layer:

it is a layer where users interact. Such as interact via UI of an application to chat etc.

>ping google.com

this command will tell you the ping of your request.

PING: Ping is a complete round trip time of signal from sending to the server and then getting back to the device.

**********************Client server and p2p architechture
There are two type of communication architecture

1) Client-server architechture (Where one server and several clients are sending request) 
3) peer to peer (devices are connected together, users are sending request to each other e.g chat app. there is no dedicated )


*****************Types of devices 
There are several device which are majorly used in computer network:
-----
These 3 are pure hardware devices
1) Cables
2) Repeaters: Repeaters are the devices that are used to regenerate the signals. It do not amplify the signal. When the signal becomes weak, they copy the signal bit by bit and regenerate 	      it. 
3) Hubs: It is a multiport repeater. A hub connects multiple wires coming from different branches. Like start topologies. They do not have intelligence to select the best path
-------
These 3 are hardware and software devices
4) Bridges: Bridges are also repeaters with some additional functionalities such as they have ability to filter content by reading MAC address of source and destination. It is also used to 	    connect two lAN networks working on same protocols. It has single input and single output.
5) Switches: A switch is a multiport bridges with a buffer and designed to boost its efficiency and performance
6) ROuters: Routes the data, assign IP addresses etc. and do much more as covered above.
----------------
Gateway is not a device its simply a term used as an entry point where Firewalls etc are set
7) Gateway: Used to connect two networks together that may work upon different networking models. They basically works as a messenger agents that takes the data from one system, interpret it, and send it to another system.
7) Brouters: They are the combination of Bridge and router. It work either at datalink layer or network layer.
----------------
These 2 used for security puposes
8) IDS (Intrusion detection system)
9) Firewall 
-----------
Modem is moduler/demoduler used to convert analogue signals into digital and vice versa.
10) Modem

**********************Continuing Application layer: Protocols
Web protocols:
HTTP Hyper text tranfer protocol. Deals with how html files will transfer from one place to another.
DHCP Dynamic Host Configuration Protocol. Used to assign IP address to the devices.
FTP File Transfer protocol: used to tranfer files. This protocol is not in used now a days as HTTP do its job too.
SMTP: Simple Mail transfer Protocol Used to send mails
POP3 and IMAP: Used to receive/download mail from the mail server.
SSH: Secure Shell. If you want to login to the terminal of someone else computer you can use SSH
VNC virtual network control: Related to graphical stuff
UDP User datagram protocol: It is a stateless connection or connectionless oriented here the lose of data is not much important e.g video calls.

*******************
Sockets: Its an interface between your process and internet.

Ports: IP address tells which device we are working, ports tells us which application of the device we are working with and Ephemeral ports tells which instance of the application of the 	device we are working with. e.g IP address will tell you about your computer, port number will identify the device let say google chrome and ephemeral port will tell us which 	instance or tab of the google chrome.


***************HTTP in detail
In Client server architecture HTTP tells us how will you send the http request and how will you get back http response from the server. HTTP use TCP/IP inside HTTP as TCP/IP make sure that all the data has sent 100%. HTTP is a stateless protocol. Server will not store any information about the client. 

Remember HTTP is an application layer protocol and TCP/IP is an transport layer protocol.

************HTTP Methods
GET
POST
PUT
DELETE
etc.

***************Status Codes
1XX --> informational code
2XX --> Success
3XX --> Redirect
4XX --> Client Error, Client did something wrong
5XX --> Server Error


*************Cookies 
cookies is a special string which is stored in our browsers.
HTTP is stateless then when we close the browser and open again to the website we are not logged out our session/state remain stored how? The answer is cookie.
whenever you first time visit a website that site set a cookie and when ever next time you will visit that site the browser will sent that cookie in the header along with you. So the website will know that you are not visiting it for the first time it will check your cookie and find your state. Thats why you get the same state whenever you logged in.
Companies can miss use your cookies information like when you visited the site and etc.

3rd party cookies: These are cookies for the sites that you haven't visited. For example you visited a site and that site have some ads so 3rd party cookies will set your cookies for  these ads sites also whcih you havent visited.


**************How email works?
SMTP simple mail transfer protocol is used for sending and receiving the emails. The email is send to the SMTP senders server and that server forward your email to SMTP receiver server and your friend to whom you are sending the mails will download the emails from SMTP receiver server. If both senders and receivers are at same gmail domain such as gmail.com then the email will be sent directly.
SMTP also uses TCP/IP protocol.
> nslookup -type=mx gmail.com


****POP post office protocol

This protocol is used to retrive/download the emails from mail server.
client simply makes a request to POP server it will transact your emails


***********IMAP: Internet Message access protocol

This is also used to retrive emails from the mail server but it allows you to access your emails from multiple devices


****************DNS  Domain name system

This is basically a service which connects our urls to the actual IP addresses of the server.
when we make HTTP request the HTTP protocol ask DNS to give the corressponding IP address for the request URL. It will connect us with that.

There are millions of URLs we cannot remember IP address of each server and neither we cannot have only a single database to store all these URLS so we distribute our database.

mail.google.com

here mail is sub-domain
google is second level domain
.com is top level domain


****************Root DNS servers
.io  .org  .com  .pk

.com for commercial puposes
.org for organizations
.io for tech world
.edu for educational purposes

student.io    internetsociety.org   these are second level domains

who are maintaining these Root servers you can check here:  root-servers.org
who register these domain? : icann.org

******************Understanding what happens when you search for a domain

whenever you visit a website your browser stores the IP address of that website in your local cache/buffer so that you dont have to search for it again and again.

So, Whenever you made a request you browser will check first in your local chache of your computer, if it not found there then it will look into the local server that is your ISP server which will look into Root DNS server if its not there then it will finally call TLD (top level domain server) this would our first time contact. So the TLD server will return the IP address of the searched website in return to the ISP server.

**Remember your ISP will have all the records of the websites you are visiting. 

**NOTE**: You cannot buy a domain name you can only rent it.

you can check DNS by using the following command:

> dig google.com

**************************Diving deep into transport layer

*****************Difference between Network layer and transport layer

let say you sent a message to your friend. Here a message is getting send from one computer to another. 

The tranfer to the data from one system to another is done by Network layer. OK, so whats is Transport layer is for?

Transport layer lies in the devices and so the role of transport layer is to take the from the network and deliver to the right application.

In short the transformation from one device to another is done by network layer but the transformation of data within the device is done by transport layer. Thats why we say Transport layer provides abstraction.

you send a gift via TCS courrier from lahore to ISB

here the travel of gift within lahore from you to TCS is done by transport layer.
And then the travel of gift from lahore to isb TCS office is done by network layer.

now Isb TCS will send this gift to your friend this is also done by transport layer.


Transport layer have some protocols such as TCP/IP and UDP.

*****************Diving deep in TCP/IP
So till now we all know basics of TCP/IP

let say you are doing video call, sending text message and voice message at the same time. how this data bundle will be reached to the right application in the right device?

here comes the multiplexer and de-multiplexer.
Multiplexer transfers the bunch of data via a single medium. De-multiplexer is opposite of multiplexer and resides are receiver side.

********How multiplexer works?
Multiplexer have sockets and Your application sends data to the sockets of multplexer. Here each socket have port number and we all know port numbers are used to identify the each device. Data travels in the form of packets and each data packet have socket port number to identify the device and sequence number to reassemble the data. These packets reaches the de-multiplexer via this they reach their resired application.

Multiplexers also do congestion (traffic) control. It will slow down the data transfer if a bunch of data is going via a same medium and so on.

Since they are in transport layer there for they tranfer data on TCP/IP and UDP protocols and therefore they work on some algorithms such as congestion control algorithm.


********Checksums

you are sending data packets to your friend and some packets get losts. How would you know?
This is verify by checksum.

checksum is simply a number which is calculated by an algorithm. Once all the data packets have been reached to your friend he will calculate the check sum and will compare it with your checksum. If they are same then everything is ok. if not then something went wrong.

*********timers

these timers tells that whether the data you sent reached the receiver or not.

if a packet get lost it will never reach to your friend so the timer will be expired. 

*********************Sequence number
This number is used to re-assemble the data and to avoid duplicate data packets

let say you send a data to a your friend and your friend didnt received a data packet then you send that data packet again. Here you will have 2 data packets. So this problem will be solved by sequence number.

*****************UDP Protocol
The data may be lost
The data might be changed
Data may not be in order

it is connectionless means it will not tell whether the data has received or not.
UDP uses checksums (a number to check the corruption of data). But it do not take any action in case of any data corruption/missing.

***************UDP packet
it contains:
1) source port number
2) destination port number
3) length of datagram/packet
4) checksum

5) data

first 4 points are called headers, as these are attached with your data packet.

**Use Cases of UDP:
its very fast
used by video conferencing apps
DNS also uses UDP

> sudo tcpdump -c 5

this command is used to check the 


************How TCP/IP works
It is a transport layer protocol. 
Application layer sends the a lot of raw data and TCP/IP segments this data. Divide in chunks--> add headers. It also may collect data from network layer where it will divided into more smaller segments and then send to the user where it get re-assembled.

**It take care of two things:
- when data does not arrive (responsible for 100% data transmission)
- maintains the order of data

Features:
- Connection oriented (100% data transmission, will let you know if any data packet get missed.
- Error control
- congestion (traffic) control
- Full duplex (both way file sending from user to receiver simultaneously)

**NOTE: TCP/IP is only established only between two computers. Its not like one computer is sending messages to 10 computers. In such case each will have its separate TCP/IP protocol.

***************How TCP/IP establishs connection: Three way hand shake
As we know TCP/IP protocol first makes connection and then transport data. It is called 3 way hand shake. In 3 way hand shake a client sends a synchronization flag along with a random sequence number to the server. And then server will acknowledge it and send back a new synchronization flag along with the a new sequence number (generated by doing some maths on the sequence number which he got from the client) along with a new acknlowledgement number. Once client has received the response, it will send back a connection.

*********************Network layer:
Transport layer--> segments
Network layer--> Packets
Data linke layer --> Frames

This a layer where routers lives in. Here data travels from one computer to another computer. 

when globally a data travels then there could be several routers in between them.

When a data reaches a router it checks the routing table and checks that whether this data was for me or not. A data packet contains the network layer address of sending and receiving destination. If the data that reaches the router 1 is not it. then it will forward it to the next router by looking the forward table. (forward table lies inside the routing table and routing  table lies inside the router) And now this next router will do the same until unless it reaches the right destination. 

It is called hope by hope data transfer or hoping.
so you mean to say that the router in my house is also contirbuting in hoping? Like my router is also helping in routing the data from one place to another? No, actually the routing or you can say hoping happens at ISP router level. Therefore in IP address for routing we use subnet address. which is:

**And ip address: 192.168.2.30
here  192.168.2 this is network address. it is also called subnet address/id. 
and 30 is device address. it is also called host id.

Every router has its own network layer address.

********************Control plane
who is making the above mentioned routing and forwarding tables. Where are they came from.
You can imagine an internet as a huge graph and routers as nodes on it.

There are two types of routing
1) Static Routing (manually): In static routing You have to add addresses manually in the routing table tell the route that you wanna go from here to here. When ever a new router is added 			      in the path you have to configure it too.
2) Dynamic Routing: You dont have to add manually. It will adapt/choose the best path dynamically by using algorithms such as Dijkstra's algorithm (an algo to find the shortest path in 		    weighted graph)

****************IP addresses
It is a networking layer protocol.

IPv4: It is a 32 bits size of IP address having 4 groups each of 8 bits. e.g 172.28.192.1. Means we can create 2^32 = 4.3Billion IP address. At early age of internet we thought it will enough but that was not so we created IPv5

IPv6: 128 bit size of IP address. 2^128 = 3.4x10^38 Billion IP addresses we can create. e.g It has 8 groups each of 16 bits and are separated by colons: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

Cons of IPv6: 
- It is not backward compatible. Like wesbites configured on IPv4 cannot be configured with the servers configured with IPv6.
- A lot of effort is required to shift to IPv6 as ISPs would have to shift. A lot of hardware work would be required. This is the reason the whole world has not shifted to IPv6 yet.

*********Classes of IP address
TCP/IP defines five classes of IP addresses: class A, B, C, D, and E. Each class has a range of valid IP addresses. The value of the first octet determines the class. IP addresses from the first three classes (A, B and C) can be used for host addresses. The other two classes are used for other purposes – class D for multicast and class E for experimental purposes.

A - first octet value: 0-127 , rest 3 octet are range from 0-255, subnet mask: 8 e.g 10.50.120.7 
B - first octet value: 128-191 rest 3 octet are range from 0-255, subnet mask: 16 e.g 172.16.55.13
C - first octet value: 192-223 rest 3 octet are range from 0-255, subnet mask: 23
D - first octet value: 224-239 rest 3 octet are range from 0-255, subnet mask: -
E - first octet value: 240-255 rest 3 octet are range from 0-255, subnet mask: -	

*****************reserved IP addresses
localhost: 127.0.0.1
loop back addresses: these address allows you to contact the same process. like you local host is your client and server as well.

***********Packets
In network layer we have packets and each packet is of 20 bytes. It contains so many information such as IP versions, checksums, length of the packet, identification, flags, 	protocols, addresses, TTL (time to live: TTL is a number which defines the number of hoping. e.g TTL=60 means that after 60 hopings (forwarding from server to server) if the packet has not reach to the destination it will be lost.) etc. 

******************Middle Boxes
These are the devices which are in between you computer and routers. They also deals with the data packets. such as your firewall lies inside the middle box. It decides which packet to pas and which to reject. It filters out IP packets on various rules such as on the basis of their:
Addresses
It modifys the packet
port numbers
flags
protocols

There are two types of firewalls:
Stateless vs Statefull firewalls.
stateless fire walls do not store any state whereas statefull wire wall do in the cache. Therefore they are more efficient.

*************NAT (network access translation

Its basically a method to map the IP addresses space into another by modifying their IP addresses.
let say your host/PC has the address of 10.0.0.1 and desitantion address is 200.100.10.1

NAT lies in the router and will modify the your IP address that is 10.0.0.1 and will represent it as let say 150.150.0.1. Now sourse address is 150.150.0.1 and desitnatino address is 200.200.10.1

coming from server to your PC the order will be reverse now the destination address will be modified and that will again your PC/Host address.

In both cases your Host address will be modified. 

***************Data Link Layer

Here data has reached to the right device. This layer receives data packet from network layer containing IP addresses of both sender and receiver and subnet mask. Here 		   mac addresses are assign to senders and receivers data packet this is called physical addressing. Physical addressing is done in this layer so that each packet reaches 		   the right application in the device. Mac address is a 12 digit alphanumeric number. It is assigned to every network controller of your device. the bluetooth of your 		   device can have different mac address and wifi router can have different.
It worked at your router level and deals with mac addresses. Its a place after that data will convert into electrical signals and will travel to the devices which is done in physical layer.

When ever a new device is connected with the router. It sends request to DHCP server. And DHCP server will assign it a new IP address. 
There is a thing called DLLA Data link layer address.

Let say 5 PCs are connected in a LAN
pc1 wants to send a data to pc5

it will check the IP address of pc5 in its cache first. If it will not be there then it will look in the cache of other PCs connected with it by using ARP (Address resolution protocol). As we know in Data link we deal with frames and each frame contains the DLLA of sender and IP address of destination. It will ask that this is the IP address of destination can you please give me its DLLA? It will get the DLLA it will sned that data frame to PC5. 


**NOTE:** DLLA are nothing  but mac address of your devices. In Data link layer physical address is done which is assigning Mac address to the frames so that they reach the right device. and remember mac address is not of your computer its of components of your computer your bluetooth and wifi can have different mac addresses. Mac stands for media access control. It is unique identifier for you device.


---------------------------------------------
# IP, Subnet, Private Subnet, Public Subnet:
Since we all know IP are the unique identifier. Used to distinguish between devices/resources in a network.

## Why do we need of Subnet:
Let say you have an office and you have a single network. When different employees are gonna attach with the same network. So if anyone of the employee is exposed to a malicious website then Hacker will have access to his device. Since that person and whole office is connceted wuth the same network. So your whole network and data can be breached all devices can be access. Just to avoid such security threat. we use Subnet. We divide our network into subnetworks.

Let say we have department that contains sensitive information. So we will keep that department in a separate subnet and rest in the other subnet. In this way, we can separate our sensitive information. And in other subnets if there is a security breach then no issue. On the devices in that particular subnet are gonna compromised not all.

### Private Subnet
The subnet that is only accessible within the network.

Generally, IP addresses start with 192, 172 or 10 are private IP addresses
### Public Private Subnet:
The subnet that is exposed to internet.

# CIDR (Class Inter Domain Routing):
CIDR is used to calculate the size of the network by the number of IP address that a particular range of CIDR can provide.
So, This means If I want to know the size of my network or virtual network I can calculate it by its number of IP addresses.

Since we all know an IP address looks like this: 192.168.2.1
we represent them in decimal but in actual they are in octat such as 11111111.00000000.00000000.00000000 = 255.0.0.0

# How to calculate CIDR:
since there are 4 digits and each digit is of 8 bit. So 4*8=32
so let say you want only 2 IP address in a subnet then you are gonna do this:
192.167.9.0/31

here 32-31=1
No. of IP addresses = 2^1 = 2

here 192.167.9 are gonna remain constant only last 0 is gonna vary.

**NOTE: If no. of IP addresses required are greater than 256 then we are going to vary more than one digit otherwise only the last digit of the IP will vary, and the rest will remain the same.**

so smaller the number after /,  greater the number of IP addresses will be.

Example:
192.167.9.0/16

so, 
32-16=16
No. of IP addresses = 2^16 = 65536
