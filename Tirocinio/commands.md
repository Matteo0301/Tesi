## Before setup

```
ip route
```

> default via 192.168.66.1 dev wlo1 proto dhcp src 192.168.66.100 metric 20600 
172.17.0.0/16 dev docker0 proto kernel scope link src 172.17.0.1 linkdown 
172.20.0.0/16 dev br-0182ce3e33cf proto kernel scope link src 172.20.0.1 linkdown 
172.21.0.0/16 dev br-dc43ea6c7713 proto kernel scope link src 172.21.0.1 linkdown 
172.22.0.0/16 dev br-009d39e73a05 proto kernel scope link src 172.22.0.1 linkdown 
172.23.0.0/16 dev br-ecdbea27f35a proto kernel scope link src 172.23.0.1 linkdown 
172.24.0.0/16 dev br-255aff90d75f proto kernel scope link src 172.24.0.1 linkdown 
192.168.66.0/24 dev wlo1 proto kernel scope link src 192.168.66.100 metric 600 
192.168.123.0/24 dev br-4b9456140280 proto kernel scope link src 192.168.123.1 linkdown

```
sudo ./scan -futav -m S -o $FILENAME -i $IP
```

## After setup

```
sudo nmap -sn 192.168.200.223/24
```