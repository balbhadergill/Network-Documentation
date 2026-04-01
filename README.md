# Home Network Documentation

**Student:** Balbhader Singh Gill  
**Course:** Networking  
**Submission Date:** April 1st, 2026  

---

# 1. Overview
This document describes my home network including physical and logical topology, addressing scheme, devices, configurations, and security practices used to protect login credentials.

The home network is used for internet access, streaming, studying, and monitoring a security camera installed in the garden.

---

# 2. Physical Topology

```
                     Internet
                         │
                     ISP Modem
                         │
                     Home Router
                  (192.168.1.1)
            ┌───────────┼───────────┐
            │           │           │
        Desktop       Laptop      Smart TV
        (Ethernet)     (WiFi)       (WiFi)

                          │
                     WiFi Network
            ┌───────────┼───────────┐
            │           │           │
         Phone        Tablet     Security Camera
                                      (Garden)
```

This diagram shows how devices are physically connected to the router through Ethernet and WiFi.

---

# 3. Logical Topology

Network Range: **192.168.1.0/24**

```
Router (Gateway)
192.168.1.1

Devices in Network
192.168.1.10   Desktop
192.168.1.12   Laptop
192.168.1.11   Smartphone
192.168.1.15   Smart TV
192.168.1.18   Tablet
192.168.1.13   Security Camera
```

All devices communicate through the router which manages DHCP, internet access, and firewall protection.

---

# 4. Addressing Documentation

| Device | IP Address | Connection Type | Description |
|--------|------------|----------------|-------------|
| Router | 192.168.1.1 | Wired | Default Gateway |
| Desktop | 192.168.1.10 | Ethernet | Main workstation |
| Laptop | 192.168.1.12 | WiFi | Study device |
| Phone | 192.168.1.11 | WiFi | Personal smartphone |
| Smart TV | 192.168.1.15 | WiFi | Streaming device |
| Tablet | 192.168.1.18 | WiFi | Household use |
| Security Camera | 192.168.1.13 | WiFi | Garden monitoring |

Subnet Mask
```
255.255.255.0
```

DNS Servers
```
8.8.8.8
8.8.4.4
```

---

# 5. Network Devices and Services

## Router
Functions:
- DHCP Server
- NAT (Network Address Translation)
- Firewall
- Wireless Access Point

## ISP Modem
Provides internet connectivity from the Internet Service Provider.

## Security Camera
Used to monitor the garden area and ensure home security.

## Network Services
- DHCP
- NAT
- Wireless Network (WPA2/WPA3)
- Internet Access

---

# 6. Device Configurations

## Router Configuration
```
SSID: Bell-5G
Wireless Security: WPA2/WPA3 Personal
DHCP Range: 192.168.1.10 - 192.168.1.100
Firewall: Enabled
Admin Access: Password Protected
```

## Desktop Configuration
```
Connection Type: Ethernet
IP Assignment: DHCP
Operating System: Windows 11
```

## Laptop Configuration
```
Connection Type: WiFi
IP Assignment: DHCP
```

## Security Camera Configuration
```
Connection: WiFi
Location: Garden
Remote Monitoring: Mobile App Enabled
```

---

# 7. Credential Security Method

Login credentials are stored securely using a password manager.

Security methods used:
- Password Manager (Bitwarden / Google Password Manager)
- Strong unique passwords
- Two-Factor Authentication (2FA)
- Encrypted password storage
- Default router password changed

Passwords are not stored in plain text.

---

# 8. Network Security Measures

The following security practices are implemented in the network:

- WPA3 Wireless Encryption
- Router Firewall Enabled
- Firmware Updates Installed
- Secure Router Login Credentials
- Regular Network Monitoring

---

# 9. Testing and Verification

Commands used to verify network connectivity.

Check IP configuration
```
ipconfig
```

Test connection to router
```
ping 192.168.1.1
```

Test internet connection
```
ping google.com
```

Display routing table
```
route print
```

Check active network connections
```
netstat
```

---

# 10. GitHub Repository

This documentation is stored in my GitHub repository.

Example repository link:
```
https://github.com/yourusername/home-network-documentation
```

---

# 11. Conclusion

This document provides a complete overview of my home network including topology, addressing scheme, devices, and security measures used to protect the network.
