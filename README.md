# Wendy


This is a fork of secondbit/wendy, that is design to work with go1.13+, and be usable by libp2p hosts.


# Hooking Into IPFS/LibP2P

Using the `DATA_SEND` message purpose, whenever a message is received we deliver it locally. This can be used to hook into an IPFS application registered via a wendy app callback to deal with dht requests, etc..

We should have a special case where for certain message purposes, we randomly forward between peers in our local cluster.