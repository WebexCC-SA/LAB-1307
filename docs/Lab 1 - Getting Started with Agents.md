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
<td><span style="color: Cyan;"><p>Use Case: In addition to standard voice communications, agents will support customers using digital channels. </p></span>
<p>Assign Premium Agent licenses to all users </p>
<ul>
<li><p>License: Premium</p></li>
<li><p>Apply scope: Existing users, preserve licenses for existing
users.</p></li>
<li><p><em>Spot check any user to ensure they have a Premium Agent license</em></p></li>
<a href="https://help.webex.com/en-us/article/n3ijtao/Set-up-automatic-license-assignments-in-Control-Hub">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">2.</td>
<td><span style="color: greenyellow;">Management-&gt; Users<em>-&gt;</em> Anita Perez</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">Use Case: In addition to Premium Agent access, Anita Perez will need to monitor and coach agents and access reporting and analytics </span></p>
<p>Add Contact Center Supervisor to Anita Perez</p>
<ul>
<li><p>License: Premium Agent</p></li>
<li><p>Add Supervisor Role</p></li>
<a href="https://help.webex.com/en-us/article/9dmqgv/Edit-service-licenses-in-Control-Hub-for-individual-users">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Skill Definitions</span></td>
</tr>
<td><p><span style="color: Cyan;">Use Case: Customer inquiries must be routed to the most qualified agents</span></p>
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
<a href="https://help.webex.com/en-us/article/6rzxls/Manage-skill-definitions-in-Webex-Contact-Center">Help Page</a>
</ul></p></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; User Management-&gt; Skill Profiles,</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">Use Case: Each agent has a unique set of skills that helps determine how calls are routed to them</span></p>
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
<a href="https://help.webex.com/en-us/article/arzaac/Manage-skill-profile-in-Webex-Contact-Center">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">5.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; Desktop Experience-&gt; Multimedia Profiles</span></td>
</tr>
<tr>
<td><p><span style="color: Cyan;">Use Case: Agents should handle only one chat at a time to ensure prompt responses. </span></p>
<p>Create multimedia profile to be applied to agents</p>
<ul>
<li><p>Profile Name: Agent MMP</p></li>
<li><p>Type: Exclusive</p></li>
<li><p>Voice and Chat only selected</p></li>
<a href="https://help.webex.com/en-us/article/nje7dhdb/Manage-multimedia-profiles">Help Page</a>
</ul></td>
</tr>
</tbody>
</table>
<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>