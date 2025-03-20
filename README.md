< <p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1> Active Directory Domain Controller Configuration and Management</h1>

This project focuses on configuring and managing an Active Directory Domain Controller (DC). Key tasks include installing Active Directory Domain Services (AD DS), promoting a server to a DC, configuring DNS integration, and managing Group Policies. It demonstrates the process of setting up a domain and managing its core components.  

## Preparation: Operating System, Tools, and Resources  

- **Windows Server 2019** – Hosts the Active Directory Domain Controller  
- **Windows 10 (Client Machine)** – Connects to and tests the domain environment  
- **Stable Internet Connection** – Required for updates and domain synchronization  

## Objectives  

- **Install and run virtual machines** – Set up a virtualized environment
- **Configure networking for the virtual environment** – In this lab I will be using Internal Network named **ADproject**
- **Create a functional domain environment** – Establish a secure and manageable Domain structure  
- **Set up a new Active Directory forest and add a root domain** – The new forest is the top level and serves as the main structure for the virtual environment.  
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
   
   <br></br>
- **4. Creation of root domain name** - In this lab,the root domain will be **mydomain.local**
 <img src="https://github.com/user-attachments/assets/7949531e-4b79-4296-a526-f3152396d361"/>

<br></br>
- **5. Creation of Domain Password** - This credentials will be used to log on to the (AD)
 <img src="https://github.com/user-attachments/assets/8c378a43-6dee-42c5-8dc0-c6ef3671dca3"/>
 

<br></br>
- **6. Check All Prerequisites Before Final Installation** – These are the components that need to be installed
 <img src="https://github.com/user-attachments/assets/8653fb7c-7577-4269-b83b-940b375e108d"/>
  <br></br>
  Next,You will see a pop-up window to confirm installation was sucessful
 <img src="https://github.com/user-attachments/assets/9921eb15-b810-43e4-a6b7-cbb678f9af5c"/>

 <br></br>
- **7.Create Adminstrator Account in AD** – The Administrator account will be used to manage User,Organisation Unit(O.U)
  groups and computers etc. In the Server Manager,look on the upright corner of the server manager and select he tab **Tools** and **Active Directory Users and Computers**
 <img src="https://github.com/user-attachments/assets/62e98bae-14fc-460c-8ed0-5f09348b335e"/>
 <br></br>
 - Click on the dropdown icon next to the **Domain Name** you created for your forest to display all the **AD Objects** 
  <img src="https://github.com/user-attachments/assets/02ad6de3-dc07-43be-8e8a-be8e3b3286a4"/>
<br></br>
- **8.Connecting a client machine to a Domain Server** To ensure efficiency within a network. 


<h2> Conclusion </h2>
<p>
In summary, Active Directory is used for managing user accounts and network resources. The scenarios provided cover common IT help desk tasks, such as creating user accounts, resetting passwords, updating group memberships, and handling account deactivation. These scenarios serve as practical exercises for training IT personnel and highlight the importance of Active Directory in maintaining a secure and organized digital environment. </p>
