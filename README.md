# `bpftrace` Scripts

## ovpn_sendto.bt
Simple script to attach to OpenVPN process, trace `sendto(2)` system call, parse and print IP address. Created to snoop ExpressVPN server IPs for manually updating `iptables(8)`. 
