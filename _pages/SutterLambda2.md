---
autogenerated: true
title: SutterLambda2
layout: page
---

<table>
<thead>
<tr class="header">
<th><p>Summary:</p></th>
<th><p>Interfaces to Sutter Lambda 10-3 controller</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Authors:</p></td>
<td><p>Nick Anthony. Based off of the <a href="SutterLambda" title="wikilink">SutterLambda</a> adapter</p></td>
</tr>
<tr class="even">
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p>License:</p></td>
<td><p>BSD</p></td>
</tr>
<tr class="even">
<td><p>Platforms:</p></td>
<td><p>Windows, Mac OS X and Linux (only serial port, no parallel port or USB)</p></td>
</tr>
<tr class="odd">
<td><p>Devices:</p></td>
<td><p><a href="http://sutter.com/IMAGING/lambda103.html">Lambda 10-3</a><br />
</p></td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------

## Device Configuration

### Serial port issues

The Lambda 10-3 Controller uses a straight through (i.e., not null
modem) DB9 serial cable. The default baud rates are 9600 for serial
ports and 128000 for USB ports (which use a build-in USB-serial
converter, drivers can be found
[here](http://www.sutter.com/SOFTWARE/imaging.html))

### Wheel speed

95% of the time speed `#1` works best (`#0` being the fastest, which
only works with an empty wheel). If speed `#1` does not work you can try
the slowest (speed `#7` IIRC). Best practice is to [set the desired
wheel speed during
startup](Micro-Manager_Configuration_Guide#Startup_Presets "wikilink"),
i.e. in your `Startup` Preset of the `System` Group.

### Lambda VF5

The Lambda VF5 tunable filter changer consists of a filter wheel which
can additionally be tilted to provide a specific bandpass wavelength. In
addition to selecting a wheel speed (described above) you can also
select a tilt speed between 0 and 3.

{% include Devices_Sidebar text="" %}