---
autogenerated: true
title: GenericSLM
layout: page
---

<table>
<tr>
<td markdown="1">

**Summary:**

</td>
<td markdown="1">

Generic Spatial Light Modulator controller

</td>
</tr>
<tr>
<td markdown="1">

**Author:**

</td>
<td markdown="1">

Arthur Edelstein, Mark Tsuchida

</td>
</tr>
<tr>
<td markdown="1">

**License:**

</td>
<td markdown="1">

LGPL

</td>
</tr>
<tr>
<td markdown="1">

**Platforms:**

</td>
<td markdown="1">

Windows

</td>
</tr>
<tr>
<td markdown="1">

**Since Version:**

</td>
<td markdown="1">

1.3.42

</td>
</tr>
</table>

The GenericSLM device adapter controls any spatial light modulator that
can be driven by a computer digital video output port (typically DVI,
HDMI, or DisplayPort). Some graphics cards have a secondary video output
port; other computers will require an additional graphics card to be
installed.

In the Hardware Configuration Wizard, you will be presented with
available "Display Ports" in the GraphicsPort property of the
GenericSLM. You may need to experiment to identify the correct display
port connected to your SLM device (all monitors except for the primary
one appear as options). The numbering in names like "\\\\.\\DISPLAY1",
"\\\\.\\DISPLAY2", etc., does not necessarily match the monitor numbers
shown in the Screen Resolution control panel.

The TestMode option of the GraphicsPort property allows testing and
demonstration. This mode differs from using a real display (SLM) in the
following ways: (1) the display configuration is not changed, (2) a
window is displayed on the primary monitor instead of an SLM, and (3)
the window has a title bar so that you can move it.

When the device is loaded, the chosen monitor (SLM) will be detached
from the desktop, then reattached to the right of all other monitors.
When the device is unloaded, the monitor will be left detached. You can
observe these effects in the Screen Resolution control panel, should you
need to troubleshoot.

Because the SLM is attached to the desktop while in use, some care needs
to be taken so as not to drag ordinary windows into the region projected
onto the SLM. There is some protection (a floating window is used to
draw patterns, the mouse cursor is prevented from entering it, and the
mouse cursor is set invisible should it enter it), but it is not perfect
(you can drag other floating windows over the SLM window, the mouse
cursor may be able to enter the SLM window momentarily, and there may be
a short delay before the cursor turns invisible).

Use the Projector plugin to control the SLM.

**Supported Devices**

SLMs that can be driven by video output ports (and in principle by this
device adapter) include (no endorsements are implied):

-   Liquid-crystal arrays (those supporting DVI or VGA input) from
    [Meadowlark (they bought Boulder Nonlinear
    Systems)](http://www.meadowlark.com/xy-spatial-light-modulator-p-119),
    [Cambridge
    Correlators](http://www.cambridgecorrelators.com/products.html),
    [Hamamatsu](http://www.hamamatsu.com/us/en/product/category/3200/4015/index.html)
    and
    [Holoeye](http://www.holoeye.com/spatial_light_modulators-technology.html)
-   A [Digital Mirror
    Device](http://en.wikipedia.org/wiki/Digital_micromirror_device)
    (DMD) from Texas Instruments, using Digital Light Innovations'
    [DLP4100](http://www.dlinnovations.com/products/d4100.html) digital
    mirror controller kit with the
    [D2D](http://www.dlinnovations.com/products/D2D.html) (DVI to DMD)
    interface card),
-   A DMD-based [DLP
    LightCommander](http://www.ti.com/DLPLightCommander) from TI.
-   Almost any digital video projector (a.k.a. a computer projector)

{% include Devices_Sidebar text="" %}