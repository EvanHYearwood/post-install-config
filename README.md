<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
<p>This tutorial provides a detailed overview of the post-installation configuration process for the open-source help desk ticketing system, osTicket. In this phase, we will take the system from its initial setup (Alpha) to a fully operational help desk system, ready for handling real-world support tickets.</p>

<h2>Environments and Technologies Used</h2>
<p>The following environments and technologies are employed in this tutorial:</p>
<ul>
  <li><strong>Microsoft Azure:</strong> Virtual machines and cloud compute services are used to host the osTicket installation.</li>
  <li><strong>Remote Desktop:</strong> Secure access to the virtual machine hosting osTicket for configuration and management purposes.</li>
  <li><strong>Internet Information Services (IIS):</strong> Web server software that hosts the osTicket web application on Windows.</li>
</ul>

<h2>Operating Systems Used</h2>
<p>In this tutorial, the following operating system was utilized:</p>
<ul>
  <li><strong>Windows 10 (21H2):</strong> The operating system installed on the virtual machine to run the IIS server and osTicket application.</li>
</ul>

<h2>Phase 2: Configuration</h2>
<p><strong>Goal:</strong> The goal of this phase is to take the osTicket system from its Alpha state (basic installation) into a fully operational system that can handle tickets, user requests, and support staff assignments.</p>

<h3>Step 1: Set up and Configure Key Components</h3>
<p>In this step, we will configure important components within osTicket to ensure it functions effectively. These components include:</p>
<ul>
  <li><strong>Roles:</strong> Assign roles to different agents, such as Admins and Support Staff, to manage access and permissions.</li>
  <li><strong>Departments:</strong> Create various departments (e.g., IT, Customer Support) to handle tickets based on the type of request.</li>
  <li><strong>Teams:</strong> Configure teams that handle specific types of support, such as Level I or Level II support.</li>
  <li><strong>Agents (Workers):</strong> Add agents who will manage and resolve tickets.</li>
  <li><strong>Users (Customers):</strong> Add the users who will submit tickets to the help desk.</li>
  <li><strong>SLAs (Service Level Agreements):</strong> Configure SLAs to ensure timely ticket resolutions based on severity.</li>
  <li><strong>Help Desk Topics:</strong> Define help topics to categorize tickets based on the issues users may encounter.</li>
</ul>

<h3>Step 2: Enable the Ticketing System</h3>
<p>In this step, we will configure osTicket to allow users to create tickets after registering an account. This ensures that the system is operational and ready to receive support requests from users.</p>

<h3>Outline for Step 1: Configuration</h3>

<ul>
  <li><strong>Configure Roles</strong>
    <ul>
      <li>Navigate to: Admin Panel -> Agents -> Roles</li>
      <li>Assign the "Supreme Admin" role for full administrative control.</li>
    </ul>
  </li>
  
  <li><strong>Configure Departments</strong>
    <ul>
      <li>Navigate to: Admin Panel -> Agents -> Departments</li>
      <li>Create a department called "System Administrators" to handle high-priority system-level issues.</li>
    </ul>
  </li>
  
  <li><strong>Configure Teams</strong>
    <ul>
      <li>Navigate to: Admin Panel -> Agents -> Teams</li>
      <li>Set up Level I and Level II support teams to handle different tiers of support requests.</li>
    </ul>
  </li>
  
  <li><strong>Configure Agents (Workers)</strong>
    <ul>
      <li>Navigate to: Admin Panel -> Agents -> Add New</li>
      <li>Add agents like "Jane" and "John" to handle incoming tickets.</li>
    </ul>
  </li>
  
  <li><strong>Configure Users (Customers)</strong>
    <ul>
      <li>Navigate to: Agent Panel -> Users -> Add New</li>
      <li>Add users like "Karen" and "Ken" who will submit tickets for support.</li>
    </ul>
  </li>
  
  <li><strong>Configure SLA (Service Level Agreements)</strong>
    <p>SLAs define the timeframes within which tickets should be resolved based on their severity. Proper configuration of SLAs ensures critical issues are prioritized and handled efficiently.</p>
    <ul>
      <li>Navigate to: Admin Panel -> Manage -> SLA</li>
      <li>Set up the following SLAs:
        <ul>
          <li><strong>Sev-A:</strong> 1 hour, 24/7 coverage for critical system outages.</li>
          <li><strong>Sev-B:</strong> 4 hours, 24/7 coverage for high-priority issues like software failures.</li>
          <li><strong>Sev-C:</strong> 8 hours, business hours coverage for less critical issues, such as password resets.</li>
        </ul>
      </li>
    </ul>
  </li>
  
  <li><strong>Configure Help Topics</strong>
    <p>Help topics categorize the types of support requests users may submit. Proper categorization helps route tickets to the correct team or department.</p>
    <ul>
      <li>Navigate to: Admin Panel -> Manage -> Help Topics</li>
      <li>Add common help topics such as:
        <ul>
          <li>Business Critical Outage</li>
          <li>Personal Computer Issues</li>
          <li>Equipment Request</li>
          <li>Password Reset</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>

<h3>Outline for Step 2: Enable Ticketing</h3>
<p>Once the configuration is complete, osTicket must be enabled to allow users to submit tickets. This step ensures that only registered users can create tickets, maintaining a secure and organized support system.</p>

<ul>
  <li><strong>Allow anyone to create tickets</strong>
    <ul>
      <li>Navigate to: Admin Panel -> Settings -> User Settings</li>
      <li>Enable "Registration Required" to ensure users register and log in before submitting tickets.</li>
    </ul>
  </li>
</ul>