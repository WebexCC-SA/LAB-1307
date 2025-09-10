In this lab, you will learn how to create Desktop Profiles and assign
all profiles to an Agent/Supervisor.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 47%" />
<col style="width: 47%" />
</colgroup>
<thead>
<tr>
<th rowspan="3">1.</th>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Desktop
Profiles</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Use Case: Agents should have access only to features necessary
for their roles on their desktops</p></span>
<p>Create an Agent Desktop Profile</p>
<p><em>Reminder: If a setting is not listed in the task instructions,
leave default settings or skip</em></p></th>
</tr>
<tr>
<td><ul>
<li><p>General</p>
<ul>
<li><p>Name: Company Desktop Profile</p></li>
<li><p>Type: Site</p></li>
<li><p>Site: Company HQ</p></li>
<li><p>Screen Popups: enabled</p></li>
</ul></li>
<li><p>Idle/Wrap-up Code</p>
<ul>
<li><p>Auto wrap-up with timeout of: 60 seconds</p>
<ul>
<li><p>Auto wrap-up extension: enabled</p></li>
</ul></li>
<li><p>Wrap-up Codes: all</p></li>
<li><p>Idle Codes: All</p></li>
<a href="https://help.webex.com/en-us/article/nvaf71f/Manage-desktop-profiles">Help Page</a>
</ul></li>
</ul></th>
<td><ul>
<li><p>Collaboration</p>
<ul>
<li><p>Entry point/ Queue targets: None</p></li>
<li><p>Buddy Teams: All</p></li>
</ul></li>
<li><p>Dial Plans</p>
<ul>
<li><p>Address Book: Company Address Book</p></li>
<li><p>Dial Plan: enabled</p></li>
<li><p>Select Dial Plan: Any Format</p></li>
</ul></li>
<li><p>Agent Statistics</p>
<ul>
<li><p>Logged-in team statistics: Enable</p></li>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3">2.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Contact Center
Users-&gt; Select User</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Use Case: All configured profiles must be assigned to each
agent for them to take effect.</p></span>
<p>Assign all previously created profiles to the agents</p></td>
</tr>
<tr>
<td><ul>
<li><p>User: Anita Perez</p>
<ul>
<li><p>User Profile: Supervisor</p></li>
<li><p>Contact Center: enable</p></li>
<li><p>Primary Team – None</p></li>
<li><p>Site: Company</p></li>
<li><p>Teams: Company, Support, Overseas and Sales Teams</p></li>
<li><p>Desktop Profile: Company Desktop Profile</p></li>
<li><p>Multimedia Profile: Agent MMP</p></li>
<li><p>Skill Profile: Anita Perez</p></li>
</ul></li>
<li><p>Users: Eric Steele, Kellie Melby and Rebekah Barretta</p>
<ul>
<li><p>Contact Center: enable</p></li>
<li><p>Site: Company</p></li>
<li><p>Teams: Overseas Team</p></li>
<li><p>Desktop Profile: Company Desktop Profile</p></li>
<li><p>Multimedia Profile: Agent MMP</p></li>
<li><p>Skill Profile: Relevant named profile</p></li>
<a href="https://help.webex.com/en-us/article/n524f2m/Manage-user-profiles-of-contact-center-users-in-Webex-Contact-Center">Help Page</a>
</ul></li>
</ul></td>
<td><ul>
<li><p>Users: Rebekah Barretta and Ricardo Filice</p>
<ul>
<li><p>Contact Center: enable</p></li>
<li><p>Site: Company</p></li>
<li><p>Teams: Company Team</p></li>
<li><p>Desktop Profile: Company Desktop Profile</p></li>
<li><p>Multimedia Profile: Agent MMP</p></li>
<li><p>Skill Profile: relevant named profile</p></li>
</ul></li>
<li><p>Users: Stefan Mauk and Taylor Bard</p>
<ul>
<li><p>Contact Center: enable</p></li>
<li><p>Site: Company</p></li>
<li><p>Teams: Sales Team</p></li>
<li><p>Desktop Profile: Company Desktop Profile</p></li>
<li><p>Multimedia Profile: Agent MMP</p></li>
<li><p>Skill Profile: Relevant named profile</p></li>
</ul></li>
</ul></td>
</tr>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>