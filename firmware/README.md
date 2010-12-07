<p>Teensy teouchpad firmware
Fall 2010</p>

<p>Firmware for the Teensy touchpad device.
Tested on Debian GNU/Linux 5.0 Lenny with 2.6.24 kernel</p>

<h1>Firmware</h1>

<p>The firmware interacts with 4 teensy pins, specified in the next section, 
according to the touchscreen specs.</p>

<p>http://www.sparkfun.com/tutorials/139</p>

<h1>Hardware connections</h1>

<p>Pin Assignment:
<table>
  <tr>
  	<td>Teensy</td>
  	<td>Touchscreen</td>
  	<td>Values to get X Pos.</td>
  	<td>Values to get Y Pos.</td>
  </tr>
  <tr>
  	<td>F1</td>
  	<td>F4</td>
  	<td>F5</td>
  	<td>F6</td>
  </tr>
  <tr>
  	<td>X1</td>
  	<td>Y2</td>
  	<td>X2</td>
  	<td>Y1</td>
  </tr>
  <tr>
  	<td>5V</td>
  	<td>ADC</td>
  	<td>GND</td>
  	<td>floating</td>
  </tr>
  <tr>
  	<td>ADC</td>
  	<td>5V</td>
  	<td>floating</td>
  	<td>GND</td>
  </tr>

</table>

<p>A push button is connected to the teensy D0 pin, when pressed the firmware
send a left click to the driver.</p>