# UPDATED JULY 30, 2024: ArduJimmy-Brushed-QuadX (with Flysky and Bluetooth Controller)
This rep is my first Arduino QuadX Using Mosfet IRL520n As Speed Controller (ESC) for Brushed 820 DC Motor
Discussion:
https://electronics.stackexchange.com/questions/682177/is-it-okay-using-irl520n-without-resistor-and-diode-for-diy-brushed-esc-dc-motor (by ArduJimmy)
<p>
  I will explains all in my Youtube Channel at: https://www.youtube.com/@ArduJimmy, including:
  <ul>
    <li>Components and part list</li>
    <li>Multiwii Firmware version (config.h setup)</li>
    <li>Wiring and Schematic Diagram</li>
    <li>Brushed ESC Calibration</li>
    <li>Do and Don'ts</li>
  </ul>
</p>

<h2>Please Subscribe and Share my Channel</h2>
<p>
  <a href="https://www.youtube.com/@ardujimmy target="_blank" title="Ardujimmy Channel on YOUTUBE">Ardujimmy Youtube Channel</a>
</p>
<h2>Connection to Bluetooth</h2>
<p>In this case, we use Multiwii 2.4 version firmware to connect our diy arduino quadcopter to smartphone. You can use HC-05 or HC-06 module.</p>
<p>To connect bluetooth HC-05/HC-06 with your smartphone, firstly, you must instal and use this android app: <a href="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/Android%20DRMS%20FLY.zip">DRMS(fly)</a></p>

<h2>BLUETOOTH MODULE WIRING</h2>
<ul>
  <li>Pin TX arduino board to RX module HC-5/06</li>
  <li>Pin RX arduino board to TX module HC-5/06</li>
  <li>Pin GND arduino board to GND module HC-5/06</li>
  <li>Pin VCC 5v arduino board (or VCC 5v of Step-up Converter Output PIN) to VCC module HC-5/06</li>
</ul>

<p>Dont forget to setup your HC module to 115200 baudrate</p>

<h2>Connection to FLysky Receiver</h2>
<p>Here's the 4 channel wiring for flysky receiver. In this case, I use Fs2a 4Ch AFHDS 2a Pwm Mini Receiver:</p>
<ul>
  <li>Channel 1 flysky module to pin D4 of Arduino Pro mini 328p 5v</li>
  <li>Channel 2 flysky module to pin D5 of Arduino Pro mini 328p 5v</li>
  <li>Channel 3 flysky module to pin D2 of Arduino Pro mini 328p 5v</li>
  <li>Channel 4 flysky module to pin D6 of Arduino Pro mini 328p 5v</li>
</ul>

<p>How To Do: https://www.youtube.com/watch?v=862kxcojHQ8 (Bluetooth Quadcopter)</p>

<h2>Components & Parts</h2>
<ul>
  <li>LiPO Battery 1s 40C 3.7v, weight:6 grams</li>
  <li>IRLZ44N, Si2302 or IRL520n (Logical Level Mosfet) / N-Fet (recommend: si2302)</li>
  <li>Capacitor: 100uf 16v/25v/50v</li>
  <li>4Ch FS2A Flysky Receiver</li>
  <li>Flysky FS-i6 TX or Blutooth Module HC-05 / HC-06 (baudrate:115200)</i>
  <li>Gyro Module: MPU6050 / GY-521</li>
  <li>720, 820 or 8520 Coreless DC Motors </li>
  <li>AMS1117 3.3v</li>
  <li>Step-up Converter, DC to DC 3.7v to 5v</li>
  <li>Mini QuadX Frame (Ice cream stick or using 3d printing (ABS material). See on: https://www.thingiverse.com/thing:6695655 (FREE)</li>
  <li>Arduino Promini 5v 328p</li>
  <li>Cables & Jumpers: AWG 28 Wire</li>
  <li>Male-Female Red Connectors</li>
  <li>Double Foam Tape</li>
  <li>Propellers: 65mm/Dia.1mm or 75mm/Dia.1mm</li>
  <li>Resistor: 10K dan 100 Ohm + Diode in5819 (or equivalent)</li>
</ul>
<p>Note: 48 grams (All components and parts above)</p>

<h2>Firmware & Softwares Needed</h2>
<ul>
  <li>Firmware: Multiwii 2.3</li>
  <li>MultiwiiConf 32bit Under Windows</li>
  <li>Windows 7 32bit with Arduino IDE version: 1.8.19</li>
</ul>
<p>
Demo: https://www.youtube.com/watch?v=p6tdkUCIFxc (flying test III)
</p>

<p><img src="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/si2302%20mosfet.jpeg"/></p>

<h2>Schematic Diagram</h2>
<p>
  <img src="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/diy-brushed-esc.png"/>
</p>
<p>
  <img src="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/1.png"/>
</p>

<p>
  <img src="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/wiring-brushed-drone-by-ardujimmy.png" alt="working brushed ESC"/>
</p>
  <p><img src="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky/blob/main/motors-wiring.png" alt="motors wiring"/></p>
<h2>Source:</h2>
<ul>
  <li>http://www.multiwii.com/wiki/index.php?title=ESC_Calibration</li>
  <li>https://www.youtube.com/@ArduJimmy</li>
  <li>https://electronics.stackexchange.com/questions/682177/is-it-okay-using-irl520n-without-resistor-and-diode-for-diy-brushed-esc-dc-motor (by ArduJimmy)</li>
</ul>
