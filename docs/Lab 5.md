In this lab, you will learn how to create flows for queues.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials

[Click here to see the presentation](./Lab5.html){:target="_blank"}

Instructions:

<table>
<colgroup>
<col style="width: 5%" />
<col style="width: 94%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.a.</th>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows-&gt; Manage Flows-&gt; Create Flows-&gt; Start Fresh</th></span>
</tr>
<tr>
<td><span style="color:#FF0099;"><p>Use Case: Each queue needs a specific flow to tailor the customer
experience and make sure inquiries are handled according to the team’s
processes</p></span>
<p>Flow Number 1</p>
<ul>
<li><p>Name: CompanyFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
<a href="https://help.webex.com/en-us/article/nhovcy4/Flow-Designer" target="_blank">Help Page</a>
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
<th rowspan="2"><span style="color:#FF9900;">Business Hours</th></span>
<td colspan="2">Activity Label: BusinessHours</td>
</tr>
<tr>
<td colspan="2">Static Business Hours: Work Week</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Message</th></span>
<td colspan="2">Activity Label: Welcome</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to Global Support Solutions</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Menu</th></span>
<td colspan="2">Activity Label: Menu1</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p>
<p>Text: For support, please press 1, for service please press
2</p></td>
<td><p>Make Prompt interruptible: Enable</p>
<p>Custom Menu Links:</p>
<p>Digit Number 1 = Support</p>
<p>Digit Number 2 = Service</p></td>
</tr>
<tr>
<th><span style="color:#FF9900;">Menu</th></span>
<td colspan="2">Activity Label: Menu2</td>
</tr>
<tr>
<td></td>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p>
<p>Text: For additions press 1, for moves press 2 and for configuration
press 3.</p></td>
<td><p>Make Prompt interruptible: Enable</p>
<p>Custom Menu Links:</p>
<p>Digit Number 1 = Adds</p>
<p>Digit Number 2 = Moves</p>
<p>Digit Number 3 = Changes</p></td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Blind Transfer</th></span>
<td colspan="2">Activity Label: ToVmail</td>
</tr>
<tr>
<td colspan="2">Specific Dial Number: 5000</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Queue Contact</th></span>
<td colspan="2">Activity Label: SupportQ</td>
</tr>
<tr>
<td><p>Static Queue: Support Q</p>
<p>Set Contact Priority:
Enable</p>
<p>Set Contact Priority: Value = 5</p></td>
<td><p>Add Static Skill: Support</p>
<p>Value: is True<p></td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Queue Contact</th></span>
<td colspan="2">Activity Label: AddQ</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td><p>Add Static Skill: Adds</p>
<p>Value: is True<p></td>
</tr>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Queue Contact</th></span>
<td colspan="2">Activity Label: MoveQ</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td><p>Add Static Skill: Moves</p>
<p>Value: is True<p></td>
</tr>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Queue Contact</th></span>
<td colspan="2">Activity Label: ChangesQ</td>
</tr>
<tr>
<td>Static Queue: Support Q</td>
<td><p>Add Static Skill: Changes</p>
<p>Value: >= 4<p></td>
</tr>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Music</th></span>
<td colspan="2">Activity Label: PlayMusic</td>
</tr>
<tr>
<td>Static Audio File: defaultmusic_on_hold_cisco_opus_no_1.wav</td>
<td><p>Start Offset = 0</p>
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
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;">Task: Link the activities together</p></span>
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
<td rowspan="2">2.a.</td>
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><p>Flow Number 2</p>
<ul>
<li><p>Name: OverseasFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
<a href="https://help.webex.com/en-us/article/nhovcy4/Flow-Designer" target="_blank">Help Page</a>
</ul></th>
</tr>
</thead>
<body>
</body>
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
<th rowspan="2"><span style="color:#FF9900;">Business Hours</th></span>
<td colspan="2">Activity Label: BusinessHours</td>
</tr>
<tr>
<td colspan="2">Static Business Hours: Work Week</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Message</th></span>
<td colspan="2">Activity Label: Welcome</td>
</tr>
<tr>
<td><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to the Global Support Solutions overseas department.
Please hold and we will be with you shortly.</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Blind Transfer</th></span>
<td colspan="2">Activity Label: ToVmail</td>
</tr>
<tr>
<td colspan="2">Specific Number to Dial: 5000</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Music</th></span>
<td colspan="2">Activity Label: PlayMusic</td>
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
<th colspan="2"><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td colspan="2"><span style="color:#FF0099;">Task: Link activities together</th></span>
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
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><p>Flow Number 3</p>
<ul>
<li><p>Name: SalesFlow</p></li>
<li><p>Add the following Activities to the canvas</p></li>
<li><p>Do NOT connect the Activities until instructed</p></li>
<a href="https://help.webex.com/en-us/article/nhovcy4/Flow-Designer" target="_blank">Help Page</a>
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
<th rowspan="2"><span style="color:#FF9900;">Business Hours</th></span>
<td colspan="3">Activity Label: BusinessHours</td>
</tr>
<tr>
<td colspan="3">Static Business Hours: Work Week</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Message</th></span>
<td colspan="3">Activity Label: Welcome</td>
</tr>
<tr>
<td colspan="2"><p>Audio: Enable TTS (Text To Speech)</p>
<p>Connector: Cisco Cloud Text-to-Speech</p></td>
<td>Text: Welcome to the Sales Department of Global Support Solutions.
We will be with you shortly</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Blind Transfer</th></span>
<td colspan="3">Activity Label: ToVmail</td>
</tr>
<tr>
<td colspan="3">Specific Number to Dial: 5000</td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Queue Contact</th></span>
<td colspan="3">Activity Label: SalesQ</td>
</tr>
<tr>
<td>Static Queue: Sales Q</td>
<td colspan="2"></td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Play Music</th></span>
<td colspan="3">Activity Label: PlayMusic</td>
</tr>
<tr>
<td colspan="2">Audio File:
defaultmusic_on_hold_cisco_opus_no_1.wav</td>
<td><p>Offset = 0</p>
<p>Music Duration: 3600</p></td>
</tr>
<tr>
<th rowspan="2"><span style="color:#FF9900;">Blind Transfer</th></span>
<td colspan="3">Activity Label: ToVmail</td>
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
<th><span style="color:#00CC66;">Contact Center-&gt; Customer Experience-&gt; Flows</th></span>
</tr>
<tr>
<td><span style="color:#FF0099;">Task: Link activities together</th></span>
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