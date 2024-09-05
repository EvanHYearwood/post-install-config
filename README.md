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

<h2>Phase 2: Configuration</h2>

<p><strong>Goal:</strong> Take the system from Alpha into a fully launched or fully operational state.</p>

<h3>Step 1: Set up and Configure</h3>
<ul>
  <li><strong>Roles</strong>, <strong>Departments</strong>, <strong>Teams</strong>, <strong>Agents</strong> (Workers), <strong>Users</strong>, <strong>SLAs</strong>, and <strong>Help Desk Topics</strong>.</li>
</ul>

<h3>Step 2: Enable the Ticketing System</h3>
<ul>
  <li>Allow anyone to create a ticket after they’ve registered an account.</li>
</ul>

<h3>Outline for Step 1: Configuration</h3>

<ul>
  <li><strong>Configure Roles</strong>
    <ul>
      <li>Admin Panel -> Agents -> Roles</li>
      <li>Role: Supreme Admin</li>
    </ul>
  </li>
  
  <li><strong>Configure Departments</strong>
    <ul>
      <li>Admin Panel -> Agents -> Departments</li>
      <li>Department: System Administrators</li>
    </ul>
  </li>
  
  <li><strong>Configure Teams</strong>
    <ul>
      <li>Admin Panel -> Agents -> Teams</li>
      <li>Level I Support</li>
      <li>Level II Support</li>
    </ul>
  </li>
  
  <li><strong>Configure Agents (Workers)</strong>
    <ul>
      <li>Admin Panel -> Agents -> Add New</li>
      <li>Agent: Jane</li>
      <li>Agent: John</li>
    </ul>
  </li>
  
  <li><strong>Configure Users (Customers)</strong>
    <ul>
      <li>Agent Panel -> Users -> Add New</li>
      <li>User: Karen</li>
      <li>User: Ken</li>
    </ul>
  </li>
  
  <li><strong>Configure SLA</strong>
    <ul>
      <li>Admin Panel -> Manage -> SLA</li>
      <li>Sev-A (1 hour, 24/7)</li>
      <li>Sev-B (4 hours, 24/7)</li>
      <li>Sev-C (8 hours, business hours)</li>
    </ul>
  </li>
  
  <li><strong>Configure Help Topics</strong>
    <ul>
      <li>Admin Panel -> Manage -> Help Topics</li>
      <li>Business Critical Outage</li>
      <li>Personal Computer Issues</li>
      <li>Equipment Request</li>
      <li>Password Reset</li>
    </ul>
  </li>
</ul>

<h3>Outline for Step 2: Enable Ticketing</h3>
<ul>
  <li><strong>Allow anyone to create tickets</strong>
    <ul>
      <li>Admin Panel -> Settings -> User Settings</li>
      <li>Registration Required: Require registration and login to create tickets</li>
    </ul>
  </li>
</ul>