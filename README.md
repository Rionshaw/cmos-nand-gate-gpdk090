# cmos-nand-gate-gpdk090
End-to-end CMOS NAND gate design in gpdk090 including layout, physical verification (DRC/LVS), and functional simulation in Cadence Virtuoso
<h2>Objectives</h2>

<ul>
  <li>Design a 2-input CMOS NAND gate using</li>
  <li>Implement schematic and layout</li>
  <li>Perform physical verification -
    <ul>
      <li>Design Rule Check (DRC)</li>
      <li>Layout vs Schematic (LVS)</li>
    </ul>
  </li>
  <li>Analyze transient response to verify correct NAND logic operation</li>
</ul>

<h2>Tools and Technology</h2>

<ul>
  <li>Cadence Virtuoso (Schematic Editor, Layout Suite)</li>
  <li>ADE L (Analog Design Environment)</li>
  <li>Technology Library - gpdk090</li>
</ul>


<h2>Circuit Description</h2>

<p>The CMOS NAND gate is implemented using complementary MOS transistors -</p>

<ul>
  <li><b>Pull-up network (PUN) -</b> Two PMOS transistors connected in parallel</li>
  <li><b>Pull-down network (PDN) -</b> Two NMOS transistors connected in series</li>
</ul>

<p><b>Operation -</b></p>

<ul>
  <li>Output is LOW only when both inputs are HIGH</li>
  <li>Output is HIGH for all other input combinations</li>
</ul>

<p>
This configuration ensures correct NAND logic functionality with low static power consumption.
</p>

<h3>Thuth Table</h3>

<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>A</th>
    <th>B</th>
    <th>Y = NAND(A,B)</th>
  </tr>
  <tr>
    <td>0</td>
    <td>0</td>
    <td>1</td>
  </tr>
  <tr>
    <td>0</td>
    <td>1</td>
    <td>1</td>
  </tr>
  <tr>
    <td>1</td>
    <td>0</td>
    <td>1</td>
  </tr>
  <tr>
    <td>1</td>
    <td>1</td>
    <td>0</td>
  </tr>
</table>

<h2>Schematic</h2>

<img src="https://github.com/Rionshaw/cmos-inverter-gpdk090/blob/bf3653e3debf6f5d914466718e5231e553d66ca0/Screenshot-9.png" alt="Schematic of NAND gate">
