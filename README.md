# Jarkom-Modul-4-C04-2021

Kelompok : C4

Anggota Kelompok :

- Muhammad Arif Faizin (05111940000060)
- Aufi Fillah (05111940000148)
- Abiya Sabitta Ragadani (05111940000166)

## Soal

![Topologi](img/soal.png)


## Variable Length Subnet Masking (VLSM) - CPT



## Classless Inter Domain Routing (CIDR) - GNS3

| Subnet | Host                 | Jumlah IP   | Netmask |
|--------|----------------------|-------------|---------|
| A1     | ELENA                | 720         | /22     |
| A2     | ENIESLOBBY           | 250         | /24     |
| A3     | SEASTONE + OIMO      | 2           | /30     |
| A4     | MAINGATE             | 500         | /23     |
| A5     | JORGE                | 12          | /28     |
| A6     | JABRA                | 520         | /22     |
| A7     | GUANHAO + FOOSHA     | 2           | /30     |
| A8     | BLUENO               | 1000        | /22     |
| A9     | CALMBELT + COURTYARD | 1000 + 1020 | /21     |
| A10    | JIPANGU              | 100         | /25     |
| A11    | PUCCI + WATER7       | 2           | /30     |
| A12    | CIPHER               | 700         | /22     |
| A13    | WATER7 + FOOSHA      | 2           | /30     |

![CIDR GNS3 Project](img/cidr_soal.png)

### ELENA
```
auto eth0
iface eth0 inet static
address 10.16.0.0
netmask 255.255.252.0
gateway 10.16.0.1
```

### SEASTONE
```
auto eth0
iface eth0 inet static
address 10.16.4.0
netmask 255.255.255.0
gateway 10.16.4.1

auto eth1
iface eth1 inet static
address 10.16.0.1
netmask 255.255.252.0
```

### ENIESLOBBY
```
auto eth0
iface eth0 inet static
address 10.16.4.0
netmask 255.255.255.0
gateway 10.16.4.1
```

### OIMO
```
auto eth0
iface eth0 inet static
address 10.16.8.0
netmask 255.255.255.252
gateway 10.16.8.1

auto eth1
iface eth1 inet static
address 10.16.4.0
netmask 255.255.255.0
```

### JABRA
```
auto eth0
iface eth0 inet static
address 192.168.20.2
netmask 255.255.252.0
gateway 192.168.20.1
```

### JORGE
```
auto eth0
iface eth0 inet static
address 10.16.18.0
netmask 255.255.255.240
gateway 10.16.18.1
```

### ALABASTA
```
auto eth0
iface eth0 inet static
address 10.16.16.0
netmask 255.255.254.0
gateway 10.16.16.1

auto eth1
iface eth1 inet static
address 10.16.18.1
netmask 255.255.255.240
```

### MAINGATE
```
auto eth0
iface eth0 inet static
address 10.16.16.0
netmask 255.255.254.0
gateway 10.16.16.1
```

### GUANHAO
```
auto eth0
iface eth0 inet static
address 10.16.32.0
netmask 255.255.255.252
gateway 10.16.32.1

auto eth1
iface eth1 inet static
address 10.16.20.0
netmask 255.255.252.0

auto eth2
iface eth2 inet static
address 10.16.8.0
netmask 255.255.255.252

auto eth3
iface eth3 inet static
address 10.16.16.0
netmask 255.255.254.0
```

### JIPANGU 
```
auto eth0
iface eth0 inet static
address 10.16.136.0
netmask 255.255.255.128
gateway 10.16.136.1
```

### CALMBELT 
```
auto eth0
iface eth0 inet static
address 10.16.128.0
netmask 255.255.248.0
gateway 10.16.128.1
```

### COURTYARD
```
auto eth0
iface eth0 inet static
address 10.16.128.0
netmask 255.255.248.0
gateway 10.16.128.1
```

### PUCCI
```
auto eth0
iface eth0 inet static
address 10.16.144.0
netmask 255.255.255.252
gateway 10.16.144.1

auto eth1
iface eth1 inet static
address 10.16.136.0
netmask 255.255.255.128

auto eth2
iface eth2 inet static
address 10.16.128.0
netmask 255.255.248.0
```

### CIPHER
```
auto eth0
iface eth0 inet static
address 10.16.160.0
netmask 255.255.252.0
gateway 10.16.160.1
```

### WATER7
```
auto eth0
iface eth0 inet static
address 10.16.192.0
netmask 255.255.255.252
gateway 10.16.192.1

auto eth1
iface eth1 inet static
address 10.16.160.0
netmask 255.255.252.0

auto eth2
iface eth2 inet static
address 10.16.144.0
netmask 255.255.255.252
```

### BLUENO
```
auto eth0
iface eth0 inet static
address 10.16.64.0
netmask 255.255.252.0
gateway 10.16.64.1
```

### FOOSHA
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
address 10.16.64.0
netmask 255.255.252.0

auto eth2
iface eth2 inet static
address 10.16.192.0
netmask 255.255.255.252

auto eth3
iface eth3 inet static
address 10.16.32.0
netmask 255.255.255.252
```

![CIDR Tree](img/cidr_tree.png)
