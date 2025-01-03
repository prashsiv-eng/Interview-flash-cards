### Border Gateway Protocol (BGP)
* Autonomous Systems (AS)
    - An Autonomous System is a collection of IP networks and routers under the control of a single organization that presents a common routing policy to the internet.
    - Internet Service Providers (ISPs) can be considered AS.
* Types of BGP
    - External BGP (eBGP)
        - Used for communication between different Autonomous Systems.
        - Typically used by ISPs to exchange routing information with other ISPs.
    - Internal BGP (iBGP)
        - Used for communication within the same Autonomous System.
        - Helps in maintaining a consistent routing policy within an AS.
* BGP Attributes
    - Path Vector Protocol: BGP uses path vectors to ensure loop-free routing.
    - Attributes such as AS-Path, Next-Hop, and Local Preference are used to determine the best path.
* BGP Operations
    - BGP routers establish a TCP connection with each other to exchange routing information.
    - BGP uses incremental updates to reduce the amount of data sent over the network.
    - BGP supports policies for route selection and advertisement.