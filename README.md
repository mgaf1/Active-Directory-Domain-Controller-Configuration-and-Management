<!-- <p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>
-->

# Active Directory Domain Controller Configuration and Management  

This project focuses on configuring and managing an Active Directory Domain Controller (DC). Key tasks include installing Active Directory Domain Services (AD DS), promoting a server to a DC, configuring DNS integration, and managing Group Policies. It demonstrates the process of setting up a domain and managing its core components.  

## Preparation: Operating System, Tools, and Resources  

- **Windows Server 2019** – Hosts the Active Directory Domain Controller  
- **Windows 10 (Client Machine)** – Connects to and tests the domain environment  
- **Stable Internet Connection** – Required for updates and domain synchronization  

## Objectives  

- **Install and run virtual machines** – Set up a virtualized environment for testing  
- **Configure networking for the virtual environment** – Choose NAT, Bridged, or Host-Only networking  
- **Create a functional domain environment** – Establish a secure and manageable domain structure  
- **Set up a new Active Directory forest and add a root domain** – Create the foundational AD structure  
- **Create an Administrator account** – Manage domain users and permissions  
- **Link a virtual Windows client machine to the Active Directory domain** – Enable centralized authentication and resource access

## Steps

 - **1. Insall Active Directory(AD)**
   - In this step, Navigate to the Manage tab and select **Add Roles and Features.**
 <img src="https://github.com/user-attachments/assets/fb7ba54a-e64d-415e-a3d4-954096831396"/>

<br></br>

 - **2. Adding Features in Add Roles and Features Wizard Pop-Up Window**
   -  When the pop-up window appears click on **Add Features**
   <img src="https://github.com/user-attachments/assets/9343c117-6cf7-459b-9d88-38aa331feebb"/>
<br></br>
- **3. Promote AD to a Domain Controller (DC)**
   -  When the pop-up window appears click on **Add Features**
   <img src="https://github.com/user-attachments/assets/a5d43db8-9bbd-41c9-bf67-5588f0a5ea12"/>



![5 creation of root domain](https://github.com/user-attachments/assets/7949531e-4b79-4296-a526-f3152396d361)
![6 creation of domain password](https://github.com/user-attachments/assets/fbaf83e1-a861-4d7d-860b-5ce7753522be)

![5 creation of root domain](https://github.com/user-attachments/assets/f530a746-5e99-4f23-87f9-f6f8f17ee5ef)


![8 checking all prerequisite before forest creation final installation](https://github.com/user-attachments/assets/b9e1e360-d013-4e35-8faf-2c07314eecc6)

![9 ad successfully promoted to domain controller](https://github.com/user-attachments/assets/a7c4671f-7231-47a8-aad5-1ad799f46c93)













<h2></h2>
Connecting a client machine to a domain server ensures efficiency within a network. 










<h2> Final Thoughts </h2>

<p>
In summary, Active Directory is crucial for managing user accounts and network resources. The scenarios provided cover common IT help desk tasks, such as creating user accounts, resetting passwords, updating group memberships, and handling account deactivation. These scenarios serve as practical exercises for training IT personnel and highlight the importance of Active Directory in maintaining a secure and organized digital environment. </p>
