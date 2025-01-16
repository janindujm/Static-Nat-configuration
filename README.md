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

# Static NAT Configuration in Cisco Packet Tracer

This repository contains a Packet Tracer lab file demonstrating the configuration of Static NAT (Network Address Translation) on a Cisco router.

## **Overview**
The lab focuses on setting up Static NAT to enable devices on a private network to be accessible from an external network using a consistent public IP address. This is a common scenario for hosting servers, such as web servers or mail servers, behind a NAT-enabled router.

## **Lab Details**
- **Inside Local IP Address**: 192.168.1.100
- **Inside Global IP Address**: 203.0.113.10
- **Router Interfaces**:
  - `GigabitEthernet0/0` (Inside)
  - `GigabitEthernet0/1` (Outside)

### **Key Configuration Steps**
1. Define inside and outside interfaces on the router.
2. Configure the static NAT mapping for the private-to-public IP address translation.
3. Verify the NAT translation table using the `show ip nat translations` command.

## **Used Commands**
Below are the commands used in the lab for configuring Static NAT:

**Router 1**
1. **Enter Global Configuration Mode**:
   ```plaintext
   configure terminal
   ```

2. **Define Inside and Outside Interfaces**:
   ```plaintext
   interface fa1/0
   ip nat inside
   exit

   interface fa0/0
   ip nat outside
   exit
   ```

3. **Set up Static NAT Mapping**:
   ```plaintext
   ip nat inside source static 10.0.1.10 203.0.113.4
   ```

4. **Verify NAT Configuration**:
   ```plaintext
   show ip nat translations
   show ip nat statistics
   ```
![image](https://github.com/user-attachments/assets/5c2157ca-f48c-4314-b5f5-9dd5e41a0e13)
  ![image](https://github.com/user-attachments/assets/a34738ca-4616-46e6-8de2-9f5cbeb8463f)

   

5. **Save the Configuration**:
   ```plaintext
   copy running-config startup-config
   ```

## **How to Use**
1. Open the `.pkt` file using Cisco Packet Tracer.
2. Review the topology and examine the router's configuration.
3. Test connectivity by simulating traffic between the private and public networks.

## **Skills Demonstrated**
- Configuring and verifying Static NAT.
- Understanding NAT translation tables and their role in network address mapping.
- Practical use of Cisco IOS commands.

## **Screenshots**

  ![image](https://github.com/user-attachments/assets/f5b27e68-fab0-43d5-b27c-469f0afff292)


---


