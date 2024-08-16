<p align="center">
<https://github.com/user-attachments/assets/345d15b1-91bf-434f-8653-514deecf4d40)](https://i.ytimg.com/vi/M66J7oRU400/maxresdefault.jpg>

</p>
<p align = "center">
<h1>Cisco Packet Tracer - Connecting Devices</h1>
</p>
<br />

<p align = "center">
<img src = "https://github.com/user-attachments/assets/d0756242-dc93-4961-b67d-266fd22489a4">

</p>

<h2>Introduction</h2>

- Objective: Demonstrate the ability to connect various network devices (PCs, servers, switches, and routers) using appropriate cabling techniques.

- Tools Used: Cisco Packet Tracer

- Skills Highlighted: Network configuration, understanding of cabling types, practical application of networking concepts.


<h2>Lab Setup: </h2>

- Network devices: PCs, servers, switches, and routers.

- Cable types: Copper straight-through, copper cross-over, and fiber-optic cables.</b> (21H2)

<h2> Additional Parameters </h2>

- Auto MDI-X will not be enabled on any devices used in this excercise.

<h2>Step-by-step Implementation</h2>


![image](https://github.com/user-attachments/assets/2e86cf37-2104-4d55-b675-473777a8e7ee)





<p>
In this simple excercise we will be using Cisco Packet Tracer to demonstrate how to connect the nodes on a network using the proper cables. As stated above, our primary objective will be to connect all of the nodes on each network, and then connect the two networks.
</p>
<br />

![image](https://github.com/user-attachments/assets/c80b5638-f554-4e07-b548-2369f7061bc5)



<
Our first step will be connecting all of our end hosts to the switches on our networks. We're going to want to use straight-through cables to do so, as our hosts transmit data on ethernet pins 1 and 2 whereas our switches recieve data on those pins. 
<br />

![image](https://github.com/user-attachments/assets/572bcfef-10b8-4fca-bfbf-8a360af91508)




<p>
Next, we'll be using crossover cables to connect our switches to each other. Switches transmit data using pins 3 and 6 and receive it using pins 1 and 2, so if we were to use straight-through cables the switches would receive data on the pins they use to send it and therefore be unable to communicate. We'll also want to make sure that each switch is connected to at least two other switches to minimize the number of single points of failure we have on our network.
</p>
<br />

![image](https://github.com/user-attachments/assets/78b2f233-eb26-4b65-b797-f8723ea2c3c0)

<p>
Now that we have connected our switches to each other, we will conncect our routers to said switches using straight-through cables since routers and switches transmit and recieve data using different pins, and don't need the help of crossover cables to communicate. Similarly to our switches, we'll want to make sure we have redundant connections to our routers so that there are as few single points of failure as possible.
</p>
<br />

![image](https://github.com/user-attachments/assets/9fd01f27-95b1-4191-ac6a-74b7c8f89dc0)

<p> Next we will connect router 1 to router 2 using a crossover cable. The distance between these two routers is 50 meters, so a standard utp cable is still a suitable choice for facilitating their connection</p>
<br />

![image](https://github.com/user-attachments/assets/3a597ebc-cd9c-417a-a228-46423b29141a)

<p>The penultimate connection of our excercise will be between routers 2 and 3. This time the distance between them is 3 kilometers, which is too great a distance for even a multimode fiber optic cable, so we will facilitate this connection with a single mode fiber optic cable. </p>
<br />

![image](https://github.com/user-attachments/assets/c4507b1e-d150-4d7b-a58c-9226d873541e)

<p> Now that we have connected all other nodes on our networks, we will conclude our excercise by connecting routers 3 and 4. The distance between them is 250 meters, which is too great a distance to connect them with a UTP cable, but within the range of multimode fiber optics. Depending on the resources of the company it may either be more appropriate to use either single-mode fiber optics to maximize the the connection speed of the connection, or multimode fiber optics to minimize the cost of installation. </p>
<br />

<h2> Conclusion </h2>

<p>In this lab, we demonstrated the practical application of connecting various network devices using Cisco Packet Tracer. We covered the essential techniques for cabling and configuring PCs, servers, switches, and routers, emphasizing the correct use of copper straight-through, copper crossover, and fiber-optic cables.</p>

<h3>Key Takeaways</h3>

<h4>End Hosts to Switches:</h4>
-We used straight-through cables to connect PCs and servers to switches. This is because end hosts transmit data on Ethernet pins 1 and 2, while switches receive data on these pins, ensuring proper communication.

<h4>Switch to Switch Connections:</h4>

-Crossover cables were utilized to connect switches to each other. Switches transmit data on pins 3 and 6 and receive on pins 1 and 2, requiring crossover cables to align the transmit and receive pins correctly. Redundant connections between switches were established to reduce single points of failure.

<h4>Switch to Router Connections:</h4>

-Straight-through cables were used to connect switches to routers. Routers and switches transmit and receive data on different pins, so straight-through cables suffice. Redundant connections to routers were also established to enhance network resilience.

<h4>Router to Router Connections:</h4>

-For short distances (e.g., 50 meters), we used crossover cables to connect routers. For longer distances, such as 3 kilometers, single-mode fiber-optic cables were used due to their extended range capabilities. For a 250-meter connection, multimode fiber-optic cables were appropriate, considering the distance and potential cost-effectiveness.
<br />
<br />
<br />

<p>By following these cabling and configuration practices, we ensured robust and efficient communication within the network, minimizing the risk of failures and optimizing performance. This exercise highlights the importance of selecting the right cabling type based on the devices and distances involved, a crucial skill for any network engineer. Thank you for reviewing this lab. For further details or questions, please refer to the provided diagrams and steps.</p>
