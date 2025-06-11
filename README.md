# Windows Server 2022 Domain Infrastructure Lab
## Objective
With this project, I aimed to create a simulated enterprise environment by deploying Windows Server 2022 as an Active Directory Domain Controller (AD DC). This involves configuring essential network services such as DHCP and DNS, managing users and groups, and integrating a Windows 10/11 client into the domain. This hands-on experience was designed to deepen my understanding of Windows Server administration, Active Directory management, and network configuration, providing a practical learning environment for testing domain-related tasks, user authentication, and security policies.

## Skills Learned

- ✅ **Installing and configuring Windows Server 2022**  
- ✅ **Promoting a server to a Domain Controller (DC)**  
- ✅ **Creating and managing Organizational Units (OUs)**  
- ✅ **Setting up and configuring DHCP & DNS**  
- ✅ **Creating and managing user accounts & groups**  
- ✅ **Joining a Windows 10 client to the domain**  
- ✅ **Resetting user passwords in Active Directory**  

## Implementation 

### Step 1. Installing Windows Server 2022
- Installed Windows Server 2022 (Standardr) on a VMware workstation VMware 

**Ref 1:Server Setup**
![W22install](https://github.com/user-attachments/assets/d51257da-6645-47c8-8e19-f43cc4ea8b83)

---

### Step 2. Setting Up Active Directory Domain Services (AD DS)

- Installed the AD DS role via Server Manager.
- Promoted the server to a Domain Controller (DC).
- Created a new domain: myorg.local.

**Ref 2: AD DS Installation & Domain Configuration**
![ADDC](https://github.com/user-attachments/assets/8b707b01-a842-4212-a37f-79f03ec398ac)

---

### Step 3. Creating Organizational Units (OUs)

- Opened Active Directory Users and Computers (ADUC).
- Created OUs.

**Ref 3:OU Structure in ADUC**
![CreateOU](https://github.com/user-attachments/assets/6ffff012-bb3d-414d-94e0-06d22b7c2e7c)

---

### Step 4. Configuring DHCP & DNS

- Installed the DHCP Server role.
- Configured a DHCP scope 
- Verified DNS resolution 

**Ref Step 4: DHCP Scope**
![DCHP](https://github.com/user-attachments/assets/a5a07a8e-145c-49e3-b91b-a0f1ce6db6b4)

---
**DNS Records**
![DNS](https://github.com/user-attachments/assets/0810298e-d83e-4bdf-9c98-fc56014483cf)

---

### Step 5. Creating Users & Groups

- Added users (Lola Joker, Vitor Joker) in ADUC.
- Created a security group ( Admin).
- Assigned users to the group. (Victor to Admin group)

**Ref 5: User Accounts & Group Membership**
#### Created Users and Group.
![Create_UG](https://github.com/user-attachments/assets/75b41ef9-bbcc-4159-a0ed-4445aefafc4f)

---

#### Added User to Group.
![Create_UjoinGr](https://github.com/user-attachments/assets/3c7cb372-c90a-49bd-b761-fe15e8c5213b)

---

### Step 6. Installing & Joining a Windows 10 Client

- Installed Windows 10 on a VM.

**Ref 6: Windows 10 client install**
![Win10inst](https://github.com/user-attachments/assets/bb30a524-619d-4b1d-a058-85a962a86e26)

---

- Changed DNS settings to point to the Domain Controller.
- Joined the client to myorg.local domain.
  
**Ref 6.1: Windows 10 Joining the Domain**
![JoinDom1](https://github.com/user-attachments/assets/15aa164d-2602-4d88-ac8f-1c1d8723a849)

---

### Verification

- Logged into the Windows 10 client with a domain account.
- Checked DHCP lease and DNS resolution.

**Ref 8: Successful Domain Login on Win 10**
![Joined](https://github.com/user-attachments/assets/ff1ababe-097f-4baa-aa76-a12ec6fb1c50)

---

### Step 7. Resetting a User Password

- Logged into the Domain Controller.
- Opened ADUC, located a user, and reset their password.
- Verified login on the Windows 10 client.

**Ref 7: Password Reset in ADUC**

---

### Step 8. Group Policy Management

 ⏳⏳⏳⏳
