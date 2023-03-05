
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Sharing Files Through the Same Network Tutorial</h1>
This tutorial displays how to share files and authorize permission levels to various users.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: Sharing Files Through the Same Network (https://youtu.be/kSnumGm2XD0)
- ### [YouTube: AD DS Prerequisite Installation (https://www.youtube.com/watch?v=VhZrN8monh0)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Active Directory Domain Services (AD DS)
- Window's File system

<h2>Operating Systems Used </h2>

- Windows Server 2022 Datacenter 
- Windows 10 PRO (21H2)

<h2>High-Level Deployment</h2>

- Prerequisite: Active Directory Domain Services Installed
- Create an Admin and some users
- Create 3 different folders
- Authorize access to user
- Create a Security Group Folder
- Demonstrate User attempts to folders


<h2>Network File Sharing and Permission step-by-step</h2>


<p> On the myhealthreport.com Domain Controller (DC), create 4 users.
  <p> At the Server Manager program, go to tools then to Active Directory Users and Computers.
     <p> Right-click on the left side bar > New > Users

<p align=center><img src="https://user-images.githubusercontent.com/121436228/222591834-3b6ff2ec-8344-42f1-a83a-36d84cbeab22.png"></p>
'
<p> Each of these users will have four levels of permission. To create the folders go to the myhealthreport.com DC, click on "File Explorer" then go to C:\. After that, right-click to "New" > Folder. </p>
  1. Read Only folder
  
  2. Read/Write folder
   
  3. No Access folder
  
  4. Security Group folder 
  5. 
  <p>This is created under the Active Director Users and Computers > right-click "New" > "Organizational Unit" > Create a new folder called "Board of Directors" > Right click on the right side of this folder > "New" > "Group" > Name it "BOD"> Group type: "Security" > Right click to "Properties" > Go to "Members"> "Add Dr. Barreau" </p>

<p align=center><img src="https://user-images.githubusercontent.com/121436228/222591810-3ba848ec-033a-490b-bf2a-348ea7840793.png"></p>

<p>In this tutorial we are going to use Dr. Barreau, the Board leader to access these four folders. 
  1. The "Doctor's research" folder will be the "Read Only" folder.
  2. The "Admin" folder will be the "Read and Write" folder.
  3. The "Patient's chart" will be the "No Access" folder.
  4. The "BOD (Board of Directors)" will be the "Read and Write" folder only for the Board Members to see.
  


<p align=center><img src="https://user-images.githubusercontent.com/121436228/222591788-26f7b906-4c21-4b8f-a57e-e6d116ea95fc.png"></p>

<p align=center><img src="https://user-images.githubusercontent.com/121436228/222591773-fddcad78-169f-4de2-aca4-821924edc1b4.png"></p>







