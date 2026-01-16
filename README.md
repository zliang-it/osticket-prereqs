# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial walks through the prerequisites and installation process of the open-source help desk ticketing system osTicket.<br /> 
<br /> 
At a high level, osTicket (short for Open Source Ticketing System) is a ticketing system. A ticket represents any issues, requests, or tasks, either from end users or internal staff. osTicket functions as a way for users to report issues and a tool IT teams can use to manage, track, and resolve tickets. For example, an employee's printer might be jammed. They submit a ticket, which lands in the IT Help Desk queue. An agent then grabs the ticket, goes to fix the printer, and closes the ticket, which automatically notifies the employee that the problem is solved.
<br />
<br />
osTicket and other ticketing systems aim to solve the problem of managing lots of issues, tasks, and requests. Without ticketing systems, there would be lost tickets, no accountability, wasted efforts, a lack of documentation, and unhappy customers. By acting as a central hub, ticketing systems add structure, communication, accountability, and documentation to the process of solving issues. This is why help desks, customer support, and IT management rely on it for efficient and quality service. 

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>



<h3>Step 1: Create Windows Virtual Machine.</h3> 

<p>
The first step of installing osTicket is creating the comptuer where our ticketing system will live. We will create a windows virtual machine on Azure functioning as our workstation or working computer. So let's head over to Azure.
</p>

<p>
<img width="1470" height="835" alt="bascis_p1" src="https://github.com/user-attachments/assets/5bec22de-b3a3-4e7a-86d3-1b3ed7b42e60" />
<img width="1470" height="831" alt="basics_p2" src="https://github.com/user-attachments/assets/0c5d23b8-4b12-4346-9317-b2f7b677d95a" />
When creating our virtual machine, the main focus is the Basics tab. Key things we need to do is name the virutal machine and pick which resource group to store it ('Resource group', 'Virtual machine name'), select the region our resource goes (Region), selecting the modern windoms operating system (Image), and give it some computing power (Size). After, we cab simply skim through the other tabs and leave the defualt values as is.
</p>

<p>
<img width="1470" height="956" alt="Screenshot 2025-11-22 at 11 22 11 AM" src="https://github.com/user-attachments/assets/4a393cfc-5458-4180-b262-48b196b67579" />
Next, in Windows App (formerly Remote Desktop), add our windows virtual machine as a new PC and connect to it. 
</p>

<p>
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 30 42 PM" src="https://github.com/user-attachments/assets/e73d7729-7a18-40c0-809c-cf5e74df3bf2" />
Then grab the installation files and open it on the virtual machine.
</p>

</hr>

<h3>Step 2: Set Up Web Server Environment</h3>

Now it's time to install our web server environment. What is a web server environment? It's the underlying system behind any website or application on the internet. It stores websites and applicaitons on the internet and delievers them to users. Why do we need to build a web server environment before installing the application? That is because a web server environment is the infrastucutre of our application. What does it actually do? Web server environments are responsbile for handling request - response cycles. Our server is constantly listening to users asking to view our application. These requests are made by a web browser whenever a user types the URL of our application. Our server (along with other parts discussed later) will send a response answering the user's request, in this case the answer will be our osTicket Help Desk page (for customers) or the internal application (for workers).

The main three parts of a web server environment are the server itself (we'll be using window's IIS), the database, and the scripting languge



<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 32 30 PM" src="https://github.com/user-attachments/assets/d998db20-433c-4b1e-ad00-f4353932213f" />

Install PHP Manager (for IIS) and PHP 
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 36 22 PM" src="https://github.com/user-attachments/assets/08115c3f-a11e-434f-8c17-a0286f1efdf0" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 40 11 PM" src="https://github.com/user-attachments/assets/2e46ba8f-e80b-4da8-adde-63a110970778" />

Install SQL
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 43 27 PM" src="https://github.com/user-attachments/assets/a58b0546-8be2-4c4c-b567-2bbf92217e91" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 44 11 PM" src="https://github.com/user-attachments/assets/1dff255c-0e34-489f-99a6-67db10b3ff59" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 45 01 PM" src="https://github.com/user-attachments/assets/f48ba339-6bba-4011-854b-c4d6d68cbade" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 45 19 PM" src="https://github.com/user-attachments/assets/b5d1e43b-8746-4272-af71-b1028fdcea52" />

Register PHP in IIS
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 47 28 PM" src="https://github.com/user-attachments/assets/6e1a5e10-cc4c-4e12-a4b8-53c8063ea220" />


<p>
Step 3: application install  

<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 52 46 PM" src="https://github.com/user-attachments/assets/385731fe-fa33-4d56-a105-490e60f0763b" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 53 24 PM" src="https://github.com/user-attachments/assets/78ac2aa2-b367-4ade-a7a6-0426c732888c" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 12 54 51 PM" src="https://github.com/user-attachments/assets/3f7a22ed-6e72-41e2-934b-6abeee94820c" />
</p>

<p>
Step 4: setup wizard + database connection 

<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 20 39 PM" src="https://github.com/user-attachments/assets/b1be606f-6a10-4750-87e8-2e6e78000e88" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 33 42 PM" src="https://github.com/user-attachments/assets/021f3603-c8e0-48d9-a9e1-d593884dfdf1" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 35 51 PM" src="https://github.com/user-attachments/assets/59307067-761e-4445-93e0-9ecba2e63794" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 36 02 PM" src="https://github.com/user-attachments/assets/fcddb29b-e7d6-4701-88e4-4f8abcf23b1f" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3a485f14-8971-4712-aba9-1362ed02203b" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 44 30 PM" src="https://github.com/user-attachments/assets/8e629541-8a6c-4431-802a-5333f79bc126" />
<img width="1470" height="956" alt="Screenshot 2025-12-04 at 3 49 11 PM" src="https://github.com/user-attachments/assets/6838def3-7179-4628-8992-e54699d91600" />
</p>

<p>
  Congratulations & Clean up
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a3364740-aa0d-47ba-b4bf-842987f0997d" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3f5b03de-1fef-46a4-91a8-944393f79857" />

Clean up phase
<img width="1470" height="956" alt="delete setup" src="https://github.com/user-attachments/assets/c44f8133-6d16-415d-aaeb-d97f5193d8a1" />
<img width="1470" height="956" alt="after delete" src="https://github.com/user-attachments/assets/6c47a15d-f0d7-4aa5-969d-693a91b27afe" />
<img width="1470" height="956" alt="change ost perms" src="https://github.com/user-attachments/assets/286cb3be-ab90-4692-b51f-5961505457dd" />

</p>

