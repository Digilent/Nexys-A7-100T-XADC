Nexys A7-100T XADC Demo
==============
  
Description
--------------
This project is a Vivado demo using the Nexys A7-100T's analog-to-digital converter ciruitry, switches, LEDs, and seven-segment display, written in Verilog. When programmed onto the board, voltage levels between 0 and 1 Volt are read off of the JXADC header. The 16 User LEDs increment from right to left as the voltage difference between the selected channel's pins gets larger. The seven-segment display shows the voltage difference between the selected channel's pins in volts. SW0 and SW1 select which XADC channel is displayed, as shown in the table below. See the Nexys A7-100T's [Reference Manual](FIXME) for more information about how the Artix 7 FPGA's XADC is connected to header JXADC.

| XADC Channel | JXADC Pins             | SW0 Position | SW1 Position |
| ------------ | ---------------------- | ------------ | ------------ |
| AD3          | JXADC1(P) / JXADC7(N)  | Up           | Down         |
| AD10         | JXADC2(P) / JXADC8(N)  | Down         | Up           |
| AD2          | JXADC3(P) / JXADC9(N)  | Down         | Down         |
| AD11         | JXADC4(P) / JXADC10(N) | Up           | Up           |
  
Requirements
--------------
* **Nexys A7-100T**: To purchase a Nexys A7-100T, see the [Digilent Store](FIXME)
* **Vivado 2018.2 Installation**: To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **MicroUSB Cable**
* **Wires and a Circuit to Measure**

Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Nexys-A7-100T-XADC/releases).
2. Open the project in Vivado 2018.2 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Nexys-A7-100T-XADC.xpr".
3. In the Flow Navigator panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug the Nexys A7-100T into the computer using a MicroUSB cable.
5. In the green bar at the top of the window, click **Open target**. Select "Auto connect" from the drop down menu.
6. In the green bar at the top of the window, click **Program device**.
7. In the Program Device Wizard, enter "\<archive extracted location\>vivado_proj/Nexys-A7-100T-XADC.runs/impl_1/top.bit" into the "Bitstream file" field. Then click **Program**.
8. The demo will now be programmed onto the Nexys A7-100T. See the Introduction section of this README for a description of how this demo works.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project.

Check out the Nexys A7-100T's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start) to find more documentation, demos, and tutorials.

For technical support or questions, please post on the [Digilent Forum](https://forum.digilentinc.com).

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)


