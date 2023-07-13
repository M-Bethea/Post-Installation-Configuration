<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Azure VMs
- osTicket

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/e774d627-d879-41bb-91eb-c4c10527a6de" height="70%" width="70%" alt="Configure Roles"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/d8e87543-3dce-4b09-bd5b-9b013b31d929" height="70%" width="70%" alt="Configure Roles"/>
</p>
<p>
1. Configure <a href="https://imgur.com/a/JzSxC9L">Roles</a> <br>
  A. Admin Panel -> Agents -> Roles <br>
  B. Add New Role -> Type "Supreme Admin" -> Checkmark all boxes under "Permissions" (tickets, task, and knowledeg) -> Add Role
</p>
<br />

<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/7d00d93f-4c9d-44a3-9a6c-704f885fb821" height="70%" width="70%" alt="Configure Departments"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/773b696c-ae94-48e1-a62e-938fcc02e8f7" height="70%" width="70%" alt="Configure Departments"/>
</p>
<p>
2. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Departments</a><br>
    A. Admin Panel -> Agents -> Departments <br>
    B. Add New Department -> Type "System Administrators" -> Create Dept
</p>
<br />

<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/e8ed17ad-4714-4d96-a091-bcac076e3228" height="70%" width="70%" alt="Configure Teams"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/eb3a3832-0c70-4a1c-9857-9b8d7cbc6b55" height="70%" width="70%" alt="Configure Teams"/>
</p>
<p>
3. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Teams</a> <br>
  A. Admin Panel -> Agents -> Teams <br>
  i.  Level I Support <br>
  ii. Add New Team -> Level II Support -> Create Team
</p>
<br />

<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/89e4f2ef-f263-4dd2-9c03-deb601c869f0" height="70%" width="70%" alt="Create Ticket"/>
</p>
<p>
  4. Allow anyone to <a href="https://docs.osticket.com/en/latest/Developer%20Documentation/API/Tickets.html#:~:text=Tickets%20can%20be%20created%20in,format%20of%20the%20request%20content.">Create Tickets</a> <br>
  A. Admin Panel -> Settings -> Users <br>
  B. Registration Required: Require registration and login to create tickets 
    i. Make sure Registration Method says "Public - Anyone Can Register"
</p>
<br />

<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/0a4017f8-cc1c-4a6e-8cce-b613b04526c7" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/6842365b-2c18-4f9f-a876-1f39f7c2ed6e" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/f0992309-60f5-4c0c-96b5-358ba6739131" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/78af1cd1-4021-46d1-9f2d-f83cb0e7583e" height="70%" width="70%" alt="Configure Agents"/>
</p>

<p>
5. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents (workers)</a> <br>
  A. Admin Panel -> Agents -> Add New <br>
  i. Jane: Add new agent -> Fill out first name, last name, email and username -> Set Password -> Go to Teams -> Choose Support Level -> Add -> Create <br>
  ii. John
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Configure Users"/>
</p>
<p>
6. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Users (customers)</a> <br>
  A. Agent Panel -> Users -> Add New <br>
  i. Karen <br>
  ii. Ken 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Configure SLA"/>
</p>
<p>
7. Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">SLA</a> <br>
  A.Admin Panel -> Manage -> SLA <br>
  i. Sev-A (1 hour, 24/7) <br>
  ii. Sev-B (4 hours, 24/7) <br>
  iii. Sev-C (8 hours, business hours)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Configure Help Topics"/>
</p>
<p>
8. Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html">Help Topics</a> <br>
  A. Admin Panel -> Manage -> Help Topics <br>
  i. Business Critical Outage <br>
  ii. Personal Computer Issues <br>
  iii. Equipment Request <br>
  iv. Password Reset
</p>
<br />
