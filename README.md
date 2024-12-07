# Integrated Security Solutions Lab (ISSL)

## Objective
The **Integrated Security Solutions Lab (ISSL)** project focuses on creating a robust, multi-layered security environment that integrates key cybersecurity principles, including **Application Security**, **Identity and Access Management (IAM)**, **Data Security**, and **Security Operations**. This project involves connecting **pfSense** instances, leveraging **IPsec VPN** for secure communication between environments, and protecting sensitive data and services with firewalls, web application firewalls (WAFs), and advanced endpoint monitoring. It also integrates **Windows Server** for IAM services and user authentication, providing a comprehensive view of secure network design and operational response.

### Skills Learned
- **Network Segmentation** and **Firewall Management** using **pfSense** (in VMware ESXi and GNS3 environments) for security boundaries.
- Establishing **IPsec VPN** tunnels between different security zones for secure communication.
- Implementing **WAFs** (e.g., **NAXSI** on **OPNsense**) to protect web servers from application-level attacks.
- Configuring and managing **Windows Server** for **Identity and Access Management (IAM)** and **user authentication** in a secure environment.
- Managing **DMZ** environments, including the hosting of public-facing web servers with added security layers.
- Integrating **SIEM** solutions (ELK Stack) for real-time log analysis and security monitoring across all zones.
- Advanced **Endpoint Detection and Response (EDR)** using **Elastic Security** for endpoint monitoring, real-time threat detection, and response.
- Secure web traffic analysis and **VPN** deployment for encrypted communication between virtual and physical network environments.

### Tools Used
- **pfSense** (Firewall, VPN, network segmentation, and IDS/IPS)
- **OPNsense** with **NAXSI WAF** (Web Application Firewall to protect web servers)
- **Windows Server** (Identity and Access Management, user authentication)
- **IPsec VPN** (for secure communication between pfSense instances)
- **Elastic Security** (part of the **Elastic Stack** for **SIEM**, **EDR**, and **threat detection**)
- **Velociraptor** (Endpoint Detection and Response for real-time monitoring)
- **Wireshark** (Network traffic analysis and troubleshooting)
- **Nginx** (Web server for hosting within the DMZ)
- **Kali Linux** (Penetration testing and security assessment)

## Steps

1. **Network Setup and Segmentation**
   - Created isolated security zones using **pfSense** in VMware ESXi and GNS3.
   - Configured **IPsec VPN** tunnels between pfSense instances for secure communication.
   - Segmented the network into **DMZ**, **LAN**, and **WLAN** zones.

2. **Identity and Access Management (IAM)**
   - Integrated **Windows Server** for user authentication and **Active Directory** management.
   - Configured user roles and policies to secure network access.

3. **Application Security**
   - Deployed **NAXSI WAF** on **OPNsense** to protect web servers in the **DMZ** zone.
   - Secured web traffic using encryption and implemented **HTTPS**.

4. **SIEM and Monitoring**
   - Installed and configured **Elastic Security** (part of the **Elastic Stack**) for real-time log ingestion, monitoring, and analysis across the network.
   - Integrated **Elastic Security** for advanced **EDR** capabilities, enabling endpoint monitoring, event correlation, and analysis.
   - Elastic Security's **SIEM** features allow the ingestion and processing of security event logs for comprehensive monitoring, detecting anomalies, and providing alerts for potential threats.
   - Used **Velociraptor** for endpoint monitoring across Windows 10, Ubuntu, and other systems within the network, feeding data into **Elastic Security** for enhanced detection and response.

5. **Incident Response**
   - Set up **Velociraptor** for incident response, logging, and monitoring suspicious activity across endpoints.
   - Integrated **Elastic Security SIEM** alerts with operational procedures for rapid incident detection and response.
   - Analyzed and responded to **security incidents** based on **Elastic Security** alerts and **Velociraptor** data, reducing time to mitigate potential threats.
   - Utilized **Elastic Security's** centralized logging and **Velociraptor's** endpoint monitoring to enhance incident response capabilities, identifying and mitigating threats in real-time.

---

### Screenshots

Example:
![Network Diagram]
(https://github.com/lyonzon2/ISSL/blob/main/cyber-lab.drawio.png)
*Ref 1: Network Diagram with pfSense(esxi), IPsec VPN, snort, ldap, and each network zone*

Example:
![GNS3 Toplogy](https://github.com/lyonzon2/ISSL/blob/main/infra-toplogy.png)
*Ref 2: Network Topology with pfSense(gns3), IPsec VPN, ,Suricata,Opensense(NAXSI), vm assets, secuirty solutions, and each network zone*
