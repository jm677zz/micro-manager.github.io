---
autogenerated: true
title: PriorNano
layout: page
---

## Prior NanoScanZ and Prior Queensgate NanoScan adapter

<table>
<tr>
<td markdown="1">

**Summary:**

</td>
<td markdown="1">

Interfaces to Prior nanopositioning stages through Prior NanoScanZ and
Prior Queensgate NanoScan controllers

</td>
</tr>
<tr>
<td markdown="1">

**Author:**

</td>
<td markdown="1">

Nenad Amodaj and Graham Bartlett

</td>
</tr>
<tr>
<td markdown="1">

**License:**

</td>
<td markdown="1">

BSD

</td>
</tr>
<tr>
<td markdown="1">

**Platforms:**

</td>
<td markdown="1">

Windows, Mac OS X, Linux (serial port)

</td>
</tr>
<tr>
<td markdown="1">

**Devices:**

</td>
<td markdown="1">

NanoZStage

</td>
</tr>
<tr>
<td markdown="1">

**Example Config File:**

</td>
<td markdown="1">
</td>
</tr>
<tr>
<td markdown="1" valign=top>

**Default serial port settings:**

</td>
<td markdown="1" valign=top>

|                     |      |
|---------------------|------|
| AnswerTimeout       | 500  |
| BaudRate            | 9600 |
| DelayBetweenCharsMs | 0    |
| Handshaking         | Off  |
| Parity              | None |
| StopBits            | 1    |

</table>

This adapter interfaces with nanopositioning stages through the Prior
NanoScanZ or Prior Queensgate NanoScan controllers. It communicates with
the controller through the serial port so that no further software is
needed. It works with Prior/Queensgate nanopositioning Z stages. No
'hub' device is defined in this adapter.

--[GrahamBartlettPrior](User:GrahamBartlettPrior "wikilink") 13:14, 17
Oct 2019 (GMT)

{% include Devices_Sidebar text="" %}