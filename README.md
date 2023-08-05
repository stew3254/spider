# Spider (Placeholder)
A mesh network written in Go using Wireguard

## Goals
 * A peer to peer network where no server is necessarily needed (though one could be configured as such)
 * To make it easy to set up
 * It allows clients to punch through a NAT
 * To have confidentiality and integrity in its communication using OTP and public key cryptography
 * To have a self hosted server for facilitating the communication between any number of peers
   * Ideally give as little power to the self hosted instance as possible, but to provide a public means for two users to find each other and communicate if they can't directly.
   * Allow users nearly full control over what they advertise to who, while keeping everything accurate and not allowing spoofing.
 * To allow users to register their identity via a token, and said identity is tied with public key cryptography
 * To allow users to create networks and specify subnets. Then, can invite other users securely into their networks.
   * Via sending a direct invitation to their user
   * By sharing a time based code (could be one time or multiple use) which allows people to join
   * To advertise directly via the identity host for anyone to be able to join.
 * The network owner is the admin and can approve others as admin as well. Admin allows you to kick people out of the network
 * To automatically assign an IP and require user to set a hostname on entry to network so others can reach you via either method
 * To be flexible in setting up networks. Allow users to advertise which ports will be open to which users or the whole network and to advertise routes.
 * If a router is available, allow users to securely route full tunnel through an available router on their network
 * VPN will manage firewall rules on the machine so users do not have to. However, allow a manual mode for users to be able to specify their own routes and rules
 * Give user easy option to run DNS server for other users on the network.
 * A nice CLI gui to show others what is available to them. Would be nice to see who is online and to neatly list everything available
 * Eventually Windows Support
 * Eventually GUI support
