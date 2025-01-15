# Konfigurasi External Proxy dengan MikroTik
```sh
/ip firewall nat
add action=dst-nat chain=dstnat dst-port=80 in-interface=ether5-server \
    protocol=tcp to-addresses=10.0.0.254 to-ports=3128
```