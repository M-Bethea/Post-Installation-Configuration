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

- Configure Roles
- Configure Departments
- Configure Teams
- Assign Permissions
- Configure Agents
- Configure Users
- Configure SLA's
- Configure Help Topics

<h2>Configuration Steps</h2>

1. Configure <a href="https://imgur.com/a/JzSxC9L">Roles</a> <br>
  &nbsp; A. Admin Panel -> Agents -> Roles <br>
  &nbsp; &nbsp; B. Add New Role -> Type "Supreme Admin" -> Checkmark all boxes under "Permissions" (tickets, task, and knowledeg) -> Add Role
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/e774d627-d879-41bb-91eb-c4c10527a6de" height="70%" width="70%" alt="Configure Roles"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/d8e87543-3dce-4b09-bd5b-9b013b31d929" height="70%" width="70%" alt="Configure Roles"/>
</p>
<br />

<p>
2. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Departments</a><br>
    &nbsp; A. Admin Panel -> Agents -> Departments <br>
    &nbsp; &nbsp; B. Add New Department -> Type "System Administrators" -> Create Dept
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/7d00d93f-4c9d-44a3-9a6c-704f885fb821" height="70%" width="70%" alt="Configure Departments"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/773b696c-ae94-48e1-a62e-938fcc02e8f7" height="70%" width="70%" alt="Configure Departments"/>
</p>
<p>
<br />

<p>
3. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Teams</a> <br>
 &nbsp;  A. Admin Panel -> Agents -> Teams <br>
 &nbsp; &nbsp;  i.  Level I Support <br>
&nbsp; &nbsp; &nbsp;   ii. Add New Team -> Level II Support -> Create Team
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/e8ed17ad-4714-4d96-a091-bcac076e3228" height="70%" width="70%" alt="Configure Teams"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/eb3a3832-0c70-4a1c-9857-9b8d7cbc6b55" height="70%" width="70%" alt="Configure Teams"/>
</p>
<p>
<br />

<p>
  4. Allow anyone to <a href="https://docs.osticket.com/en/latest/Developer%20Documentation/API/Tickets.html#:~:text=Tickets%20can%20be%20created%20in,format%20of%20the%20request%20content.">Create Tickets</a> <br>
 &nbsp;  A. Admin Panel -> Settings -> Users <br>
  &nbsp; &nbsp; B. Registration Required: Require registration and login to create tickets 
    &nbsp; &nbsp; &nbsp; i. Make sure Registration Method says "Public - Anyone Can Register"
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/89e4f2ef-f263-4dd2-9c03-deb601c869f0" height="70%" width="70%" alt="Create Ticket"/>
</p>
<br />

<p>
5. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents (workers)</a> <br>
  &nbsp; A. Admin Panel -> Agents -> Add New <br>
 &nbsp; &nbsp;  i. Jane: Add new agent -> Fill out first name, last name, email and username -> Set Password -> Go to Teams -> Choose Support Level -> Add -> Create  <br> 
  &nbsp; &nbsp; &nbsp; ii. !!! Important !!! Be sure to fill out (for the Sys Admin): Extended Access -> Support -> Add -> Select Role -> Supreme Admin -> Create  <br>
 &nbsp; &nbsp; &nbsp; &nbsp;  iii. John (Try giving John a different department and role)
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/0a4017f8-cc1c-4a6e-8cce-b613b04526c7" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/6842365b-2c18-4f9f-a876-1f39f7c2ed6e" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/71adf974-b47a-47d3-b6d5-b206864a50fe" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/78af1cd1-4021-46d1-9f2d-f83cb0e7583e" height="70%" width="70%" alt="Configure Agents"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/14ddb299-307e-44f9-ae8a-a10c575d3e87" height="70%" width="70%" alt="Configure Agents"/>
</p>
<br />

<p>
  6. Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Users (customers)</a> <br>
 &nbsp;  A. Agent Panel -> Users -> Add New <br>
  &nbsp; &nbsp; i. Karen: New User -> Email, Full Name -> Add User <br>
  &nbsp; &nbsp; &nbsp; ii. Ken 
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/1596c05d-02c2-4757-9e33-01cdb7975e25" height="70%" width="70%" alt="Configure Users"/>
</p>
<br />

7. Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">SLA</a> <br>
  &nbsp; A.Admin Panel -> Manage -> SLA <br>
 &nbsp; &nbsp;  i. Sev-A (1 hour, 24/7): Add New SLA Plan -> Name, Grace Period, Schedule -> Add Plan <br>
 &nbsp; &nbsp; &nbsp;  ii. Sev-B (4 hours, 24/7) <br>
 &nbsp; &nbsp; &nbsp; &nbsp;  iii. Sev-C (8 hours, business hours)
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/4eb62e18-c914-478f-be95-35cf52fa0d2c" height="70%" width="70%" alt="Configure SLA"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/2df47820-46ed-47c1-a7f0-a8a144f151a4" height="70%" width="70%" alt="Configure SLA"/>
</p>
<br />

8. Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html">Help Topics</a> <br>
 &nbsp;  A. Admin Panel -> Manage -> Help Topics <br>
  &nbsp; &nbsp; i. Business Critical Outage: Add New Help Topic -> Topic -> Add Topic <br>
  &nbsp; &nbsp; &nbsp; ii. Personal Computer Issues <br>
  &nbsp; &nbsp; &nbsp; &nbsp; iii. Equipment Request <br>
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; iv. Password Reset
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/34b3d90c-a446-40c6-8942-c8ec5617547a" height="70%" width="70%" alt="Configure Help Topics"/>
</p>
<p>
<img src="https://github.com/M-Bethea/Post-Installation-Configuration/assets/139162550/fcd158ba-b6f4-4607-9cce-d43a013197e8" height="70%" width="70%" alt="Configure Help Topics"/>
</p>
<br />
