# Active Directory and PowerShell Automation Lab

## **Overview**
This project documents the step-by-step process of setting up an **Active Directory Domain Controller** on **Windows Server**, configuring **DHCP**, setting up **Remote Access and NAT**, adding users with **PowerShell** and joining a **Windows client** to the domain. **Group Policy** is then used to apply security settings to different OUs.

## **Network Topology**
- **Domain Controller (AD-DC):** Windows Server
- **Client Machine:** Windows 10 or 11
- **Hypervisor:** Hyper-V, VMware or VirtualBox
- **Network Range:** 10.20.0.0/24
- **Domain:** corp.example

## **Project Objectives**
- Set up **Active Directory Domain Services (AD DS)**
- Configure a **DHCP Server**
- Set up **Remote Access and NAT** for internal routing
- Add users and **Organizational Units (OUs)** from a CSV file with PowerShell
- Join a Windows client to the domain
- Authenticate users and verify network connectivity
- Apply **Group Policy** to different OUs

---

## **1. Setting Up the Active Directory Domain Controller**
1. **Launch the Windows Server VM**
2. **Rename the network interfaces (Internal and External)**
3. **Assign a static IP to the internal NIC**
4. **Rename the server to AD-DC**
5. **Install Active Directory Domain Services**
6. **Promote the server to a domain controller**
7. **Verify the domain controller status**

## Setting Up the Active Directory Domain Controller - Visual Guide

<!-- screenshots -->


## **2. Installing and Configuring DHCP**
1. **Install the DHCP Server role**
2. **Create a DHCP scope**
3. **Set the router and DNS options**
4. **Authorize the DHCP server in Active Directory**
5. **Verify lease assignments**

## Installing and Configuring DHCP - Visual Guide

<!-- screenshots -->


## **3. Setting Up Remote Access and NAT**
1. **Install the Remote Access role**
2. **Enable Routing and Remote Access**
3. **Configure NAT for the internal network**
4. **Verify internet access from the internal network**

## Setting Up Remote Access and NAT - Visual Guide

<!-- screenshots -->


## **4. Adding Users and OUs with PowerShell**
1. **Prepare a CSV file with the user details**
2. **Write the PowerShell script to import the users**
3. **Run the script**
4. **Verify the users and OUs in Active Directory Users and Computers**

## Adding Users and OUs with PowerShell - Visual Guide

<!-- screenshots -->


## **5. Joining a Windows Client to the Domain**
1. **Install the Windows client VM**
2. **Check connectivity to the domain controller**
3. **Join the client to the domain**
4. **Sign in with a domain account**
5. **Verify the DHCP address**

## Joining a Windows Client to the Domain - Visual Guide

<!-- screenshots -->


## **6. Authenticating a Domain User**
1. **Pick a user from the CSV**
2. **Sign in to the client as that user**
3. **Verify the network configuration with ipconfig**
4. **Check the permissions that come with the user's OU**

## Authenticating a Domain User - Visual Guide

<!-- screenshots -->


## **7. Group Policy and Helpdesk Tasks**
1. **Create Group Policy Objects for different OUs**
2. **Apply a password policy and login restrictions**
3. **Restrict administrative access for standard users**
4. **Reset a password, unlock an account and move a user between OUs**

## Group Policy and Helpdesk Tasks - Visual Guide

<!-- screenshots -->


## **Project Outcomes & Key Results**
- **Automated User Creation** – Users and OUs created from a CSV with PowerShell
- **Working Network Services** – DHCP, DNS and NAT serving the internal network
- **Domain Join** – A Windows client joined and signed in with domain accounts
- **Policy Enforcement** – Group Policy applied and checked per OU

## **Potential Next Steps**
- **Deploy a file server with shared folders**
- **Configure RDP and VPN for remote access**
- **Add multi-factor authentication**

---

This project is part of my **Networking and Infrastructure portfolio**. For any inquiries, reach out via **[LinkedIn](https://www.linkedin.com/in/kimutai-fredrick/)**.

**_Built and documented by Fredrick Kimutai._**
