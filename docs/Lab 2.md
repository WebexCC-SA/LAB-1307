In this lab, you will learn how to create Sites, Teams, Desktop Layouts,
Address Books and Auxiliary Codes.

URL: [admin.webex.com](http://admin.webex.com/){:target="_blank"} Login: Instructor
provided credentials

[Click here to see the presentation](./Lab2.html){:target="_blank"}

Instructions:

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 47%" />
<col style="width: 47%" />
</colgroup>
<thead>
<tr>
<td rowspan="2">1.</td>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; User Management-&gt; Sites</span></th>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Supervisors and admins require a straightforward
reporting solution for individual locations</p></span>
<ul>
<p>Create a site</p>
<ul>
<li><p>Name: Company HQ</p></li>
<li><p>MultiMedia Profile: Agent MMP</p></li>
<a href="https://help.webex.com/en-us/article/nqipixt/Manage-sites-in-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></td>
</tr>
<td>
<tr>
<td rowspan="3">2.</td>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; User Management-&gt; Teams</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Supervisors and admins need to easily manage and
streamline queue assignments for groups of agents.</p></span>
<p>Create Teams for use in queues</p>
<tr>
<td><ul>
<li><p>Name: Company Team</p></li>
<ul>
<li><p>Parent Site: Company HQ</p></li>
<li><p>Team Type: Agent Based</p></li>
</ul></li>
<li><p>Name: Overseas Team</p></li>
<ul>
<li><p>Parent Site: Company HQ</p></li>
<li><p>Team Type: Agent Based</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/article/mqf72s/Manage-teams-in-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></th>
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
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Desktop Experience-&gt; Desktop
Layouts</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Agents need to use Webex on their desktops</p></span>
<p>Create a new desktop layout to use Webex</p>
<ul>
<li><p>Name: Company Layout</p>
<ul>
<li><p>Teams: Company, Overseas and Sales</p></li>
<li><p>JSON File: Download the default desktop layout</p>
<ul>
<li><p>Open the file with a text editor</p>
<li><p>Look for Agent:</p></li>
  <p>"DesktopChatApp" {</p></li>
  <p>"webexconfigured":</p></li>
<a href="https://webexcc-sa.github.io/LAB-1307/assets/Lab2/Json.jpeg" target="_blank">Reference Image</a>
  <li><p>Change false to true</p></li>
<li><p>Repeat for Supervisor (further down the file)</p></li>
</li>
<li><p>Save the file as CompanyDesktopLayout.json</p></li>
</ul>
<li><p>Replace file in the Desktop Layout</p></li>
</li>
<li><p>Make sure to click Create</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/article/60x9ji/Manage-desktop-layouts" target="_blank">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Desktop Experience-&gt; Address
Books</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Agents and supervisors need to easily call the local
numbers they call on a regular basis</p></span>
<p>Create an Address Book for agents to use</p>
<ul>
<li><p>Name: Company Address Book</p></li>
<li><p>Type: Site</p></li>
<li><p>Site: Company HQ</p></li>
<li><p>Entry List</p>
<ul>
<li><p>Name: Cisco TAC</p></li>
<li><p>Contact Number: 8005532447</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="3">5.</td>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Desktop Experience-&gt; Idle/Wrap-up
Codes</th><span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Outcomes for each customer/agent interaction need to
be categorized and tracked for reporting and analysis</p></span>
<p>Create codes for agent use after a call completes</p></td>
</tr>
<tr>
<td><p>Name: Support</p>
<ul>
<li><p>Make it default: enable</p></li>
<li><p>Code type: Default Wrap-up Work Type</p>
</ul>
<p>Name: Service</p></li>
<ul>
<li><p>Code type: Default Wrap-up Work Type</p></li>
</ul>
<a href="https://help.webex.com/en-us/">Help Page</a>
</ul></td>
<td><p>Name: Sales</p>
<ul>
<li><p>Code type: Default Wrap-up Work Type</p>
</ul>
<p>Name: Administration Time</p></li>
<ul>
<li><p>Make it default: enable</p></li>
<li><p>Code type: Default Idle Work Type</p>
</ul>
<p>Name: Break</p></li>
<ul>
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