<p align="center">
  <img src="https://github.com/user-attachments/assets/48ecb6c3-9465-4d26-9c94-5eee9f6ea8ee" width="300"/>
</p>

<h1> Active Directory Domain Controller Configuration and Management</h1>

This project covers setting up and managing an Active Directory Domain Controller (DC), including installing AD DS, promoting a server to a DC, configuring DNS, and managing Group Policies.

## Preparation: Operating System, Tools, and Resources  

- **Windows Server 2019** 
- **Windows 10 (Client Machine)**  
- **Virtual Box**
- **Stable Internet Connection** 

## Objectives  

- **Install and run virtual machines** – Set up a virtualized environment.
- **Create a functional domain environment** – Establish a secure and manageable Domain structure.
- **Set up a new Active Directory forest and create a Root Domain** –  This creates the main system that organizes and manages all computers and users in the network.  
- **Create an Administrator account** – Manage domain users and permissions.  
- **Link a virtual Windows client machine to the Active Directory domain** – Allows users to log in and access network resources from one central system.
- **AD Objects Management** - Create user accounts and organize them into departments for easier management.

## Steps

 - **1. Insall Active Directory(AD)**
   - Navigate to the Menu tab, click **Manage** and select **Add Roles and Features**.
 <img src="https://github.com/user-attachments/assets/00660db0-54b6-4c77-9b55-5b8082e4aae2"/>

<br></br>
  - **Add Roles and Features**
    - Click on **Add Features** to install  **Active Directory Domain Services** and **DNS Server**.
   <img src="https://github.com/user-attachments/assets/9343c117-6cf7-459b-9d88-38aa331feebb"/>

  <br></br>
  - **Select the roles to add to the Server**
    - Select **Active Directory Domain Services** and **DNS Server**. The DNS server will translate domain names into IP addresses so that computers can find each other in our network.
      - Click Install to proceed
      - Wait for the installation to finish.
  <img src="https://github.com/user-attachments/assets/c161c795-a257-469b-8997-c90afcc6fa52"/>

<br></br>
- **2. Promote AD to a Domain Controller (DC)**
 - An **alert icon** will appear next to the flag icon in the menu tab when installation is complete.
  - Click on the flag icon in the Menu tab, then click **Promote this Server to a Domain Controller**
   <img src="https://github.com/user-attachments/assets/a5d43db8-9bbd-41c9-bf67-5588f0a5ea12"/>
  <br></br>
  
  - **Creation of root domain name** - For this lab,the root domain will be **mydomain.local**.
 <img src="https://github.com/user-attachments/assets/7949531e-4b79-4296-a526-f3152396d361"/>
  <br></br>

  - **Create a strong password** - This credentials will be used to log on to the **AD**.
 <img src="https://github.com/user-attachments/assets/8c378a43-6dee-42c5-8dc0-c6ef3671dca3"/>
<br></br>

   - **Check All Prerequisites Before Final Installation** – These are the components that need to be installed.
 <img src="https://github.com/user-attachments/assets/8653fb7c-7577-4269-b83b-940b375e108d"/>
  <br></br>
  
   - Next, a pop-up window will appear to confirm installation was sucessful.
 <img src="https://github.com/user-attachments/assets/9921eb15-b810-43e4-a6b7-cbb678f9af5c"/>

 <br></br>
- **3.Create Organisational Units and Users in Active Directory** – The Administrator account will be used to manage **Users**,**Organisation Units (O.U)**
  **groups** and **computers**.
   - In the Menu, click **Tools** and select **Active Directory Users and Computers**.
 <img src="https://github.com/user-attachments/assets/62e98bae-14fc-460c-8ed0-5f09348b335e"/>

<br></br>
 - Click on the dropdown icon next to the **Domain Name** you created for your forest to display all the **AD Objects** 
<br></br>
- **Create Organisational Unit (O.U) named ADMINS ,EMPLOYEES and USERS** - These serve as containers for users and their respective departments.
<br></br>

<img src="https://github.com/user-attachments/assets/a88c3035-bda4-4132-9164-b942a2b9f20c"/>
<br></br>

- **Create Administrator and User Accounts** - These accounts will be used to access **mydomain.local**
  - Right-click on ADMIN, Left-click to select **New User**(eg. in this lab **michael**)
    - Now the user is created.Double-click the new user account, go to **Properties**, and click the **Member Of** tab to add **M Gaf** to **Domain Admins**
  <br></br>
  <img src="https://github.com/user-attachments/assets/38a1963f-f725-4075-a110-78458f0479e9"/>

   <img src="https://github.com/user-attachments/assets/a9cd6022-1695-4a5e-a80f-fd2fea190fca"/>
<br></br>

- **Log Out and Log In to AD** – Use the newly created user **Michael** to sign in to the domain server.
  <br></br>
  <img src= "https://github.com/user-attachments/assets/239c4472-8b82-4e0e-aa31-38c761af01c2"/>

- **4. Link Virtual WINDOWS client Machine to AD Domain controller**- To enable centralized authentication and user management .

  - **Set the AD DC IP as the client's preferred DNS** - To enable domain name resolution, authentication, and Group Policy application.
    <img src="https://github.com/user-attachments/assets/dd17d1b6-37e5-4ffc-ae51-cef402a50b8f"/>
   <br></br>
   
  - Open the Windows client machine, go to Settings, and select System.
  - Scroll down and righ-click Advance system settings
  - Click the Computer Name tab and then select **Change** to connect the client machine to the AD Domain..
  - Name the client machine (e.g., **Target** for this lab).
  - Unselect Workgroup and Select Domain to join client to AD DC.
  <br></br>
  <img src="https://github.com/user-attachments/assets/c9dd8ec1-a665-4eef-b4dd-24e44c9b1e96"/>
<br></br>
  - **Logout and log back into client machine as Admin user account **michael****
  <br></br>
  
  <img src="https://github.com/user-attachments/assets/99ff36f0-d288-4da8-af61-2c943a48441f"/>


<h2> Conclusion </h2>
<p>
This project sets up an Active Directory Domain Controller to manage users and resources in a network. It helps keep everything organized, secure, and easy to manage. </p>
