<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. Using made up scenerios on how users create tickets and agents working tickets to completion by observing the issue, setting SLAs, and how to complete a ticket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

### Setup:

<p>
<img width="958" height="351" alt="image" src="https://github.com/user-attachments/assets/0e88cbc5-2dc6-4aed-a831-dd811dcd2014" /> 
<img width="956" height="363" alt="image" src="https://github.com/user-attachments/assets/d0df7b16-246d-4bd7-a8cc-4a287c6b63f9" />
</p>
<p>
Delete the Maintenance Department. Admin Panel -> Agents -> Departments. Check Departments and Delete. This will ensure ticket flow and visibility and won't be routed to an unused department. 
</p>
<br />

### Scenerio #1: Banking System is Down
<p>
<img width="835" height="479" alt="image" src="https://github.com/user-attachments/assets/3bc15452-42cc-4523-96e9-51e87b394d05" />
</p>
<p>
Open a new page for the end users osTicket URL: http://localhost/osTicket/. Click Open a New Ticket. 
</p>
<br />

<p>
<img width="829" height="813" alt="image" src="https://github.com/user-attachments/assets/417e3dae-6d40-4dd9-8b3c-7272d4ea5074" />
</p>
<p>
In the creation of the new ticket I will use a fake end user called "karen". In the ticket as karen select the help topic as "General Inquiry / Other" (It should be business critical outage, but it will be fixed when observing the ticket as a support agent). Entered the made up scenerio in the summary. Submit the ticket. Note: The email being used is fake and only for this tutorial.
</p>
<br />

<p>
<img width="511" height="388" alt="image" src="https://github.com/user-attachments/assets/3728f4a3-c49d-489f-ad3a-8eea23b41f5c" />
</p>
<p>
In the Admin login (http://localhost/osTicket/scp/login.php) we are going to login as john as a help desk agent. If you can't login as john look at the previous tutorial.

</p>
<br />

<p>
<img width="956" height="886" alt="image" src="https://github.com/user-attachments/assets/d815f4d1-00f6-4596-919c-f327b409021c" />
<img width="951" height="325" alt="image" src="https://github.com/user-attachments/assets/2674b386-2f43-4a04-a9a9-c6e934c739e3" />
</p>
<p>
Open the most recent ticket. Observe the properties of the ticket (Priotity, Department, SLA, etc.). Notice john is in "read only" mode and can't do much except make an internal note. Feel free to leave a note, but its not necessary for the rest of this scenerio.
</p>
<br />

<p>
<img width="951" height="570" alt="image" src="https://github.com/user-attachments/assets/75f5f51e-0a7b-4261-96d5-b38a85ec829e" />
</p>
<p>
We now want to give John permissions to do more with the ticket. In the Admin Login page log back in as "adminuser". Navigate to Agent Panel -> Agents -> Agents -> John Doe -> Access. Give John "All access" and save changes.
</p>
<br />

<p>
<img width="952" height="785" alt="image" src="https://github.com/user-attachments/assets/64c19eb3-4836-43aa-96b8-6fa8ee21a655" />
</p>
<p>
Login back as john and view the ticket again. Notice you can change and modify the ticket. Update the Prioity from "Normal" to "Emergency" as the entire banking system being down is a big issue and needs to be dealt with right away. Update SLA to "Sev-A" (Sev-A is 1 hour, 24/7) because its urgent and needs to be completed ASAP. Update help topic from "General Inquiry / Other" to "Business Critical Outage".
</p>
<br />

<p>
<img width="950" height="76" alt="image" src="https://github.com/user-attachments/assets/6b43b08a-5284-4cc9-9c78-cd43f99379c4" />
</p>
<p>
This issue may need someone else to work on it to ensure the issue is handled correctly. Change the "Assigned to" to "Jane Doe" and Transfer the ticket to the Department of "SysAdmins". With the way Johns permissions are setup he will no longer have access to the ticket. 
</p>
<br />

<p>
<img width="955" height="955" alt="image" src="https://github.com/user-attachments/assets/9b7c6c27-10ee-4dcf-91fc-b86729b0b7dc" />
</p>
<p>
Logout as john and login as jane. Open the ticket that was worked on as john. Observe you can see everything that john did in the ticket thread before the ticket was transferred.
</p>
<br />

<p>
<img width="956" height="273" alt="image" src="https://github.com/user-attachments/assets/c3e44898-d563-4a0c-8601-349c562c1bf6" />
<img width="948" height="85" alt="image" src="https://github.com/user-attachments/assets/9e60caf6-c8f4-4236-8078-0d15a1847667" />
</p>
<p>
As jane we need to investigate and troubleshoot the issue, provide updates to the user, and resolve and close the ticket. I left 2 notes as "Jane" as she worked through the ticket. Once the ticket is completed changed the status from "Open" to "Resolved".  
</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />


