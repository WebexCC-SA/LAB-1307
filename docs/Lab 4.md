In this lab, you will learn how to create Queues and Business Hours.

URL: [admin.webex.com](http://admin.webex.com/){:target="_blank"} Login: Instructor
provided credentials

[Click here to see the presentation](./Lab4.html){:target="_blank"}

Instructions:

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 47%" />
<col style="width: 47%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Customer Experience -&gt; Business
Hours</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Agents should only be reached through queues during
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
<li><p>Date range: Today’s date - 12/25/2025</p></li>
<li><p>Do NOT enable</p></li>
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
<li><p><em>Reminder: If a setting is not listed in the task instructions,
leave default settings or skip</em></p></li>
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
<a href="https://help.webex.com/en-us/article/dqekw4/Set-up-business-hours-for-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3">2.</td>
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Customer Experience -&gt;
Queues</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;"><p>Use Case: Separate queues are needed for Support and Sales to
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
<li><p>Call Distribution: Create Group</p>
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
<a href="https://help.webex.com/en-us/article/np2fdx/Understand-Routing-and-Queueing-in-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></td>
<td><p>Queue Name: Sales Q</p>
<ul>
<li><p>Contact Routing Settings</p>
<ul>
<li><p>Agent Assignment: Teams</p></li>
<li><p>Call Distribution: Create Group</p></li>
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