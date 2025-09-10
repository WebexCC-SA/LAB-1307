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
<td><span style="color: Cyan;"><p>Use Case: Each queue needs a specific flow to tailor the customer
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
<td colspan="2"><span style="color: Cyan;">Task: Link the activities together</p></span>
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
<td colspan="2"><span style="color: Cyan;">Task: Link activities together</th></span>
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
<td><span style="color: Cyan;">Task: Link activities together</th></span>
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