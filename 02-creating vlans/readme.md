problem-
in an office we have to setup an internal network having different departments-
devs , sales and server
but they should be able to communicate 

so we used a layer 3 router as they can be used to set up routing route

then created vlans 10 (devs) , 20( sales) and 30 ( server)
assigned the respective ports to them.

vlan 10 uses default gateway 192.168.10.1 via fa0/1
vlan 20 uses default gateway 192.168.20.1 via fa0/3
vlan 30 uses default gateway 192.168.30.1 via fa0/2

till now seprating the departments was done then we 
commanded the switch - ip routing , to make communication between vlans possible.

question which arise-
1) why divide them into vlan when we route them later?
    as if one system in lets say sales department get compromised its not easy for malicious virus 
      or an attacker to move from one vlan to another , they have to passthrough a firewall
      so they can be spotted.

