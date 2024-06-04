# `bpftrace` Scripts

## ovpn_sendto.bt
Simple script to attach to OpenVPN process, trace `sendto(2)` system call, parse and print IP address. Created to snoop ExpressVPN server IPs for manually updating `iptables(8)`. 

<details>
  <summary>Ex.</summary>
  
  `$ expressvpn connect usla1`
  
  ```sh
  
    # bpftrace ./ovpn_sendto.bt
    Attaching 3 probes...
    Tracing openvpn sendto(2). Ctrl-C to end.
    openvpn -> 45.38.57.61
    openvpn -> 45.38.57.139
    openvpn -> 45.38.57.61
    ^C  
  ```

</details>
