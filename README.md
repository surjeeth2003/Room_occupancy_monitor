# Room_occupancy_monitor
<!-- Doc 2 is in language en-US. Optimizing Doc 2 for scanning, using lists and bold where appropriate, but keeping language en-US, and adding id attributes to every HTML element: -->
<h2 id="qyc7g2k">Room Occupancy Monitor</h2>
<h3 id="nd0l4yr">Project Overview</h3>
<p id="wrhtlk">This project is an embedded system for monitoring room occupancy using STM32, ultrasonic sensors, and a 3-digit 7-segment display. It tracks people entering and exiting a room, counts the number of occupants, and displays the count in real-time.</p>
<h3 id="nog4cb">Features</h3>
<ul id="m5uibwo">
  <li id="coghnc"><strong id="im7ebns">Occupant Count</strong>: Tracks entry and exit sequences using two ultrasonic sensors.</li>
  <li id="2uwswt"><strong id="f65k39">Threshold Alert</strong>: An LED indicator lights up when the maximum room capacity is reached.</li>
  <li id="gotuupi"><strong id="q1tot2">Remote Monitoring</strong> <em id="2o7zoc">(optional)</em>: Transmits data via Bluetooth for remote display on a mobile device.</li>
</ul>
<h3 id="11gvipi">Components</h3>
<ul id="s92ewia">
  <li id="orusgwg"><strong id="36tgh3a">Microcontroller</strong>: STM32</li>
  <li id="mk7kapd"><strong id="mgy6xfv">Sensors</strong>: 2x Ultrasonic sensors (HC-SR04)</li>
  <li id="d1csvy"><strong id="n7vejgl">Display</strong>: 3-digit 7-segment display</li>
  <li id="7c69p1u"><strong id="nhs4kj5">Communication</strong>: Bluetooth module (HC-05) for remote monitoring</li>
  <li id="t33pl5"><strong id="r86iswc">Other</strong>: Breadboard, resistors, wiring, LED</li>
</ul>
<h3 id="oa59ptn">Project Structure</h3>
<ul id="ia9ogh">
  <li id="zfk4t9h"><strong id="eoz53dp">/src</strong>: Contains source code files (e.g., main program, sensor handling, and display updates)</li>
  <li id="vew4rtc"><strong id="1vjwinf">/include</strong>: Header files for modular functions</li>
  <li id="8di4qwg"><strong id="rewgoy">/docs</strong>: Any documentation or circuit diagrams for the project</li>
  <li id="yvk3k3q"><strong id="r38nrzc">README.md</strong>: Overview and instructions for the project</li>
</ul>
<h3 id="qm3xbi9">Circuit Diagram</h3>
<p id="gtl3vcn">Provide a simple circuit diagram here or link to one in the <code id="icyfolb">/docs</code> folder. This should show how the STM32, sensors, display, and LED are connected.</p>
<h3 id="8d2o6ad">How to Use</h3>
<ol id="dpm0eq">
  <li id="ee79ema"><strong id="6dokgua">Setup</strong>: Connect the STM32 to the sensors, display, and LED as per the circuit diagram.</li>
  <li id="0h76l0b"><strong id="31qetk">Run</strong>: Upload the code to the STM32 board using the Keil5 environment.</li>
  <li id="fvt9b5b"><strong id="8gm6xf">Observe</strong>: Check the 7-segment display for real-time room occupancy count.</li>
  <li id="63p1j4wb"><strong id="mz8vajd">Monitor Remotely (optional)</strong>: Use a Bluetooth-enabled device to receive real-time data from the STM32 board.</li>
</ol>
<h3 id="ov6m0k">Code Overview</h3>
<ul id="5ofitx">
  <li id="uofq5jp"><strong id="ytxeqcb">main.c</strong>: Initializes the system and contains the main control logic.</li>
  <li id="1wm3c8"><strong id="7zv1oyr">sensor.c</strong>: Manages sensor readings to detect entry and exit.</li>
  <li id="swnjn4j"><strong id="g4fg26c">display.c</strong>: Controls the 3-digit 7-segment display for showing the occupancy count.</li>
  <li id="w5w9s2m"><strong id="m651sul">bluetooth.c</strong>: (Optional) Handles Bluetooth communication for remote monitoring.</li>
</ul>
<div id="ljn4zyq">
  <h3 id="r84tiuki">Requirements</h3>
  <ul id="gjmim7h">
    <li id="y340ko"><strong id="v9q19i">STM32 Development Board</strong></li>
    <li id="dm6sjxm"><strong id="h1g3p7g">Keil5 IDE</strong> for code development and flashing</li>
  </ul>
  <h3 id="doknrr4">Future Improvements</h3>
  <ul id="qmyq0m7">
    <li id="2b1amw"><strong id="kfvpo9b">Wi-Fi Monitoring</strong>: Add Wi-Fi capability for monitoring via a web interface.</li>
    <li id="0sm0icc"><strong id="tzphnux">Data Logging</strong>: Store occupancy data for analytics on usage patterns.</li>
    <li id="3o7dk8c"><strong id="vss04h">Threshold Customization</strong>: Allow dynamic adjustment of room capacity limits.</li>
  </ul>
</div>
