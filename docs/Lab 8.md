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
<td><span style="color: greenyellow;">Contact Center-&gt; Overview-&gt; Webex Engage-&gt; Assets-&gt;
Channel Assets-&gt;Websites</th></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Use Case: Customer wants to make the chat template look good</p></span>
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
<ul>
</ul>
<li><p>Edit the Appearance</p></li>
<li><p>Change Color and Widget button to your taste</p></li>
<li><p>Save</p></li>
<ul>
</ul>
<li><p>Edit Widget Visibility</p></li>
<li><p>Show without restrictions</p></li>
<li><p>Save</p></li>
<ul>
</ul>
<li><p>Select Installation</p></li>
<li><p>Copy then save installation code</p></li>
<a href="https://help.webex.com/en-us/article/otcepj/Webex-Engage-Admin-and-Setup-Guide">Help Page</a>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td><span style="color: greenyellow;">Contact Center-&gt; Overview-&gt; Webex Connect-&gt; My First
Service-&gt; Flows</td></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Use Case: Customer wants to receive chats into the Contact Center</p></span>
<p>Create a new Chat Flow</p>
<ul>
<li><p>Flow Name: Chat inbound</p></li>
<li><p>Upload: LiveChatInboundFlowWithoutForm</p></li>
<li><p>Save the Configure APP Event</p></li>
<ul>
</ul>
<li><p>Resolve Conversation node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Add Flow ID: All numbers at the end of URL in your tab, after the
equals sign</p></li>
<li><p>Save</p></li>
<ul>
</ul>
<li><p>Queue Task node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Queue Name: Chat Q</p></li>
<li><p>Save</p></li>
<ul>
</ul>
<li><p>Close Task node</p></li>
<li><p>Authorize with Cholland after screen fully loads</p></li>
<li><p>Save</p></li>
<ul>
</ul>
<li><p>Setting Gear Icon:</p></li>
<li><p>General: Disable descriptive logs</p></li>
<li><p>Select: Custom Variables</p></li>
<li><p>Live Chat Domian: <a
href="http://www.w3schools.com">www.w3schools.com</a></p></li>
<li><p>AppID: Chat Asset ID Copied and Saved earlier</p></li>
<ul>
</ul>
<li><p>Make Live</p></li>
<li><p>Application: Chat_Asset</p></li>
<a href="https://help.webexconnect.io/docs/flows">Help Page</a>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td><span style="color: greenyellow;">Control Hub-&gt; Management-&gt; Users</td></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Use Case: Agent needs login credentials to receive chats</p></span>
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
<td><span style="color: greenyellow;">New Tab in Browser-&gt; www.w3schools.com</td></span>
</tr>
<tr>
<td><span style="color: Cyan;"><p>Use Case: We need a way of simulating the customer website</p></span>
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
  ![Stop](./assets/Stop.png)
</figure>

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>

