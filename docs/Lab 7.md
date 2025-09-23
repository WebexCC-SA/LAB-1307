In this lab, you will learn how to create a Chat Queue, Asset and Entry
Point / Channel

URL: [admin.webex.com](http://admin.webex.com/){:target="_blank"} Login: Instructor
provided credentials

[Click here to see the presentation](./Lab7.html){:target="_blank"}

Instructions:

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th><span style="color:#00CC66;">Contact Center-&gt; Overview-&gt; Webex Connect-&gt; Assets-&gt;
Integrations</th></span>
</tr>
<tr>
<td><span style="color:#FF0099;"><p>Use Case: Customer needs Digital channel integration enabled</p></span>
<p>Authorize Webex CC Tasks and Webex CC Engage</p>
<ul>
<li><p>Webex CC Tasks: Manage</p>
<ul>
<ul>
<li><p>Actions: Manage</p>
<ul>
<li><p>Add Authentication: Cholland email</p></li>
<li><p>Sign in as Cholland in the popup window</p></li>
</ul></li>
</ul>
<li><p>Webex CC Engage: Manage</p>
<ul>
<li><p>Add Authentication: Cholland email</p></li>
</ul></li>
<a href="https://help.webexconnect.io/docs/wxcc-node-palette#node-authorization" target="_blank">Help Page</a>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Overview-&gt; Webex Connect-&gt; Assets-&gt;
Apps</th></span>
</tr>
<tr>
<td><p><span style="color:#FF0099;">Use Case: Customer needs an ability to route chats.</p></span>
<p>Create a Chat Asset</p>
<ul>
<li><p>Configure New App: Mobile/Web</p></li>
<li><p>Name: Chat_Asset</p></li>
<li><p>Live Chat/ In-App Messaging: enable</p></li>
<li><p>Primary Protocol: MQTT</p></li>
<li><p>Secondary Protocol: Web Socket</p></li>
<li><p>Use a Secure Port: Enable</p>
</ul>
<p>Once Saved</p></li>
</ul>
<ul>
<li><p>Register to Webex Engage: My First Service</p></li>
<li><p>On Apps main Page: Copy and Save App ID</p></li>
<a href="https://help.webexconnect.io/docs/wxcc-channel-assset-configuration-wxcc" target="_blank">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience -&gt; Queues</th></span>
</tr>
<tr>
<td><p><span style="color:#FF0099;">Use Case: Customer wants a queue created</p></span>
<p>Create a queue</p>
<ul>
<li><p>Queue Name: Chat Q</p></li>
<li><p>Channel Type: Chat</p></li>
<li><p>Routing Type: Longest Available Agent</p></li>
<li><p>Chat Distribution:</p>
<ul>
<li><p>Priority 1 – Company, Overseas and Sales teams</p></li>
</ul></li>
<li><p>Service Level Threshold: 7200</p></li>
<li><p>Max time in Queue: 80100</p></li>
<a href="https://help.webex.com/en-us/article/np2fdx/Understand-Routing-and-Queueing-in-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience -&gt; Channels</th></span>
</tr>
<tr>
<td><p><span style="color:#FF0099;">Use Case: Customer wants to receive chats into the Contact Center</p></span>
<p>Create a Channel</p>
<ul>
<li><p>Name: Chat Entry</p></li>
<li><p>Channel Type: Chat</p></li>
<li><p>Asset Name: Chat_Asset</p></li>
<li><p>Service Level: 7200</p></li>
<li><p>Timezone: NewYork</p></li>
<a href="https://help.webex.com/en-us/article/n954r0k/Set-up-digital-channels-in-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></td>
</tr>
</tbody>
</table>

<center><span style="color: Red;"><strong>STOP</strong></span></center>
<figure markdown>
  ![ACI](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>