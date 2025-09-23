In this lab, you will learn how to connect calls to the flow and to
receive a call on an Agent Desktop.

URL: [admin.webex.com](http://admin.webex.com/){:target="_blank"} Login: Instructor
provided credentials

[Click here to see the presentation](./Lab6.html){:target="_blank"}

Instructions:

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Channels</th></span>
</tr>
<tr>
<td><span style="color:#FF0099;"><p>Use Case: In order for agents to receive calls, entry points need to be
created to connect incoming calls to the appropriate flows</p></span>
<p>Create Multiple Channel Entry Points</p>
<p>Entry Point 1</p>
<ul>
<li><p>Name: Main Number</p>
<ul>
<li><p>Channel Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Company FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Webex Calling Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later!)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/article/2dputx/Set-up-voice-channels-for-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Channels</th></span>
</tr>
<tr>
<td><p>Entry Point 2</p>
<ul>
<li><p>Name: Overseas Number</p>
<ul>
<li><p>Channel Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Overseas FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Webex Calling Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/article/2dputx/Set-up-voice-channels-for-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Channels</th></span>
</tr>
<tr>
<td><p>Entry Point 3</p>
<ul>
<li><p>Name: Sales Number</p>
<ul>
<li><p>Channel Type: Inbound Telephony</p></li>
<li><p>Service Level: 120</p></li>
<li><p>Timezone: NewYork</p></li>
<li><p>Routing Flow: Sales FLow</p></li>
<li><p>Version Label: Latest</p></li>
<li><p>Music On Hold: Default Music on Hold.wav</p></li>
<li><p>Support Number:</p>
<ul>
<li><p>Webex Calling Location: dCloud</p></li>
<li><p>Number: Any (Make a note of this number for later)</p></li>
<li><p>PSTN Region Default</p></li>
</ul></li>
<a href="https://help.webex.com/en-us/article/2dputx/Set-up-voice-channels-for-Webex-Contact-Center" target="_blank">Help Page</a>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<th><span style="color:#00CC66;">Control Hub-&gt; Management-&gt; Users-&gt; Eric Steele</th></span>
</tr>
<tr>
<td><span style="color:#FF0099;"><p>Use Case: Login as an agent to make a test call</p></span>
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
<li><p>Handle Calls using: Desktop</p></li>
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

<center><span style="color: Red;"><strong>END OF LAB</strong></span></center>