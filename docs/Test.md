## Lab 1 - Getting Started with Agents

 Lab 1 – Agent Creation Part 1

In this lab, you will log in to Control Hub (CH) and learn how to assign
Webex Contact Center Licenses. Then you will create Skill Definitions,
Skill Profiles and Multimedia Profiles

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<td><span style="color: greenyellow;">Management-&gt; Users<em>-&gt;</em> Licenses-&gt; Organization-based
licenses</span></td>
</tr>
<tr>
<td><span style="color: Cyan;"><p>In addition to standard voice communications, agents will support customers using digital channels. </p></span>
<p>Assign Premium Agent licenses to all users </p>
<ul>
<li><p>License: Premium</p></li>
<li><p>Apply scope: Existing users, preserve licenses for existing
users.</p></li>
<li><p><em>Spot check any user to ensure they have a Premium Agent license</em></p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">2.</td>
<td><span style="color: greenyellow;">Management-&gt; Users<em>-&gt;</em> Anita Perez</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">In addition to Premium Agent access, Anita Perez will need to monitor and coach agents and access reporting and analytics </span></p>
<p>Add Contact Center Supervisor to Anita Perez</p>
<ul>
<li><p>License: Premium Agent</p></li>
<li><p>Add Supervisor Role</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Skill Definitions</span></td>
</tr>
<td><p><span style="color: Cyan;">Customer inquiries must be routed to the most qualified agents</span></p>
<p>Create several skills to be applied to agents</p>
<p>
</ul>
<li>Skill Name: Changes</li>
<ol>
<li>Skill Type: Proficiency</li>
</ol>
</ul>
<li>Skill Name: Adds</li>
<ol>
<li>Skill Type: Boolean</li>
</ol>
</ul>
<li>Skill Name: Moves</li>
<ol>
<li>Skill Type: Boolean</li>
</ol>
</ul>
<li>Skill Name: Changes</li>
<ol>
<li>Skill Type: Boolean</li>
</ol>
</ul>
<li>Skill Name: Overseas</li>
<ol>
<li>Skill Type: Boolean</li>
</ol>
</ul></p></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Skill Profiles,</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">Each agent has a unique set of skills that helps determine how calls are routed to them</span></p>
<p>Create Skill Profiles for 4 agents and 1 Supervisor</p>
<ul>
<p>Skill Profile Name: Eric Steele</p>
<li><p>Skill: Adds - True</p></li>
<li><p>Skill: Changes – 10</p></li>
<li><p>Skill: Moves - True</p></li>
<li><p>Skill: Overseas - True</p></li>
<li><p>Skill: Support - True</p></li>
<p>Skill Profile Name: Rebekah Barretta</p>
<li><p>Skill: Adds - True</p></li>
<li><p>Skill: Changes – 8</p></li>
<li><p>Skill: Support - True</p></li>
<p>Skill Profile Name: Kellie Melby</p>
<li><p>Skill: Adds - True</p></li>
<li><p>Skill: Changes – 10</p></li>
<li><p>Skill: Moves - True</p></li>
<li><p>Skill: Overseas - True</p></li>
<li><p>Skill: Support - True</p></li>
<p>Skill Profile Name: Ricardo Filice</p>
<li><p>Skill: Changes – 5</p></li>
<li><p>Skill: Moves - True</p></li>
<li><p>Skill: Support - True</p></li>
<p>Skill Profile Name: Anita Perez</p>
<li><p>Skill: Adds - True</p></li>
<li><p>Skill: Changes – 5</p></li>
<li><p>Skill: Moves - True</p></li>
<li><p>Skill: Overseas - True</p></li>
<li><p>Skill: Support – True</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">5.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Multimedia Profiles</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">Agents should handle only one chat at a time to ensure prompt responses. </span></p>
<p>Create multimedia profile to be applied to agents</p>
<ul>
<li><p>Profile Name: Agent MMP</p></li>
<li><p>Type: Exclusive</p></li>
<li><p>Voice and Chat only selected</p></li>
</ul></td>
</tr>
</tbody>
</table>
<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

## Lab 2 - Agent basics

 Lab 2 – Agent Creation: Part 2

In this lab, you will learn how to create Sites, Teams, Desktop Layouts,
Address Books and Auxiliary Codes.

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
<th rowspan="2">1.</th>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Sites</span></td>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Supervisors and admins require a straightforward
reporting solution for individual locations</p></span>
<ul>
<p>Create a site</p>
<ul>
<li><p>Name: Company HQ</p></li>
<li><p>MultiMedia Profile: Agent MMP</p></li>
</ul></td>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3">2.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Teams</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Supervisors and admins need to easily manage and
streamline queue assignments for groups of agents.</p></span>
<p>Create Teams for use in queues</p>
<ul>
<tr>
<td><ul>
<li><p>Name: Company Team</p>
<ul>
<li><p>Parent Site: Company HQ</p></li>
<li><p>Team Type: Agent Based</p></li>
</ul></li>
<li><p>Name: Overseas Team</p>
<ul>
<li><p>Parent Site: Company HQ</p></li>
<li><p>Team Type: Agent Based</p></li>
</ul></li>
</ul></td>
<td><ul>
<li><p>Name: Sales Team</p>
<ul>
<li><p>Parent Site: Company HQ</p></li>
<li><p>Team Type: Agent Based</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Desktop
Layouts</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Agents need to use Webex on their desktops</p></span>
<p>Create a new desktop layout to use Webex</p>
<ul>
<li><p>Name: Company Layout</p>
<ul>
<li><p>Teams: Company, Overseas and Sales</p></li>
<li><p>JSON File: Download the default desktop layout</p>
<ul>
<li><p>Open the file with a text editor</p>
<li><p>Find: Agent-&gt; DesktopChatApp-&gt;Webexconfigured, change false
to true</p></li>
<li><p>Repeat for Supervisor (further down the file)</p></li>
</li>
<li><p>Save the file as CompanyDesktopLayout.json</p></li>
</ul>
<li><p>Replace file in the Desktop Layout</p></li>
</li>
<li><p>Make sure to click Create</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Address
Books</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Agents and supervisors need to easily call the local
numbers they call on a regular basis</p></span>
<p>Create an Address Book for agents to use</p>
<ul>
<li><p>Name: Company Address Book</p></li>
<li><p>Type: Site</p></li>
<li><p>Site: Company HQ</p></li>
<li><p>Entry List</p>
<ul>
<li><p>Name: Joes Pizza</p></li>
<li><p>Contact Number: 2406568923</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="3">5.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Idle/Wrap-up
Codes</td><span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Outcomes for each customer/agent interaction need to
be categorized and tracked for reporting and analysis</p></span>
<p>Create codes for agent use after a call completes</p></td>
</tr>
<tr>
<td><p>Name: Support</p>
<ul>
<li><p>Make it default: enable</p></li>
<li><p>Code type: Default Wrap-up Work Type</p>
<p>Name: Service</p></li>
<li><p>Code type: Default Wrap-up Work Type</p></li>
</ul></td>
<td><p>Name: Sales</p>
<ul>
<li><p>Code type: Default Wrap-up Work Type</p>
<p>Name: Administration Time</p></li>
<li><p>Make it default: enable</p></li>
<li><p>Code type: Default Idle Work Type</p>
<p>Name: Break</p></li>
<li><p>Code type: Default Idle Work Type</p></li>
</ul></td>
</tr>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

# Lab 3 – Agent finalization

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
<td colspan="2"><span style="color: Cyan;"><p>Agents should have access only to features necessary
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
<td colspan="2"><span style="color: Cyan;"><p>All configured profiles must be assigned to each
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

# Lab 4 – Flow Pre-Work

In this lab, you will learn how to create Queues and Business Hours.

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
<th rowspan="2">1.</th>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Customer Experience -&gt; Business
Hours</th></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Agents should only be reached through queues during
set hours</p></span>
<p>Define Business Hours</p>
<ul>
<li><p>Overrides</p>
<ul>
<li><p>Name: Emergencies</p></li>
<li><p>Time zone: America/New York</p></li>
<li><p>Add new override</p>
<ul>
<li><p>Name: Emergency</p></li>
<li><p>Do NOT enable</p></li>
<li><p>Date range: Today’s date - 12/25/2025</p></li>
</ul></li>
</ul></li>
<li><p>Holiday Lists</p>
<ul>
<li><p>Name: Holidays</p></li>
<li><p>Holiday Number 1: Xmas</p>
<ul>
<li><p>12/25/2025 – 12/25/2025</p></li>
</ul></li>
<li><p>Holiday Number 2: Birthday</p>
<ul>
<li><p>Your 2026 birthday date (Hint – type the date in)</p></li>
</ul></li>
</ul></li>
<li><p>Working Hours</p>
<ul>
<li><p>Name: Work Week</p></li>
<li><p>Time zone: America/New York</p></li>
<li><p>Add Shift</p>
<ul>
<li><p>Name: Day</p></li>
<li><p>Mon – Fri: 9am - 5pm</p></li>
</ul></li>
<li><p>Holiday List: Holidays</p></li>
<li><p>Overrides: Emergencies</p></li>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3">2.</td>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Customer Experience -&gt;
Queues</td></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;"><p>Separate queues are needed for Support and Sales to
ensure customer inquiries are routed to the appropriate team.</p></span>
<p>Create two queues</p></td>
</tr>
<tr>
<td><p>Queue Name: Support Q</p>
<ul>
<li><p>Contact Routing Settings</p>
<ul>
<li><p>Skills-based routing: Enable</p></li>
<li><p>Skill assignment type: Assign skills in flows</p></li>
<li><p>Routing Pattern: Best Available Agent</p></li>
<li><p>Call Distribution: Group</p>
<ul>
<li><p>Priority 1: Company and Overseas teams</p></li>
</ul></li>
</ul></li>
<li><p>Advanced settings</p>
<ul>
<li><p>Service Monitoring: Enable</p></li>
<li><p>Allow pause/resume for calls: Enable</p></li>
<li><p>Service Level Threshold: 120</p></li>
<li><p>Max time in Queue: 3600</p></li>
<li><p>Music In Queue: defaultmusic_on_hold_cisco_opus</p></li>
</ul></li>
</ul></td>
<td><p>Queue Name: Sales Q</p>
<ul>
<li><p>Contact Routing Settings</p>
<ul>
<li><p>Agent Assignment: Teams</p></li>
<li><p>Call Distribution: Group</p></li>
<li><p>Priority 1: Sales team</p></li>
</ul></li>
<li><p>Advanced settings</p>
<ul>
<li><p>Service Monitoring: Enable</p></li>
<li><p>Allow pause/resume for calls: Enable</p></li>
<li><p>Service Level Threshold: 120</p></li>
<li><p>Max time in Queue: 3600</p></li>
<li><p>Music In Queue: defaultmusic_on_hold_cisco_opus</p></li>
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

#  Lab 5 – Flows

In this lab, you will learn how to create flows for queues.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.a.</th>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Each queue needs a specific flow to tailor the customer
experience and make sure inquiries are handled according to the team’s
processes</p></span>
<p>Flow Number 1</p>
<ul>
<li><p>Name: CompanyFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 44%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th><strong>Activity</strong></th>
<th colspan="2"><strong>Configuration - Main Flow</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2"><span style="color: gold;">Business Hours</td></span>
<td colspan="2">Title: Business Hours</td>
</tr>
<tr>
<td colspan="2">Static Business Hours: Work Week</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Message</td></span>
<td colspan="2">Title: Welcome</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to Global Support Solutions</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Menu</td></span>
<td colspan="2">Title: Menu 1</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p>
<p>Text: For support, please press 1, for service please press
2</p></td>
<td><p>Make Prompt interruptible: Enable</p>
<p>Make two Menu Links 1 and 2</p>
<p>1 = Support</p>
<p>2 = Service</p></td>
</tr>
<tr>
<td><span style="color: gold;">Menu</td></span>
<td colspan="2">Title: Menu 2</td>
</tr>
<tr>
<td></td>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p>
<p>Text: For additions press 1, for moves press 2 and for configuration
press 3.</p></td>
<td><p>Make Prompt interruptible: Enable</p>
<p>Make two Menu Links 1 and 2</p>
<p>1 = Adds</p>
<p>2 = Moves</p>
<p>3 = Changes</p></td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Blind Transfer</td></span>
<td colspan="2">Title: ToVmail</td>
</tr>
<tr>
<td colspan="2">Specific Number to Dial: 5000</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Queue Contact</td></span>
<td colspan="2">Title: SupportQ</td>
</tr>
<tr>
<td><p>Static Queue: Support Q</p>
<p>Set contact Priority: Value = 5</p></td>
<td>Skill: Support is True</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Queue Contact</td></span>
<td colspan="2">Title: AddQ</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td>Skill: Add is True</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Queue Contact</td></span>
<td colspan="2">Title: Move Q</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td>Skill: Move is True</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Queue Contact</td></span>
<td colspan="2">Title: Changes Q</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td>Skill: Changes &gt;= 4</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Music</td></span>
<td colspan="2">Title: PlayMusic</td>
</tr>
<tr>
<td>Audio File: defaultmusic_on_hold_cisco_opus_no_1.wav</td>
<td><p>Offset = 0</p>
<p>Music Duration: 3600</p></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 46%" />
<col style="width: 48%" />
</colgroup>
<thead>
<tr>
<td rowspan="4">1.b.</th>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;">Link the activities together</p></span>
</tr>
<tr>
<td><ul>
<li><p>NewPhoneContact Activity</p>
<ul>
<li><p>Output –&gt; Business Hours</p></li>
</ul></li>
<li><p>Business Hours Activity</p>
<ul>
<li><p>Holidays –&gt; ToVmail</p></li>
<li><p>Override -&gt; ToVmail</p></li>
<li><p>Default -&gt; ToVmail</p></li>
<li><p>Working Hours –&gt; Welcome</p></li>
</ul></li>
<li><p>Welcome Activity</p>
<ul>
<li><p>Output -&gt; Menu 1</p></li>
</ul></li>
<li><p>Menu 1 Activity</p>
<ul>
<li><p>Menu Link 1 –&gt; SupportQ</p></li>
<li><p>Menu Link 2 –&gt; Menu 2</p></li>
<li><p>No-Input Timeout -&gt; Start of Menu 1 Activity</p></li>
</ul></li>
</ul></th>
<td><ul>
<li><p>Menu 2 Activity</p>
<ul>
<li><p>Menu Link 1 –&gt; AddQ</p></li>
<li><p>Menu Link 2 –&gt; MoveQ</p></li>
<li><p>Menu Link 2 -&gt; ChangesQ</p></li>
<li><p>No-Input Timeout -&gt; Start of Menu 2 Activity</p></li>
</ul></li>
<li><p>All Queue Activities</p>
<ul>
<li><p>Output –&gt; PlayMusic</p></li>
</ul></li>
<li><p>PlayMusic Activity</p>
<ul>
<li><p>Output –&gt; Start of PlayMusic Activity</p></li>
</ul></li>
</ul></th>
</tr>
<tr>
<th colspan="2">Validate and Publish flow using Latest Version</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<td rowspan="2">2.a.</th>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
<p>Flow Number 2</p>
<ul>
<li><p>Name: OverseasFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 44%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th><strong>Activity</strong></th>
<th colspan="2"><strong>Configuration - Main Flow</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2"><span style="color: gold;">Business Hours</td></span>
<td colspan="2">Title: Business Hours</td>
</tr>
<tr>
<td colspan="2">Static Business Hours: Work Week</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Message</td></span>
<td colspan="2">Title: Welcome</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to the Global Support Solutions overseas department.
Please hold and we will be with you shortly.</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Blind Transfer</td></span>
<td colspan="2">Title: ToVmail</td>
</tr>
<tr>
<td colspan="2">Specific Number to Dial: 5000</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Music</td></span>
<td colspan="2">Title: PlayMusic</td>
</tr>
<tr>
<td>Audio File: defaultmusic_on_hold_cisco_opus_no_1.wav</td>
<td><p>Offset = 0</p>
<p>Music Duration: 3600</p></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 46%" />
<col style="width: 48%" />
</colgroup>
<thead>
<tr>
<th rowspan="4">2.b.</th>
<td colspan="2"><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td colspan="2"><span style="color: Cyan;">Link activities together</th></span>
</tr>
<tr>
<td><ul>
<li><p>NewPhoneContact Activity</p>
<ul>
<li><p>Output –&gt; Business Hours</p></li>
</ul></li>
<li><p>Business Hours Activity</p>
<ul>
<li><p>Holidays –&gt; ToVmail</p></li>
<li><p>Override -&gt; ToVmail</p></li>
<li><p>Default -&gt; ToVmail</p></li>
<li><p>Working Hours –&gt; Welcome</p></li>
</ul></li>
</ul></th>
<td><ul>
<li><p>Welcome Activity</p>
<ul>
<li><p>Output -&gt; OverseasQ</p></li>
</ul></li>
<li><p>OverseasQ Activity</p>
<ul>
<li><p>Output –&gt; PlayMusic</p></li>
</ul></li>
<li><p>PlayMusic Activity</p>
<p>Output –&gt; Start of PlayMusic Activity</p></li>
</ul></th>
</tr>
<tr>
<th colspan="2">Validate and Publish flow using Latest Version</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">3.a.</th>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><p>Flow Number 3</p>
<ul>
<li><p>Name: SalesFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 42%" />
<col style="width: 2%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th><strong>Activity</strong></th>
<th colspan="3"><strong>Configuration - Main Flow</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2"><span style="color: gold;">Business Hours</td></span>
<td colspan="3">Title: Business Hours</td>
</tr>
<tr>
<td colspan="3">Static Business Hours: Work Week</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Message</td></span>
<td colspan="3">Title: Welcome</td>
</tr>
<tr>
<td colspan="2"><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to the Sales Department of Global Support Solutions.
We will be with you shortly</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Blind Transfer</td></span>
<td colspan="3">Title: ToVmail</td>
</tr>
<tr>
<td colspan="3">Specific Number to Dial: 5000</td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Queue Contact</td></span>
<td colspan="3">Title: SalesQ</td>
</tr>
<tr>
<td>Static Queue: Sales Q</td>
<td colspan="2"></td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Play Music</td></span>
<td colspan="3">Title: PlayMusic</td>
</tr>
<tr>
<td colspan="2">Audio File:
defaultmusic_on_hold_cisco_opus_no_1.wav</td>
<td><p>Offset = 0</p>
<p>Music Duration: 3600</p></td>
</tr>
<tr>
<td rowspan="2"><span style="color: gold;">Blind Transfer</td></span>
<td colspan="3">Title: ToVmail</td>
</tr>
<tr>
<td colspan="3">Specific Number to Dial: 5000</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<th rowspan="4">3.b.</th>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><span style="color: Cyan;">Link activities together</th></span>
</tr>
<tr>
<td><ul>
<li><p>NewPhoneContact Activity</p>
<ul>
<li><p>Output –&gt; Business Hours</p></li>
</ul></li>
<li><p>Business Hours Activity</p>
<ul>
<li><p>Holidays –&gt; ToVmail</p></li>
</ul></li>
</ul></th>
</tr>
<tr>
<th>Validate and Publish flow using Latest Version</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

# Lab 6 – Channels and Testing Voice

In this lab, you will learn how to connect calls to the flow and to
receive a call on an Agent Desktop.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Channels</th></span>
</tr>
<tr>
<td><p>In order for agents to receive calls, entry points need to be
created to connect incoming calls to the appropriate flows</p>
<p>Create Multiple Channel Entry Points</p>
<p>Entry Point 1</p>
<ul>
<li><p>Name: Main Number</p>
<ul>
<li><p>Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Company FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later!)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Channels</td></span>
</tr>
<tr>
<td><p>Entry Point 2</p>
<ul>
<li><p>Name: Overseas Number</p>
<ul>
<li><p>Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Overseas FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; Customer Experience-&gt; Channels</td></span>
</tr>
<tr>
<td><p>Entry Point 3</p>
<ul>
<li><p>Name: Sales Number</p>
<ul>
<li><p>Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Sales FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td><span style="color: greenyellow;">Control Hub-&gt; Management-&gt; Users-&gt; Eric Steele</td></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Login as an agent to make a test call</p></span>
<ul>
<li><p>Copy email address for Eric Steele (Overseas Team)</p></li>
<li><p>Open new browser; NOT a new tab, a different browser</p>
<ul>
<li><p>Go to: <a
href="https://desktop.wxcc-us1.cisco.com/">https://desktop.wxcc-us1.cisco.com/</a></p></li>
<li><p>Login as Eric</p>
<ul>
<li><p>Password is the same as Charles Holland (admin account)</p></li>
</ul></li>
<li><p>Use Desktop for Audio / Calls</p></li>
</ul></li>
<li><p>Call the appropriate phone numbers you select above from your
cell or other phone</p></li>
<li><p>Answer the call as Eric in the browser. (Make sure to mute!)</p>
<p>Using the same steps, login as agents on other teams as desired to
test flows</p></li>
</ul></td>
</tr>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>













# Lab 7 – Chat Flow Pre-Work

In this lab, you will learn how to create a Chat Queue, Asset and Entry
Point / Channel

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Contact Center-&gt; Overview-&gt; Webex Connect-&gt; Assets-&gt;
Integrations</th>
</tr>
<tr>
<th><p>Customer needs Digital channel integration enabled</p>
<p>Authorize Webex CC Tasks and Webex CC Engage</p>
<ul>
<li><p>Webex CC Tasks: Manage</p>
<ul>
<li><p>Add Authentication: Cholland email</p></li>
<li><p>Sign in as Cholland in the popup window</p></li>
</ul></li>
<li><p>Webex CC Engage: Manage</p>
<ul>
<li><p>Add Authentication: Cholland email</p></li>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Contact Center-&gt; Overview-&gt; Webex Connect-&gt; Assets-&gt;
Apps</td>
</tr>
<tr>
<td><p>Customer needs an ability to route chats.</p>
<p>Create a Chat Asset</p>
<ul>
<li><p>New App: Mobile/Web</p></li>
<li><p>Name: Chat_Asset</p></li>
<li><p>Live Chat/ In-App Messaging: enable</p></li>
<li><p>Primary Protocol: MQTT</p></li>
<li><p>Secondary Protocol: Web Socket</p></li>
<li><p>Use a Secure Port: Tick</p>
<p>Once Saved</p></li>
</ul>
<ul>
<li><p>Register to Webex Engage: My First Service</p>
<p>On Apps main Page: Copy and Save App ID</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Contact Center-&gt; Customer Experience -&gt; Queues</td>
</tr>
<tr>
<td><p>Customer wants a queue created</p>
<p>Create a queue</p>
<ul>
<li><p>Queue Name: Chat Q</p></li>
<li><p>Channel Type: Chat</p></li>
<li><p>Routing Type: Longest Available Agent</p></li>
<li><p>Call Distribution:</p>
<ul>
<li><p>Priority 1 – Company, Overseas and Sales teams</p></li>
</ul></li>
<li><p>Service Level Threshold: 7200</p></li>
<li><p>Max time in Queue: 80100</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td>Contact Center-&gt; Customer Experience -&gt; Channels</td>
</tr>
<tr>
<td><p>Customer wants to receive chats into the Contact Center</p>
<p>Create a Channel Entry Point</p>
<ul>
<li><p>Name: Chat Entry</p></li>
<li><p>Type: Chat</p></li>
<li><p>Asset Name: Chat_Asset</p></li>
<li><p>Service Level: 7200</p></li>
<li><p>Timezone: NewYork</p></li>
</ul></td>
</tr>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

# Lab 8 – Chat Flow Creation and Testing

In this lab, you will learn how to connect chats to a flow and to
receive a chat on an Agent Desktop

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Contact Center-&gt; Overview-&gt; Webex Engage-&gt; Assets-&gt;
Channel Assets-&gt;Websites</th>
</tr>
<tr>
<th><p>Customer wants to make the chat template look good</p>
<p>Edit the Chat Asset</p>
<ul>
<li><p>Add Website</p></li>
<li><p>Display Name: Global Support Solutions</p></li>
<li><p>Byline Text: This is the future!</p></li>
<li><p>Greeting message: Please Click to initiate a Chat with
us</p></li>
<li><p>First Message: Welcome to the chat!</p></li>
<li><p>PCI Compliance Message: All Chats are stored and reviewed as
needed.</p></li>
<li><p>Domain: <a
href="http://www.w3schools.com">www.w3schools.com</a></p></li>
<li><p>Save</p></li>
<li><p>Edit the Appearance</p></li>
<li><p>Change Color and Widget button to your taste</p></li>
<li><p>Save</p></li>
<li><p>Edit Widget Visibility</p></li>
<li><p>Show without restrictions</p></li>
<li><p>Save</p></li>
<li><p>Select Installation</p></li>
<li><p>Copy then save installation code</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Contact Center-&gt; Overview-&gt; Webex Connect-&gt; My First
Service-&gt; Flows</td>
</tr>
<tr>
<td><p>Customer wants to receive chats into the Contact Center</p>
<p>Create a new Chat Flow</p>
<ul>
<li><p>Flow Name: Chat inbound</p></li>
<li><p>Upload: LiveChatInboundFlowWithoutForm</p></li>
<li><p>Save the Configure APP Event</p></li>
<li><p>Resolve Conversation node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Add Flow ID: All numbers at the end of URL in your tab, after the
equals sign</p></li>
<li><p>Save</p></li>
<li><p>Queue Task node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Queue Name: Chat Q</p></li>
<li><p>Save</p></li>
<li><p>Close Task node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Save</p></li>
<li><p>Setting Gear Icon:</p></li>
<li><p>General: Disable descriptive logs</p></li>
<li><p>Select: Custom Variables</p></li>
<li><p>Live Chat Domian: <a
href="http://www.w3schools.com">www.w3schools.com</a></p></li>
<li><p>AppID: Chat Asset ID Copied and Saved earlier</p></li>
<li><p>Make Live</p>
<p>Application: Chat_Asset</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Control Hub-&gt; Management-&gt; Users</td>
</tr>
<tr>
<td><p>Agent needs login credentials to receive chats</p>
<p>Copy details to use</p>
<ul>
<li><p>Name: Eric Steele (Overseas Team)</p></li>
<li><p>Copy email Address</p></li>
<li><p>Open new browser (not a new tab but a different browser)</p></li>
<li><p>Got to: <a
href="https://desktop.wxcc-us1.cisco.com/">https://desktop.wxcc-us1.cisco.com/</a></p></li>
<li><p>Login as Eric, Password is the same as Charles Holland</p></li>
<li><p>Use Desktop for Audio / Calls</p>
<p>You can test any agent in the same manner as you require.</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td>New Tab in Browser-&gt; www.w3schools.com</td>
</tr>
<tr>
<td><p>We need a way of simulating the customer website</p>
<p>HTML – Try it Yourself</p>
<ul>
<li><p>Paste copied installation code between &lt;p&gt;This is a
paragraph.&lt;/p&gt; and &lt;/body&gt;.</p></li>
<li><p>Run the code</p></li>
<li><p>Start and new Conversation with your logged in Agent</p></li>
</ul></td>
</tr>
</tbody>
</table>
<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

Congratulations!

You have completed:

LAB-1307

Your ultimate guide to Webex Contact Center​

