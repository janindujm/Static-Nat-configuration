# Static NAT Configuration in Cisco Packet Tracer

This repository contains a Packet Tracer lab file demonstrating the configuration of Static NAT (Network Address Translation) on a Cisco router.

## **Overview**
The lab focuses on setting up Static NAT to enable devices on a private network to be accessible from an external network using a consistent public IP address. This is a common scenario for hosting servers, such as web servers or mail servers, behind a NAT-enabled router.

## **Lab Details**
- **Inside Local IP Address**: 10.0.2.11
- **Inside Global IP Address**: 203.0.113.4
- **Router Interfaces**:
  - `FastEthernet0/0` (Outside)
  - `FastEthernet0/1` (Inside)

### **Key Configuration Steps**
1. Define inside and outside interfaces on the router.
2. Configure the static NAT mapping for the private-to-public IP address translation.
3. Verify the NAT translation table using the `show ip nat translations` command.

## **File Details**
- `29-1 NAT Configuration.pkt`: The Packet Tracer lab file containing the network topology and configuration.

## **How to Use**
1. Open the `.pkt` file using Cisco Packet Tracer.
2. Review the topology and examine the router's configuration.
3. Test connectivity by simulating traffic between the private and public networks.

## **Skills Demonstrated**
- Configuring and verifying Static NAT.
- Understanding NAT translation tables and their role in network address mapping.
- Practical use of Cisco IOS commands.

## **Screenshots**
(https://github.com/user-attachments/assets/ddb8416d-f64f-4d61-97f7-1d16fe08e9e9)


---


