Download Link: https://assignmentchef.com/product/solved-cpe526-homework2-combinational-modeling
<br>
Cryptographic applications commonly require circular shifts. Whereas these shifts can be accomplished using a shift register, combinational shifting is required to complete these operations in a reasonable amount of time. Design an 8 bit barrel shifter that has 8 data inputs and 8 data outputs, and 3 control inputs that determine the shift amount (0-7). An additional enable input controls whether the outputs are tri-state or not. Use the truth table below as the functionality and use the entity declaration given.




<strong>  en  s2  s1  s0       c7  c6  c5  c4  c3  c2  c1  c0  </strong>

<table width="474">

 <tbody>

  <tr>

   <td width="192">   0   0   0   0</td>

   <td width="282"> a7  a6  a5  a4  a3  a2  a1  a0</td>

  </tr>

  <tr>

   <td width="192">   0   0   0   1</td>

   <td width="282"> a0  a7  a6  a5  a4  a3  a2  a1</td>

  </tr>

  <tr>

   <td width="192">   0   0   1   0</td>

   <td width="282"> a1  a0  a7  a6  a5  a4  a3  a2</td>

  </tr>

  <tr>

   <td width="192">   0   0   1   1</td>

   <td width="282"> a2  a1  a0  a7  a6  a5  a4  a3</td>

  </tr>

  <tr>

   <td width="192">   0   1   0   0</td>

   <td width="282"> a3  a2  a1  a0  a7  a6  a5  a4</td>

  </tr>

  <tr>

   <td width="192">   0   1   0   1</td>

   <td width="282"> a4  a3  a2  a1  a0  a7  a6  a5</td>

  </tr>

  <tr>

   <td width="192">   0   1   1   0</td>

   <td width="282"> a5  a4  a3  a2  a1  a0  a7  a6</td>

  </tr>

  <tr>

   <td width="192">   0   1   1   1</td>

   <td width="282"> a6  a5  a4  a3  a2  a1  a0  a7</td>

  </tr>

  <tr>

   <td width="192">   1   0   0   0</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   0   0   1</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   0   1   0</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   0   1   1</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   1   0   0</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   1   0   1</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   1   1   0</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

  <tr>

   <td width="192">   1   1   1   1</td>

   <td width="282">  Z   Z   Z   Z  Z   Z   Z   Z</td>

  </tr>

 </tbody>

</table>




Use the following entity




<strong>entity </strong>barrel<strong> is </strong>

<strong>  port (</strong>a<strong> : in std_logic_vector (7 downto 0);          </strong>s<strong> : in std_logic (2 downto 0;        en : in std_logic; </strong>

<strong>        </strong>c<strong> : out std_logic_vector (7 downto 0)); end entity </strong>barrel<strong>; </strong>




Develop a behavioral architecture for the system.

Perform the following steps

<ol>

 <li>Modify the test bench given in homework #1 to test this circuit.</li>

 <li>Compile all of the files</li>

 <li>Simulate to verify correctness.</li>

</ol>

Turn in all VHDL files.