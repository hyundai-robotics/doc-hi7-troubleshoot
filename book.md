
[__SOURCE](README.md)
# Hi7-N Controller Maintenance Manual – Troubleshooting

The controller is designed with primary emphasis on high precision and high-speed performance.
In the event of a malfunction, the system is structured to allow easy identification of the cause and rapid recovery. Please read and fully understand this manual to ensure effective and efficient troubleshooting.

## Troubleshooting Procedures

This section describes the troubleshooting procedures for each error code that may occur in the Hi7-N Controller.

[__SOURCE](0-about-this-manual/precautions.md)
# Precautions

{% include file="en/precautions.md" %}

[__SOURCE](1-elec/README.md)
# 1. Electrical equipment
[__SOURCE](1-elec/VOLTAGE_1.md)
## 1.1. Voltage Check 1 – Internal 3-Phase Voltage Test for Hi7-N Controller

(1) Verify the 3-phase power voltage inside the controller.

The Power Supply Module (PSM) mounted on the front of the controller is responsible for distributing and relaying various power sources. The 3-phase power is switched ON/OFF via a magnetic switch within the PSM. With the motor in the OFF state, check whether the input voltage to the PSM is within a 10% tolerance range based on AC 220V. If the measured voltage is outside the allowable range, perform the following inspections.

![](../_assets/1.전장/전압점검/전압점검1_en.PNG)<br>
Figure 1.1 3-phase power input to the PSM (Power Supply Module)


{% hint style="warning" %}
Warning
Exercise caution when measuring high voltage, as there is a risk of short circuits between phases or with surrounding components."
{% endhint %}

1)  Case where the controller nameplate voltage is 220V<br>
If the controller input voltage is 220V AC, the voltage input from the external power switch or terminal block must be identical to the voltage measured at the internal PSM (Power Supply Module). If there is a discrepancy, please inspect the 3-phase power wiring.

2)	Case where the controller nameplate voltage is NOT 220V<br>
If the controller input power is not a 220V AC specification, the 3-phase power is converted to 220V AC using an internal transformer and then connected to the PSM. Check whether the voltage measured at the PSM is within a 10% tolerance range based on 220V AC.
If the measured voltage is outside the allowable range, inspect the connection status of the input and output terminals of the internal transformer. The primary side of the internal transformer must be connected to the voltage indicated on the controller nameplate. The secondary side of the transformer is always set to 3-phase 220V AC.
If 3-phase 220V AC is not output correctly from the output terminal despite the input and output terminals being properly connected, the transformer is defective. In this case, the output voltage tolerance of the transformer must be within 5%.

[__SOURCE](1-elec/VOLTAGE_2.md)
## 1.2. Voltage Check 2 – Hi7-N Controller Input 3-Phase Voltage Inspection Procedure

(1) Verify the voltage on the controller nameplate and the actual input voltage.

Check whether the voltage actually supplied to the controller is within the allowable range of the voltage indicated on the nameplate. The allowable range for the input voltage is within 10% of the value marked on the nameplate and must be at least 198V AC based on a 220V AC standard.

The figure below illustrates the measurement method for the controller's input voltage. If the measured voltage is outside the allowable range, please inspect the power supply facilities.

*	Measurement at the power line side of the front switch

![](../_assets/1.전장/전압점검/전압점검2.PNG)<br>
(a) Hi7-N Conroller<br>
Figure 1.2 Measurement on the power line side of the power switch

{% hint style="warning" %}
Exercise caution when measuring high voltage, as there is a risk of short circuits between phases or with surrounding components.
{% endhint %}

[__SOURCE](1-elec/Parts_replacement_tips.md)
## 1.3. Replacement Procedures

This section describes the replacement procedures for each component and printed circuit board (PCB) during troubleshooting.

### 1. Module Replacement Procedures

{% hint style="warning" %}
Operators must keep the following precautions in mind when replacing modules.
{% endhint %}

① Ensure that the power supply is turned OFF before starting any work.</br>
② Keep your hands clean to prevent oil or moisture from getting onto the circuit boards. When you must handle a board, hold it by its edges. Be careful not to touch electronic components, conductive patterns, or especially the contact areas of the connectors.</br>
③ Ensure that the operator's body (hands) and the controller are at the same electrical potential (equipotential).</br>
④ Each circuit board has multiple connectors. During replacement, ensure they are inserted correctly to avoid incorrect insertion, omission, or loose connections. Align the connector labels with the names printed on the board before insertion.</br>

### 1.1. Main Module Replacement Procedures

{% hint style="warning" %}
Before removing the main module, be sure to take the following actions
{% endhint %}

① When replacing the main module, first back up all necessary programs and parameter data using the HR-VIEW S/W on a (Notebook) PC or a USB memory drive before proceeding with the replacement.</br>
② Since the taught programs and parameter data are stored in the RAM of the main module, the existing data will not be present once the board is replaced with a new one.</br>
③ After the replacement, you can use the system by loading the previously backed-up data onto the new board.</br>
Please adhere to the precautions above and follow the steps below to replace the circuit board.</br>

#### 1.1.1 Removing the Control Module

① First, disconnect the input power from the power supply unit.</br>
② Disconnect all connectors attached to the module. For connectors fastened with screws, use an appropriate screwdriver to loosen them, and remove the connectors carefully to avoid applying excessive force.</br>
③ Slightly loosen the top and bottom fixing screws, move the module upward, and then pull it out to remove it.</br>

#### 1.1.2 Installing the Control Module

① First, verify that the controller input power is in the OFF state.</br>
② Mount the replacement module by hooking it onto the top and bottom fixing screws, then tighten the screws to secure it.</br>
③ Reconnect all connectors to the module. For connectors fastened with screws, use an appropriate screwdriver to secure them, ensuring they are connected firmly without applying excessive force.</br>
④ Double-check that the communication cables are connected correctly and that no steps have been omitted.</br>

### 1.2. Drive Module Replacement Procedures

{% hint style="warning" %}
Operators must keep the following precautions in mind when replacing the servo drive module.
{% endhint %}

Be sure to check the nameplate on the front panel, as compatibility may vary between different models of servo drive modules.

#### 1.2.1 Removing the Servo Drive Unit
① First, turn OFF the input power to the power supply unit.</br>
② Loosen the fixing bolts on the protective cover of the servo drive unit and remove the cover.</br>
③ Disconnect the wiring secured by screws to the terminal block.</br>
④ Disconnect all connected connectors.</br>
⑤ Remove the screws securing the servo drive unit.</br>
⑥ Carefully take out the servo drive unit. The servo drive unit is heavy; use caution to avoid injury while removing it. </br>Also, be careful not to damage any adjacent wiring.

#### 1.2.2 Installing the Servo Drive Unit
① First, verify that the input power to the power supply unit is turned OFF.</br>
② Carefully lift and slide the servo drive unit into place. The unit is heavy; use caution to avoid injury during installation. Take care not to damage the surrounding wiring.</br>
③ Secure the servo drive unit with screws.</br>
④ Tighten the wiring onto the terminal block using the screws.</br>
⑤ Reconnect all the connectors.</br>
⑥ Fasten the protective cover of the servo drive unit with the bolts.</br>
⑦ Double-check to ensure that no steps have been omitted.</br>

### 1.3. Power Supply Module (PSM) Replacement Procedures 

{% hint style="warning" %} The PSM is a multi-power supply unit used as the main control power source. As it is a precision device, please handle it with extraordinary care. {% endhint %}

#### 1.3.1 Removing the Power Supply Module (PSM)
① First, turn OFF the input power to the power supply unit.</br>
② Disconnect all connectors attached to the module.</br>
③ Slightly loosen the top and bottom fixing screws, move the module upward, and then pull it out to remove it. The PSM is heavy; use caution to avoid injury while removing it. Take care not to damage any adjacent wiring. Additionally, be careful not to pull the module too suddenly or with excessive force, as this may cause injury.</br>

#### 1.3.2 Installing the Power Supply Module (PSM)
① First, verify that the controller input power is in the OFF state.</br>
② Mount the replacement module by hooking it onto the top and bottom fixing screws, then tighten the screws to secure it. The PSM is heavy; use caution to avoid injury during installation. Take care not to damage the surrounding wiring. Avoid pushing the module in too abruptly, as it may lead to injury.</br>
③ Reconnect all connectors to the module. For connectors fastened with screws, use an appropriate screwdriver to secure them, ensuring they are connected firmly without applying excessive force.</br>
④ Double-check to ensure that no connectors are misplaced and that no steps have been omitted.</br>


[__SOURCE](1-elec/Adjustment_tips.md)
## 1.4. Adjustment Procedures

This controller is fully adjusted at the factory prior to shipment; therefore, no additional adjustments are typically required. However, when replacing certain components, some adjustments may be necessary. This section describes the adjustment points and procedures. Do not perform adjustments unless absolutely necessary. If a problem occurs and the cause is not identified, do not attempt to modify the settings.

### 1. Power System Adjustment 

In the event of a power system failure or if the power source is changed, measure each power supply voltage and adjust any values that fall outside the reference range (use a digital multimeter for measurement).

### 1.1. Power System Adjustment for Hi7-N Controller


![](../_assets/1.전장/조정요령/Hi7-N제어기%20전원%20기준치_en.PNG)

Figure 1. Power Supply Reference Values for Hi7-N Controller


(Note 1) If the values are not within the reference range, replace the PSM (Power Supply Module).

(Note 2) First, verify the reference values at the designated measurement points. If possible, measure the voltage between the terminals or connector pins closest to the robot's encoder. In this case, the reference value must be DC 5.1V ± 0.1V

### 2. Transformer (TR2)

{% hint style="warning" %}
Hi7-N Controller: The output power of Transformer (TR2) must be used at AC 220V.</br>
The secondary terminals are wired to power sources that match the specifications of internal components. Never tamper with these connections.</br>
{% endhint %}

The input power for this controller must be 3-phase AC 220V. Controllers with other voltage specifications are fully adjusted before shipment; therefore, taps must never be changed without authorization from our technical staff.

[__SOURCE](2-servo-amp-board-part/README.md)
# 2. Servo AMP Board
[__SOURCE](2-servo-amp-board-part/E02500.md)
## 2.1. E02500 AMP Regenerative Discharge Resistor Overheat

### 1. Overview

This error relates to the overheating of the resistor used to dissipate regenerative power generated during robot deceleration or downward movement in the direction of gravity. It can be caused by decreased cooling fan performance, temporary rapid movements, or exceeding the regenerative discharge capacity due to continuous robot operation.

### 2. Causes and Inspection Methods

{% hint style="info" %}

The temperature of the regenerative discharge resistor has risen above the reference value. This is due to excessive robot playback speed or issues with the cooling system.

* < If the error occurs at a specific step depending on the robot's playback speed >

(1)	Verify the error by adjusting the robot's playback speed.

(2)	Inspect the resistance value of the regenerative discharge resistor.

* <If the error occurs after the robot has been operating for 5 minutes or longer>

(3)	Inspect the controller's cooling system and the amount of regenerative power.

->	Check the operational status of each fan.

->	Inspect the power supply voltage provided to the fans.

(4)	Inspect the robot's regenerative power load.

->	Verify the error by reducing the robot's playback speed to see if the thermal load decreases.

{% endhint %}

(1)	Verify the error by adjusting the robot's playback speed.

During robot deceleration or downward movement in the direction of gravity, the DC voltage of the servo drive unit increases. To prevent component damage caused by this voltage surge, electrical power is consumed through the regenerative discharge resistor. Rapid deceleration or high-speed movement in the direction of gravity can trigger this error. Please verify whether the error occurs according to the robot's playback speed.

* Changing the Robot Playback Speed

An "Regenerative Resistor Overheat" error may occur if the regenerative power generated by the robot's motion exceeds the controller's design specifications. Please operate the robot after reducing the speed of the step where the error occurs and verify if the error persists.


(2)	Inspect the resistance value of the regenerative discharge resistor.

* Inspection of Regenerative Discharge Resistance Value

If the resistance value measured at the end of the CNDR cable deviates by 10% or more from the value specified in the manual, the resistor is defective. Please replace the resistor. Refer to the previous page for the detailed measurement procedure.

 (2)-1. Hi7-N Controller

-> Resistance value for mid-sized robots (H7D6X): 5 ohm (Models N00-00, N00-70: Two 2.5 ohm resistors connected in series)

-> Resistance value for large-sized robots (H7D6X): 4 ohm (Model N00-80)

-> Resistance value for small-sized robots (H7D6A): 15 ohm (Model N00-30)

(2)-2. Hi7-T Controller

-> To be included in the future (TBD)

(2)-3. Hi7-NX Controller

-> To be included in the future (TBD)

(3)	Please inspect the controller's cooling conditions and the amount of regenerative power.

If a regenerative resistor overheat error occurs after the robot has been operating for 5 minutes or longer, it indicates either a malfunction in the controller’s cooling system or that the robot’s playback speed exceeds the controller’s design specifications. Fans are installed at the rear of the controller to cool the servo drive unit's heatsink and the regenerative discharge resistor.

![](../_assets/2.서보AMP/E02500/E02500_1.png  )

Figure 2.1.1 Installation Locations of Hi7-N00 Controller Fans

* Inspection of Fan Operational Status

If a fan is not rotating or its speed is abnormally low, please replace the corresponding fan. The lifespan of a cooling fan varies depending on the operating environment and total usage hours.


* Inspection of Fan Power Supply Voltage

If all fans are inoperative, please verify the fan input voltage. The fan input voltage is set to AC 220V, with an allowable range within 10% of the rated voltage. If the voltage is more than 10% below the rating, the cooling efficiency will decrease due to the reduced fan rotation speed. If the voltage is low, please inspect the fan power connector (CNFN2) and the overall input voltage of the controller.

(4)	Please inspect the robot's regenerative power load.

* Verify the error according to the robot's playback speed.

If an overheat error occurs during continuous playback for 5 minutes or longer, it is likely because the robot's repetitive motions have exceeded the controller's cooling capacity. Please reduce the robot's playback speed and verify if the error persists. If the overheat error is resolved by lowering the speed but the required cycle time for the task cannot be achieved, please contact our technical support department.

[__SOURCE](2-servo-amp-board-part/E02501.md)
## 2.2. E02501 AMP Regenerative Discharge Resistor Open Circuit, Resistor or Circuit Error

### 1. Overview

This error occurs during the dissipation of regenerative power generated during robot deceleration or downward movement in the direction of gravity. It can be caused by a failure in the overheat detection sensor circuit, an open circuit in the resistor, or an overvoltage in the 3-phase power supply.

### 2. Causes and Inspection Methods

{% hint style="info" %}
Overheat errors can also occur due to an open circuit in the resistor or an anomaly in the discharge control system. Additionally, an increase in the regenerative resistance value or a surge in the 3-phase power supply voltage may trigger this error.

* < If the error consistently occurs at the moment the motor is turned ON >

(1)	Inspect the resistance value of the regenerative discharge resistor.

-> Check the resistance value at the CNDR cable.

(2)	Inspect the servo drive unit.

-> Replace the servo drive unit and verify if the error persists.

(3)	Inspect the power-related components.

-> Check the internal 3-phase voltage of the controller.

-> Check the input 3-phase voltage supplied to the controller.

{% endhint %}

(1)	Please inspect the resistance value of the regenerative discharge resistor.

Overheat errors may also occur due to an open circuit in the resistor or an increase in the regenerative resistance value.
 
* Inspection for Open Circuit in the Regenerative Resistor

If the resistance measured at the end of the CNDR cable is in the range of several mega-ohm, it indicates either an open circuit in the resistor or a poor internal wiring contact. Please replace the regenerative resistor with a known functional unit or repair the wiring.

![](../_assets/2.서보AMP/E02501/E02501_1.png)

Figure 2.2.1. Measuring Resistance at the CNDR Connector

(a) Hi7-N Controller (BD651 / BD653 Board)

(b) Hi7-T Controller (To be included in the future)

(c) Hi7-NX Controller (To be included in the future)

(2)	Please inspect the power-related components.

Overheat errors can also occur due to anomalies in the discharge control circuit.

* Replacement Inspection of the Drive Unit

Replace the module that detects the regenerative discharge resistor overheat error and verify if the error recurs. A circuit failure within the module may cause the error to persist.

(2)-1. Hi7-N Controller

-> Servo drive unit for mid-sized robots: H7D6X

-> Servo drive unit for small-sized robots: H7D6A

(2)-2 Hi7-T Controller

-> To be included in the future (TBD)

(2)-3 Hi7-NX Controller

-> To be included in the future (TBD)


(3)	Please inspect the power-related components.

Overheat errors can occur due to an open circuit in the resistor or an anomaly in the discharge control system. Furthermore, an increase in the regenerative resistance value or a surge in the 3-phase power supply voltage may also trigger this error.

* Inspection of Internal 3-Phase Voltage of the Controller

Regenerative discharge operation begins at approximately DC 375V. If a voltage of AC 242V or higher is supplied to the servo drive unit, a regenerative resistor overheat error may be triggered the moment the motor is turned ON. If the input voltage exceeds the allowable range, please perform inspections according to the controller input voltage and internal 3-phase voltage inspection procedures.

-> Servo Drive Unit Input Voltage Specification: 3-phase AC 220V
-> Allowable Range when Motor is ON: 198V ~ 242V

[__SOURCE](2-servo-amp-board-part/E02502.md)
## 2.3. E02502 AMP Regenerative Discharge Resistor Detection Circuit Error

### 1. Overview

This error relates to the overheating of the resistor used to dissipate regenerative power generated during robot deceleration or downward movement in the direction of gravity. It is typically caused by a failure in the overheat detection sensor circuit or a cable-related issue.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly has occurred in the path used to detect overheat errors, or the resistance value has changed.

* < If the error consistently occurs even when the motor is OFF >

(1)	Inspect the cables related to overheat error detection.

-> Check the resistance of the CNTR cable.

(2)	Inspect the components related to overheat error detection.

-> Hi7-N Controller: Replace the Control Module (including the BD642 board) and verify if the error persists.

-> Hi7-T Controller: (To be included in the future)

-> Servo Drive Unit: Replace the servo drive unit and verify if the error persists.

{% endhint %}

(1)	Please inspect the overheat error detection cable.

The regenerative resistor overheat error is detected by the servo drive unit by monitoring the ON/OFF status of the overheat sensor attached to the resistor via the CNTR connector. In the Hi7-N controller, the detected error signal is transmitted from the BD651/BD653 board through the BD652/BD654 and is finally processed by the software on the BD642 board.

![](../_assets/2.서보AMP/E02502/E02502_1.png  )

Figure 2.3.1. Component Layout for Regenerative Resistor Overheat Error (Hi7-N Controller)

* CNTR Cable Inspection

Check for any anomalies in the sensor at the CNTR connector that connects to the overheat detection sensor. Under normal conditions, the sensor resistance should measure less than 0.1 ohm.

![](../_assets/2.서보AMP/E02502/E02502_2.png  )

Figure 2.3.2. Measuring Resistance at the CNTR Connector (Hi7-N Controller)

(2)	Please inspect the components related to overheat error detection.
	
* Servo Control Board Replacement Inspection

Replace the servo control board with a known functional unit. If the error does not recur, the original board is defective. Please replace it with a normal part for continued use.

-> Hi7-N Controller: BD642

-> Hi7-T Controller: To be included in the future (TBD)

-> Hi7-NX Controller: To be included in the future (TBD)


* Replacement Inspection of the Servo Drive Unit

The modules responsible for detecting the regenerative discharge resistor overheat error are as follows.

-> Hi7-N Controller: H7D6X for mid-sized robots, H7D6A for small-sized robots (excluding the servo board).

-> Hi7-T Controller: To be included in the future (TBD).

-> Hi7-NX Controller: To be included in the future (TBD).

Please identify the specific components installed in your current controller before proceeding with the inspection. Replace the unit with a known functional part and verify whether the error recurs.

[__SOURCE](2-servo-amp-board-part/E02503.md)
## 2.4. E02503 AMP PN Overvoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error can occur when the robot's motion changes abruptly or if the resistance value of the regenerative discharge resistor has increased.

* < If the error occurs at a specific step depending on the robot's playback speed >

(1)	Verify the error by adjusting the robot's playback speed.

(2)	nspect the resistance value of the regenerative discharge resistor.

{% endhint %}

(1)	Please verify the error occurrence according to the robot's playback speed.

Rapid deceleration or high-speed downward movement in the direction of gravity can trigger an overvoltage error. Please verify whether the error occurs depending on the robot's playback speed. An AMP overvoltage error can also be caused by a defective regenerative discharge resistor or an anomaly in the regenerative discharge control system.

* Changing the Robot Playback Speed

An overvoltage error may occur if the regenerative power generated by the robot's motion exceeds the controller's design specifications. Please operate the robot after reducing the speed of the step where the error occurs and verify if the error persists. If the error does not occur at a lower speed, please adjust the taught speed of that step before further use.

(2)	Please verify the error occurrence according to the robot's playback speed.

* Inspection of Regenerative Discharge Resistance Value

If the resistance value is higher than the specification, regenerative discharge cannot be performed smoothly, which may lead to an overvoltage error. The specifications for the regenerative resistor may vary depending on the controller model. Please refer to the manual and the Controller Check Sheet provided at the time of purchase. If the measured resistance value deviates from the specification by more than 10%, please replace the resistor.

(2)-1. Hi7-N Controller

-> Resistance value for mid-sized robots (Hi7-N00-00, H7D6X): 5 ohm (N00)

-> Resistance value for large-sized robots (Hi7-N00-80, H7D6X): 4 ohm (N80)

-> Resistance value for small-sized robots (Hi7-N00-30, H7D6A): 15 ohm (N30)

(2)-2 Hi7-T Controller

-> To be included in the future (TBD)

(2)-3 Hi7-NX Controller 

-> To be included in the future (TBD)

![](../_assets/2.서보AMP/E02503/E02503_1.png  )

Figure 2.4.1. Measuring Resistance at the CNDR Connector (Hi7-N Controller)
[__SOURCE](2-servo-amp-board-part/E02504.md)
## 2.5. E02504 AMP Diode Module Error or AC Input Voltage Exceeded

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold of DC 395V.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly in the diode module has caused the PN voltage to fall outside the allowable range. This error can also occur if the 3-phase AC voltage supplied to the servo drive unit (AMP) is abnormally high.

* < If the error consistently occurs at the moment the motor is turned ON >

(1)	Inspect the power-related components.

-> Replace the servo drive unit and verify if the error persists.

(2) Inspect the power supply voltage.

-> Check the internal 3-phase voltage of the controller.

-> Check the input 3-phase voltage supplied to the controller.

{% endhint %}

(1)	Please inspect the power-related components.

* Replacement Inspection of the Servo Drive Unit

Replace the module responsible for detecting the AMP overvoltage error and verify if the error recurs. A circuit failure within the module may cause the error to persist.

(1)-1. Hi7-N Controller

-> Servo drive unit for mid-sized robots: H7D6X

-> Servo drive unit for small-sized robots: H7D6A

(1)-2. Hi7-T Controller

-> Servo drive unit for electronics industry robots: To be included in the future (TBD)

(1)-3. Hi7-NX Controller

-> Servo drive unit for large-sized robots: To be included in the future (TBD)

(2)	Please inspect the power supply voltage.

* Hi7-N and NX Controller: 3-Phase Voltage Inspection

If a voltage of AC 242V or higher is supplied to the servo drive unit, an overvoltage error may be triggered at the moment the motor is turned ON. If the input voltage exceeds the allowable range, please inspect the voltage following the controller input voltage and internal 3-phase voltage inspection procedures.

-> Servo Drive Unit Input Voltage Specification: 3-phase AC 220V

-> Allowable Range when Motor is ON: 198V ~ 242V

* Hi7-T Controller: Single-Phase Voltage Inspection (To be included in the future)

If a voltage of AC 242V or higher is supplied to the servo drive unit, an overvoltage error may be triggered at the moment the motor is turned ON. If the input voltage exceeds the allowable range, please inspect the voltage following the controller input voltage and internal single-phase voltage inspection procedures.

-> Servo Drive Unit Input Voltage Specification: Single-phase AC 220V

-> Allowable Range when Motor is ON: 198V ~ 242V


[__SOURCE](2-servo-amp-board-part/E02505.md)
## 2.6. E02505 AMP PN Overvoltage Detection Path Error or Discharge Error

Former Error Code: E0011 AMP P-N Overvoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly has occurred in the path used to detect PN voltage drops from the diode module, or a failure has occurred in the PN discharge circuit.

* < If the error consistently occurs even when the motor is OFF >

(1)	Hi7-N Controller

->  Replace the BD642 board and verify if the error persists.

->  Replace the Control Module and verify if the error persists.

->	Replace the servo drive unit and verify if the error persists.

(2)	Hi7-T Controller

->	To be included in the future (TBD)

(3)	Hi7-NX Controller

->	To be included in the future (TBD)


{% endhint %}

(1)	Hi7-N Controller

The overvoltage error in the Hi7-N controller AMP is detected by the servo drive unit when the DC link power (P-N) supplied to the unit exceeds the preset level. The detected error is then processed by the BD642 board via the AMP boards (BD651, BD652, BD653, or BD654).

-> Replacement Inspection of the BD642 Board

Replace the BD642 board with a known functional unit. If the error does not recur, the original board is defective. Please replace the BD642 with a normal part for continued operation.

-> Replacement Inspection of the Servo Drive Unit

The modules responsible for detecting the AMP overvoltage error are as follows:

* Hi7-N Controller: H7D6X (for mid-sized robots) or H7D6A (for small-sized robots), excluding the servo board.

Please verify the specific components installed in your current controller before proceeding with the inspection. Replace the unit with a known functional part and verify whether the error recurs.

![](../_assets/2.서보AMP/E02505/E02505_1_en.png)

Figure 2.6.1. Component Layout for Overvoltage Error (Hi7-N Controller)

<br>

(2)	Hi7-T Controller

->	To be included in the future (TBD)

(3)	Hi7-NX Controller

->	To be included in the future (TBD)
[__SOURCE](2-servo-amp-board-part/E02506.md)
## 2.7. E02506 AMP PN Undervoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error may occur at a specific step depending on the robot's playback speed. It indicates that the PN voltage has dropped due to high energy consumption. It can also be caused by an unstable 3-phase input power supply to the controller.

* < If the error occurs at a specific step depending on the robot's playback speed >

(1)	Verify the error by adjusting the robot's playback speed.

(2)	Inspect the controller's power supply voltage.

->	Check the 3-phase or single-phase input voltage of the controller while the robot is in motion.

->	If the input voltage is not 220V, inspect the internal 3-phase or single-phase voltage settings and levels.

{% endhint %}

(1)	Please verify the error occurrence by adjusting the robot's playback speed.

An AMP undervoltage error occurs when the input power capacity is insufficient or when the robot undergoes rapid acceleration. Please verify whether the error occurs according to the robot's playback speed and monitor the fluctuations in the 3-phase voltage supplied to the servo drive unit.

* Changing the Robot Playback Speed

An undervoltage error may occur if the instantaneous power required by the robot's motion exceeds the controller's design specifications. Please operate the robot after reducing the speed of the step where the error occurs and verify if the error persists. If the error is resolved at a lower speed, please adjust the taught speed of that step before further use.


(2)	Please inspect the controller's power supply voltage.

* Hi7-N and NX Controller: 3-Phase Voltage Inspection at the Error Step

The AMP undervoltage error is triggered when the DC link voltage drops to approximately DC 142V (or 210V). If the 3-phase input voltage supplied to the servo drive unit falls below AC 100V (or 148V) during the step where the error occurs, an undervoltage fault may be generated. If the input voltage falls outside the allowable range, please perform inspections following the controller input voltage and internal 3-phase voltage inspection procedures.

->	Servo Drive Unit Input Voltage Specification: 3-phase AC 220V

->	Allowable Range when Motor is ON: AC 198V ~ 242V


* Hi7-T Controller: Single-Phase Voltage Inspection at the Error Step

The AMP undervoltage error is triggered when the DC link voltage drops to approximately DC 142V (or 210V). If the single-phase input voltage supplied to the servo drive unit falls below AC 100V (or 148V) during the step where the error occurs, an undervoltage fault may be generated. If the input voltage falls outside the allowable range, please perform inspections following the controller input voltage and internal single-phase voltage inspection procedures.

->	Servo Drive Unit Input Voltage Specification: Single-phase AC 220V

->	Allowable Range when Motor is ON: AC 198V ~ 242V




[__SOURCE](2-servo-amp-board-part/E02507.md)
## 2.8. E02507 AMP Diode Module Error or AC Input Voltage Insufficient


Former Error Code: E0033 AMP PN Undervoltage Generated


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

The PN voltage failed to charge due to an anomaly in the diode module. This error can also occur if the AC voltage supplied to the servo drive unit is insufficient.

* < If the error occurs at the moment the motor is turned ON >

  * Hi7-N Controller, NX Controller

     (1)	Inspect the power-related components.
     
     -> Replace the servo drive unit and verify if the error persists.

     (2)	Inspect the controller's power supply voltage.

     ->	Check the internal 3-phase voltage of the controller.
     
     ->	Check the input 3-phase voltage supplied to the controller.

  * Hi7-T Controller

     (3)	Inspect the power-related components.
     
     -> Replace the BD667T board and verify if the error persists.

     (4)	Inspect the controller's power supply voltage.

     ->	Check the internal single-phase voltage of the controller.

     ->	Check the input single-phase voltage supplied to the controller.

{% endhint %}


* Hi7-N Controller

(1)	Please inspect the power-related components.

The AMP undervoltage error occurs when the 3-phase AC 220V input to the servo drive unit falls outside the allowable range. It may also occur if an anomaly in the regenerative discharge control circuit triggers a discharge operation at the moment the motor is turned ON.

** Replacement Inspection of the Servo Drive Unit

Replace the module responsible for detecting the AMP undervoltage error and verify if the error recurs. A circuit failure within the module may cause the error to persist.

The modules responsible for detecting the AMP undervoltage error are as follows:

->	For mid-sized robots: H7D6X

-> For small-sized robots: H7D6A


(2)	Please inspect the controller's power supply voltage.

** 3-Phase Voltage Inspection

The AMP undervoltage error is triggered at approximately DC 142V. If the motor is turned ON while the voltage supplied to the servo drive unit is below AC 100V, an undervoltage error may occur. If the input voltage falls outside the allowable range, please perform inspections following the controller input 3-phase voltage and internal 3-phase voltage inspection procedures.

->	Servo Drive Unit Input Voltage Specification: 3-phase AC 220V

->	Allowable Range when Motor is ON: AC 198V ~ 242V


* Hi7-T Controller (To be included in the future)

(3)	Please inspect the power-related components.

The AMP undervoltage error occurs when the single-phase AC 220V input to the servo drive unit falls outside the allowable range. It may also occur if an anomaly in the regenerative discharge control circuit triggers a discharge operation at the moment the motor is turned ON.

**	Replacement Inspection of the Servo Drive Unit

Replace the module responsible for detecting the AMP overvoltage error and verify if the error recurs. A circuit failure within the module may cause the error to persist.

The modules responsible for detecting the AMP undervoltage error are as follows:

->	To be included in the future (TBD)


(4)	Please inspect the controller's power supply voltage.

**	Single-Phase Voltage Inspection

The AMP undervoltage error is triggered at approximately DC 142V. If the motor is turned ON while the voltage supplied to the servo drive unit is below AC 100V, an undervoltage error may occur. If the input voltage falls outside the allowable range, please perform inspections following the controller input single-phase voltage and internal single-phase voltage inspection procedures.

->	Servo Drive Unit Input Voltage Specification: Single-phase AC 220V

->	Allowable Range when Motor is ON: AC 198V ~ 242V


* Hi7-NX Controller (To be included in the future)

-> Specifications and inspection procedures for the Hi7-NX model will be updated in a future revision.
[__SOURCE](2-servo-amp-board-part/E02508.md)
## 2.9. E02508 AMP PN Undervoltage Detection Path Error or Discharge Error


Former Error Code: E0033 AMP PN Undervoltage Generated


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

A problem has occurred in the path used to detect PN voltage drops starting from the diode module. Alternatively, an anomaly has occurred in the PN discharge circuit.

* < If the error occurs even when the motor is OFF >

  * Hi7-N Controller

     (1)	Inspect the components related to undervoltage error detection.
     
     -> Replace the BD642 board and verify if the error persists.

     ->	Replace the servo drive unit and verify if the error persists.

    
  * Hi7-T Controller (To be included in the future)

     (2)	Inspect the components related to undervoltage error detection.
     
     -> To be included in the future (TBD)

{% endhint %}

(1)	Please inspect the components related to undervoltage error detection.

* Replacement Inspection of the BD642 Board

   Replace the BD642 board with a known functional unit. If the error does not recur, the original board is defective and should be replaced.

* Replacement Inspection of the Servo Drive Unit

   The modules responsible for detecting the AMP undervoltage error are as follows:

  -> Hi7-N Controller: H7D6X (for mid-sized robots) or H7D6A (for small-sized robots), excluding the servo board.

  Please verify the specific components installed in your current controller before proceeding with the inspection. Replace the unit with a known functional part and verify whether the error recurs.


![](../_assets/2.서보AMP/E02508/E02508_1_en.png  )

Figure 2.9.1. Replacement of Control Module and Servo Drive Unit

<br>


(2) Please inspect the components related to undervoltage error detection.

-> To be included in the future (TBD)

[__SOURCE](2-servo-amp-board-part/E02522.md)
## 2.10. E02522 (Axis ○) IPM Fault – Specific Step

### 1. Overview

A fault output has been triggered from the IPM (Intelligent Power Module), which is the switching element within the servo drive unit that powers the motor. An IPM fault can be caused by a temperature rise in the heat sink, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Methods

{% hint style="info" %}

* < If the error occurs at a specific step >

(1)	Inspect the robot at the step where the error occurs.

->  Inspect the robot's wiring at the position where the error is triggered.

->  Verify the error by reducing the robot's playback speed.

->  Verify the error after changing the interpolation of the taught step.

{% endhint %}


(1)	Please inspect the robot at the step where the error occurs.

An IPM fault error occurring at a specific step can be triggered when damage to the internal wiring becomes more pronounced at that particular taught position, or when the axis speed changes drastically during a posture transition in the taught program.

->  Inspect the internal wiring at the position where the error occurs.

Examine the condition of the internal robot wiring connected to the motor of the corresponding axis. During inspection, turn OFF the controller power, disconnect the output connector from the servo drive unit, and measure the resistance between each phase and the ground on the cable side to check for a short circuit.

![](../_assets/2.서보AMP/E02522/E02522_2.PNG)

Figure 2.10.1. Internal Wiring Inspection Points by Axis


-> Verify the error by reducing the robot's playback speed

If the error occurs at a step where a posture change causes a sudden fluctuation in axis speed, reduce the playback speed to verify the error. If the error is resolved after lowering the playback speed, adjust the taught speed for that specific step and save the task program before further use.

->  Verify the error by changing the interpolation of the taught step

If the axis speed continues to fluctuate drastically even after reducing the playback speed to 75% or lower, change the interpolation of the taught step to 'P' (PTP: Point-to-Point) and verify the error. If the error is resolved by changing the interpolation at the same playback speed, please modify the teaching points accordingly.

[__SOURCE](2-servo-amp-board-part/E02541.md)
## 2.11. E02541 Drive Unit Control Voltage Low

### 1. Overview

The +15V control power supplied to the servo drive unit has dropped below the threshold. This error is detected through different paths depending on the controller model and then transmitted to the servo board.

*   Hi7-N: Detected directly by the servo drive unit.

### 2. Causes and Inspection Methods

{% hint style="info" %}

*   < Checking the Power LEDs >

    (1)	Please inspect the power status LEDs.

    ->  Hi7-N: Check the 'POW' LED located on the servo drive unit.

    ->  Hi7-T: To be included in the future (TBD)
    
    ->  Hi7-NX: To be included in the future (TBD)

    ->  Check the 24V control power voltage at the PSM (Power Supply Module).


*   < If both the Board LEDs and PSM LEDs are OFF >

    (2)	Please inspect the output of the control power supply (PSM).

    -> Hi7-N Controller

    *  Disconnect the CN24VB1 connector connected to the BD604 of the Control Module, then check the 24V output status LED on the PSM.

    *   Remove the BD642 board, then check if the 'POW' LED on the servo drive unit lights up.

    ->  Hi7-T Controller: To be included in the future (TBD)

    -> Hi7-NX Controller: To be included in the future (TBD)


    (3)	Please inspect the control power supply unit (CMSMPS).

    ->  Check the input voltage supplied to the CMSMPS.

    ->  Replace the CMSMPS and check the status LEDs.

    * < If only the Board LEDs are OFF >

    (4)	Replace the relevant components and check the power status LEDs.

    -> Hi7-N Controller

    * Replace the CN24VB1 cable that connects the PSM and the Control Module, then check the LEDs.

    * Replace the servo board (BD642) and check the LEDs.

    * Replace the servo drive unit and check the LEDs.

    ->  Hi7-T : To be included in the future (TBD)

    ->  Hi7-NX : To be included in the future (TBD)


{% endhint %}


(1)	Please inspect the power status LEDs.

The drive unit control voltage low error is triggered when the +15V control power drops. This fault is detected through different paths depending on the controller model and is then transmitted to the servo board.

*   Hi7-N: Detected directly by the servo drive unit.

*   Hi7-T : To be included in the future (TBD)

*   Hi7-NX : To be included in the future (TBD)

![](../_assets/2.서보AMP/E02541/E02541_1.png )

Figure 2.11.1. Location of Controller Power LEDs (Location of the ‘POW LED’ on the Hi7-N Servo Drive Unit)

<br>


(2)	Please inspect the output of the control power supply (PSM).

->  Hi7-N Controller

*   Disconnect the CN24VB1 connector from the BD642 board, then check the 'SMPS OK' LED on the PSM.

*   Remove the BD642 board, then check the 'POW' LED on the servo drive unit.

->  Hi7-T : To be included in the future (TBD)

->  Hi7-NX : To be included in the future (TBD)

(3)	Check the control power supply unit.

->  Check the input voltage supplied to the CMSMPS.

->  Replace the CMSMPS and verify the status of the LED.

(4)	Replace related components and check the power indicator LED.

->  Hi7-N

*   Replace the CN24VB1 cable connecting the PSM and BD604 of the Control Module, then check the LED.

*   Replace the Servo Board and check the LED.

*   Replace the Servo Drive Unit and check the LED.

->  Hi7-T : To be included in the future (TBD)

->  Hi7-NX : To be included in the future (TBD)


[__SOURCE](2-servo-amp-board-part/E50300.md)
## 2.12. E50300 (Axis ○) IPM Fault

### 1. Overview

An IPM (Intelligent Power Module) fault output has occurred within the switching element of the servo drive unit that operates the motor. An IPM fault can be triggered by an increase in heat sink temperature, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Procedures

{% hint style="info" %}

* < If the error occurs at the moment the motor is turned on or occurs intermittently >

(1)	Inspect the motor drive components.

->	Check the output cables connected to the servo drive unit.

->	Inspect the terminals of the switching elements inside the servo drive unit.

->	Replace the servo board and verify if the error persists.

*	Hi7-N Controller : BD642

*	Hi7-T Controller : To be included in the future (TBD)

*	Hi7-NX Controller : To be included in the future (TBD)

->  Please check the error after replacing the servo drive.

*	Hi7-N Controller : Medium H7D6X, Small: H7D6A (excluding servo board)

*	Hi7-T Controller : To be included in the future (TBD)

*	Hi7-NX Controller : To be included in the future (TBD)

->	Replace the servo motor and verify if the error persists.


< If the error occurs after the robot has been operating for 5 minutes or longer >

(2)	Inspect the controller's cooling fans.

->	Check the operating status of each fan.

->	Check the power supply voltage of the fans.

{% endhint %}

(1)	Inspect the motor drive components.

The servo drive unit that operates the motor receives commands from the servo board (BD642) through a direct board-to-board connector. The current output from the internal amplification circuit is then delivered to the motor via the wiring connected to each axis connector.

->	Inspect the output cables connected to the servo drive unit.

Check the condition of the wiring connecting the servo drive unit to the motor. When inspecting, ensure the controller power is OFF, then disconnect the connector from the servo drive unit. Measure the resistance between each phase and the ground on the cable side to check for any short circuits.

![](../_assets/2.서보AMP/E02520/E02520_1_en.png)


Figure 2.12.1. Inspection of the output cable for the Hi7-N controller servo drive unit

<br>


->	Inspect the switching elements of the servo drive unit.

The switching elements of the servo drive unit output AC current for each phase by switching the DC voltage supplied from the diode module. If a short circuit occurs at the internal terminals of the switching element, overcurrent flows, triggering an IPM fault error. With the connectors disconnected, check for a short circuit between the output terminals (U, V, or W) and the P or N terminals of the switching element. If a short circuit is confirmed, the servo drive unit must be replaced, and the cable connecting the servo drive unit to the motor should also be inspected.

*	Hi7-N Controller

    -	Servo drive unit for mid-sized robots: H7D6X

    -	Servo drive unit for small-sized robots: H7D6A 


*	Hi7-T제어기 (To be included in the future)

*	Hi7-NX제어기 (To be included in the future)

![](../_assets/2.서보AMP/E02520/E02520_2.png)


Figure 2.12.2. Inspection for short circuits in the switching elements of the Hi7-N controller

<br>

->	Replacement and inspection of the servo board.

If the error does not recur after replacing the servo board, the original servo board is defective. Please replace the servo board with a known-good unit.

*	Hi7-N Controller: BD642

*	Hi7-T Controller : To be included in the future

*	Hi7-NX Controller : To be included in the future

->	Replacement and inspection of the servo drive unit.

If the error does not recur after replacing the servo drive unit, the original servo drive unit is defective. Please replace the servo drive unit with a known-good unit.

*	Hi7-N Controller

    -	Servo drive unit for mid-sized robots: H7D6X

    -	Servo drive unit for small-sized robots: H7D6A 

*	Hi7-T Controller : To be included in the future

*	Hi7-NX Controller : To be included in the future


->	Replacement and inspection of the servo motor.

If the error does not recur after replacing the servo motor, the original servo motor is defective. Please replace the servo motor with a known-good unit. The figure below shows the location of the motors for each axis of the robot. For other robot models, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/2.서보AMP/E02520/E02520_3.PNG)

Figure 2.12.3. Servo motor locations for each axis of the robot

<br>

(2)	Inspect the controller’s cooling fans.

If an IPM fault error occurs after the robot has been operating for 5 minutes or longer, it indicates that the controller's cooling system is malfunctioning, causing the IPM to exceed its specified operating temperature range. The rear of the controller is equipped with fans to cool the heat sinks of the servo drive units and the regenerative discharge resistors.

<br>


Figure 2.12.4. Installation locations of Hi7 controller fans

![](../_assets/2.서보AMP/E02520/E02520_4.png)


->	Check the operating status of each fan.

If a fan is not rotating or the rotation speed is abnormally low, please replace the affected fan. The lifespan of a fan varies depending on the operating environment and total usage hours.


->	Check the fan power supply voltage.

If all fans are not operating, please check the input voltage supplied to the fans. The input voltage for the fans is set to 220V AC, with an allowable tolerance of within 10% of the rated voltage. If the voltage is more than 10% lower than the rating, the cooling efficiency will decrease due to the reduced fan rotation speed. If the voltage is low, please check the power connector for the rear cooling fans and the main input voltage of the controller.

[__SOURCE](2-servo-amp-board-part/E50301.md)
## 2.13. E50301 (Axis ○) IPM Fault - Gate Drive Power Undervoltage

### 1. Overview

An IPM (Intelligent Power Module) fault output has occurred within the switching element of the servo drive unit that operates the motor. While an IPM fault can be caused by an increase in heat sink temperature, a drop in IPM control voltage, or an overcurrent output, this specific error is detected while the servo is in the OFF state. Since the system only monitors for a drop in control voltage when the servo is OFF, you must inspect items related to the amplifier's Gate drive power supply.

### 2. Causes and Inspection Procedures

{% hint style="info" %}

* < If the IPM fault error occurs while the servo is in the OFF state >

(1) Inspect the motor drive components.

->  Check the output cables connected to the servo drive unit.

->  Replace the servo drive unit and verify if the error persists.

->  Replace the servo board and verify if the error persists.

{% endhint %}

(1)	Inspect the motor drive components.

The servo drive unit that operates the motor receives commands from the servo board through an interface board and board-to-board connector. The current output from the internal amplification circuit is then delivered to the motor via the wiring connected to each axis connector.

->  Inspect the output cables connected to the servo drive unit.

Check the condition of the wiring connecting the servo drive unit to the motor. During inspection, ensure the controller power is OFF, then disconnect the connector from the servo drive unit. Measure the resistance between each phase and the ground on the cable side to check for any short circuits.


![](../_assets/2.서보AMP/E02521/E02521_1_en.png)

Figure 2.13.1. Inspection of the output cable for the Hi7-N controller servo drive unit

<br>


->  Replacement and inspection of the servo drive unit.

If the error does not recur after replacing the servo drive unit, the original servo drive unit is defective. Please replace the servo drive unit with a known-good unit.

*   Hi7-N Controller

    -  Servo drive unit for mid-sized robots: H7D6X
    -  Servo drive unit for small-sized robots: H7D6A

*   Hi7-T Controller: To be included in the future

*   Hi7-NX Controller: To be included in the future

->  Replacement and inspection of the servo board.

If the error does not recur after replacing the servo board, the original servo board is defective. Please replace the servo board with a known-good unit.

*   Hi7-N Controller: BD642
*   Hi7-T Controller: To be included in the future
*   Hi7-NX Controller: To be included in the future
[__SOURCE](3-safety-board-part/README.md)
# 3. Servo Safety Board (Safety Section)
[__SOURCE](3-safety-board-part/N00088.md)
## 3.1. N00088 External Emergency Stop (E-Stop) Input

### 1. Overview
An external emergency stop (E-Stop) signal has been triggered.<br>
To ensure safety, all robot motions are immediately stopped, and the servo motors are switched to **Motor OFF** state.

### 2. Causes and Checks
{% hint style="info" %}
(1) The external emergency stop (E-Stop) button was actually pressed.<br>
(2) There is a problem in the wiring or contacts of the external E-Stop circuit.<br>
(3) The safety input assignment for the external E-Stop signal is not configured.<br>
{% endhint %}<br>

### (1) When the External E-Stop Button Was Actually Pressed
Check whether the external emergency stop (E-Stop) button was actually pressed. Another operator or administrator may have triggered the E-Stop button.<br>
Also, verify if there are any personnel around the robot or potential hazards (tools, jigs, etc.) inside the safety fence, as someone might be working within it.<br>
If it is judged safe to restart the robot, release the external E-Stop button first and operate the robot in **Manual Mode** before resuming normal operation.<br>

### (2) When There Is an Issue with the Wiring or Contacts of the External E-Stop Circuit
To inspect the wiring related to the external E-Stop, first check which input channel the external E-Stop signal is assigned to through the **Safety I/O Assignment** function.<br>
By default (factory setting), the external E-Stop input is assigned to the basic safety input.

System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety I/O -> 1: I/O Assignment<br>
![](../_assets/3-Safety-io/N00088/base_add_comm_si_func_sel.png)<br>
Figure 3.1.1. T/P Screen Safety I/O Assignment

#### 2-1) When Assigned to Basic Safety Input
If the external E-Stop input is assigned to the **Basic Safety Input**, it is connected to the **CNSI1 connector (4 channels)** on the Servo Safety Board. For detailed pin mapping of this connector, refer to **Hi7 Controller Maintenance Manual, Section 4.3.2.6**.

![](../_assets/3-Safety-io/N00088/bd642_cnsi1_position.png)<br>
Figure 3.1.2. Hi7-N Controller Servo Safety Board CNSI1 Location<br>

Check which channel the external E-Stop input is assigned to. The input channel assignment can be confirmed using Figure 3.1.1.<br>
Once the assigned input channel is confirmed, refer to the site electrical drawings or wiring diagrams to ensure that the wiring is correct. Also, check the actual wiring for proper connections and assembly.<br>
When verifying the electrical drawings or wiring diagrams, refer to **Hi7 Controller Maintenance Manual, Section 4.3.2.6** for the standard wiring of the Servo Safety Board CNSI1.

#### 2-2) If Assigned to Extended Safety Input  
If the external E-Stop input is assigned to an extended safety input, it is connected to the Option Safety IO Board CNSI2 connector (8 channels). Refer to **Hi7 Controller Maintenance Manual, Section 5.4.6** for the detailed pinout of this connector.  
![](../_assets/3-Safety-io/N00088/bd680_cnsi2_position.png)<br>
Figure 3.1.3. Hi7-N Controller Option Safety IO Board CNSI2 Location<br>

Check which channel the external E-Stop input is assigned to. The input channel assignment can be confirmed using Figure 3.1.1.<br>
Once the assigned input channel is confirmed, refer to the site electrical drawings or wiring diagrams to ensure proper wiring. Also, inspect the actual wiring for proper connections and assembly.<br>
When verifying the electrical drawings or wiring diagrams, refer to **Hi7 Controller Maintenance Manual, Section 5.4.6** for the standard wiring of the Option Safety IO Board CNSI2.

#### 2-3) When assigned to Safety Communication Input
If the external E-Stop input is assigned to the Safety Communication Input, refer to the **Hi7 Robot Controller Function Manual – Industrial Communication**.

### (3) When no safety input assignment is set for the external E-Stop signal
If the external E-Stop input is not selected in the safety input assignment, activate the external E-Stop function by selecting one of the following options:<br>

- Basic Safety Input<br>
- Extended Safety Input<br>
- Safety Communication Input<br>

The safety input assignment can be configured through the following menu:

System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety IO -> 1: Input/Output Assignment<br>
![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)<br>
Figure 3.1.4. T/P screen – Safety Input/Output Assignment

[__SOURCE](3-safety-board-part/E00002.md)
## 3.2. E00002 Primary Axis Limit Switch Activated

### 1. Overview

The limit switch installed at the end of the travel range for each robot axis has been triggered. For safety, the robot immediately stops and cannot operate normally until it is moved back to a safe operating range using the proper procedure.

### 2. Cause and Inspection

{% hint style="info" %}
(1) Verify whether the robot has actually moved outside the operating range.<br>
* Recovery procedure when the operating range is exceeded<br>

(2) If the error occurs even though the operating range has not been exceeded<br>
* Check at the system board connector (CNLS)<br>
* Inspect the wire harness (C(M)ER1 or C(M)EC1)<br>
* Check the limit switch and internal wiring of the main body<br>
* Inspect the safety board (BD632)<br>

(3) If there is an abnormality in the wiring or contacts of the Primary Axis limit switch circuit<br>

(4) If the safety input assignment for the Primary Axis limit switch has not been configured<br>
{% endhint %}

### (1) Verify Whether the Robot Has Actually Exceeded the Operating Range

Check whether the robot has moved outside its designated operating range. If a soft limit error occurs simultaneously, the robot has indeed exceeded the operating range. Move the robot back into the operating range using proper operation procedures. The operating range varies depending on the robot model, so the installation position of the limit switches may also differ. Refer to the “Operating Range Limits” section in the maintenance manual of the respective robot.

![](../_assets/3-Safety-io/E00002/그림1.jpg)<br>
Figure 3.2.1. Example of Hardware Limit Switch Installation Position

![](../_assets/3-Safety-io/E00002/그림2.png)<br>
Figure 3.2.2. Example of Hardware Limit Switch Operating Range

#### [Recovery Procedure When the Operating Range Is Exceeded]

To move the robot while a hardware limit switch is triggered, follow the conditions and sequence below:

A) Enter **System Mode** from **Manual Mode**.  
B) Hold the **Enabling Switch** on the teach pendant.  

『Manual Mode』 + 『System』 + 『TP Enabling Switch ON』  

C) Turn **Motor ON** in this state.  
D) Use the **Jog Keys** to move the robot back into the operating range.

### (2) Error Occurs Even When the Operating Range Is Not Exceeded

First, check on the teach pendant’s dedicated input signal window whether the **Limit (Over-Travel)** item is continuously active. You can view this window by selecting **『Window Layout』 → 『Select』 → 『System Input』**. If the **Limit (Over-Travel)** item is highlighted in yellow, it indicates an error occurrence.

### [Caution]
- In **Manual Mode**, the **Enabling Switch** on the teach pendant must be ON for monitoring.  
- In **Automatic Mode**, monitoring occurs regardless of the enabling switch status.

![](../_assets/3-Safety-io/E00002/그림3.png)<br>
Figure 3.2.3. Over-Travel Monitoring in the System Input Window

In such cases, the cause can be traced to components related to the limit switch. The limit switch is connected to the controller’s servo safety system via the **CEC1 – CER1** cable from the robot body, as shown in the following figure.

![](../_assets/3-Safety-io/E00002/hw_limit_sw_wire_0_en.png)<br>
Figure 3.2.4. Hardware Limit Switch Wiring Structure

The main inspection points and sequence are as follows:  
A1) Servo Safety Board (CNSI1) **or**  
A2) Optional Safety IO Board (CNSI2)  
B) Internal wiring and connectors of the controller  
C) Wire harness and connectors  
D) Limit switch and robot body wiring  

At the appropriate location, jumper the input line of the limit switch and check whether the **Limit (Over-Travel)** item in the monitoring window changes to white.  
Proceed according to the following sequence.

### [How to Check from the Servo Safety Board Connector (CNSI1) or Optional Safety IO Board Connector (CNSI2)]

{% hint style="warning" %}
Always perform cable connection or disconnection **with the controller powered OFF**. Electrical hazards can cause personal injury or property damage.<br>
{% endhint %}

#### * How to Check the Servo Safety Board Connector (CNSI1)
This step determines whether the fault originates from the servo safety board via the CNSI1 connector. Jumper the pins related to the assigned input channel. Then, check the **Limit (Over-Travel)** item in the dedicated input signal monitoring window.

1. If the indicator changes to **white**, the servo safety board is faulty. Replace the board.
2. If it remains **yellow** (error state), check for faults along the path from the servo safety board to the hardware limit switch on the robot.

The figure below shows an example of jumper shorting when the limit switch is assigned to channel 1. Perform the test by connecting the jumper to the actually assigned channel.

![](../_assets/3-Safety-io/E00002/bd642_cnsi1_short.png)<br>
Figure 3.2.5. Servo Safety Board Connector (CNSI1)

#### * How to Check the Option Safety IO Board Connector (CNSI2)
This step determines whether the fault originates from the option safety IO board via the CNSI2 connector. Jumper the pins related to the assigned input channel. Then, check the **Limit (Over-Travel)** item in the dedicated input signal monitoring window.

1. If the indicator changes to **white**, the option safety IO board is faulty. Replace the board.
2. If it remains **yellow** (error state), check for faults along the path from the option safety IO board to the hardware limit switch on the robot.

The figure below shows an example of jumper shorting when the limit switch is assigned to channel 3. Perform the test by connecting the jumper to the actually assigned channel.

![](../_assets/3-Safety-io/E00002/bd680_si_short.png)<br>
Figure 3.2.6. Hardware Limit Switch Wiring Structure

### [How to Check the Wire Harness (C(M)ER1 or C(M)EC1)]

{% hint style="warning" %}<br>
Always turn off the controller power before connecting or disconnecting cables. Electrical hazards may cause personal injury or property damage.<br>
{% endhint %}

This step determines whether the fault originates from the wire harness via the C(M)ER1 or C(M)EC1 connector. First, remove the C(M)EC1 wire harness from the controller. Then, jumper the pins related to the limit switch on the C(M)EC1 connector attached to the controller. Check the **Limit (Over-Travel)** item in the dedicated input signal monitoring window to verify the signal.

① If the color changes to **white**,  
the fault lies in the cable or connector between the C(M)EC1 connector inside the controller and the system board. Inspect or replace the cable/connector as needed.  

② If the color remains **yellow**,  
check for faults in the area from the C(M)EC1 connector to the hardware limit switch on the robot body.  

Reconnect the C(M)EC1 wire harness and remove the C(M)ER1 wire harness from the robot body. Then, jumper the pins related to the limit switch on the C(M)ER1 connector of the wire harness.  
Check the **Limit (Over-Travel)** item in the dedicated input signal monitoring window.  

① If the color changes to **white**,  
the fault lies in the wire harness cable or connectors between the C(M)ER1 and C(M)EC1 connectors. Inspect or replace as necessary.  

② If the color remains **yellow**,  
check for faults in the area from the C(M)ER1 connector on the robot body to the limit switch.

### [How to Inspect the Limit Switch (SW) and Internal Wiring of the Robot Body]

{% hint style="warning" %}<br>
Always ensure the controller power is **OFF** before connecting or disconnecting any cables. Electrical hazards can cause personal injury or property damage.<br>
{% endhint %}

After disconnecting the CER1 wire harness from the robot body, use a multimeter to perform a continuity test on the lines related to the limit switch at the CER1 connector on the robot body.

① If the resistance measures **open**,  
there is a fault in the limit switch or the connector/cable between the limit switch and CER1. Inspect or replace as needed.  

② If the resistance measures **short**,  
check other sections for faults. Contact the manufacturer for further guidance.

![](../_assets/3-Safety-io/E00002/그림8_en.png)<br>
Figure 3.2.7. Hardware Limit Switch (SW) Harness C(M)ER Structure

### (3) If there is a fault in the Primary Axis limit switch circuit wiring or contacts

To inspect the Primary Axis limit switch wiring, first check which input channel the Primary Axis limit switch is assigned to via the **Safety I/O Assignment** function.  
By default, the Primary Axis limit switch is **disabled**, so inspection is not required.  
If use is needed, you can assign it through the **Safety I/O Assignment** function by selecting one of the following: 1) Basic Safety, 2) Additional Safety, or 3) Safety Communication.

#### 3-1) Assigned to Basic Safety Input

If the Primary Axis limit switch input is assigned to the **Basic Safety Input**, it is connected to the **CNSI1 connector (4 channels) on the Servo Safety Board**.  
Check which channel is assigned on the CNSI1 connector as described in item (1). For detailed pin mapping of this connector, refer to section 4.3.2.6 of the Hi7 Controller Maintenance Manual.

#### 3-2) Assigned to Additional Safety Input

If the Primary Axis limit switch input is assigned to the **Additional Safety Input**, it is connected to the **CNSI2 connector (8 channels) on the Optional Safety I/O Board**.  
Check which channel is assigned on the CNSI2 connector as described in item (1). For detailed pin mapping of this connector, refer to section 5.4.6 of the Hi7 Controller Maintenance Manual.

#### 3-3) Assigned to Safety Communication Input

If the Primary Axis limit switch input is assigned to the **Safety Communication Input**, refer to the **Hi7 Robot Controller Function Manual – Industrial Communication** for details.

### (4) If the Primary Axis Limit Switch Safety Input Assignment is Not Configured

If the external emergency stop input is not selected in the safety input assignment, activate the external E-Stop function by selecting one of the following options:

- **Basic Safety Input**  
- **Extended Safety Input**  
- **Safety Communication Input**  

The Safety Input Assignment can be configured via the following menu:

`System -> 8: Safety System -> 2: Parameter Setting -> 3: Safety I/O -> 1: Input/Output Assignment`  

![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)  
Figure 3.2.8. T/P screen: Safety Input/Output Assignment


[__SOURCE](3-safety-board-part/E02310.md)
## 3.3. E02310 Automatic Mode Safety Guard Switch Activated

### 1. Overview
A safety guard signal in automatic mode has been detected.<br>
In automatic mode, to ensure safety, all robot motions are immediately stopped, and the servo motors are switched to Motor OFF status.<br>

### 2. Causes and Checks
{% hint style="info" %}<br>
(1) The automatic mode safety guard signal was actually activated.<br>
(2) A wiring or contact issue occurred in the automatic mode safety guard circuit.<br>
(3) The safety input assignment for the automatic mode safety guard signal is not configured.<br>
{% endhint %}

### (1) When the Automatic Mode Safety Guard Signal is Actually Activated
Check whether the automatic mode safety guard (SGA) switch was actually triggered.  
Another operator or supervisor may have activated the automatic mode safety guard (SGA) switch.<br>
Also, verify that no personnel are inside the safety fence and check for potential hazards (tools, jigs, etc.) around the robot.  
If it is determined to be safe to restart the robot, release the external emergency stop button and operate the robot first in manual mode.

### (2) If There is a Wiring or Contact Issue in the Automatic Mode Safety Guard Circuit
To inspect the wiring related to the automatic mode safety guard, first check which input channel the automatic mode safety guard input is assigned to via the [Safety I/O Assignment] function.  
By default, the automatic mode safety guard input is assigned to channel 2 of the Basic Safety Input.

System -> 8: Safety System -> 2: Parameter Setting -> 3: Safety I/O -> 1: Safety I/O Assignment<br>
![](../_assets/3-Safety-io/E02310/io_alloc_param1.png)<br>
Figure 3.3.1. T/P screen showing the Safety I/O Assignment


#### 2-1) If Assigned to Basic Safety Input
If the automatic mode safety guard input is assigned to the Basic Safety Input, it is connected to the Servo Safety Board CNSI1 connector (4-channel). For a detailed pin map of this connector, refer to Section 4.3.2.6 of the Hi7 Controller Maintenance Manual.  
![](../_assets/3-Safety-io/E02310/bd642_cnsi1_position.png)<br>
Figure 3.3.2. Location of Servo Safety Board CNSI1 on Hi7-N Controller

Check which channel the automatic mode safety guard input is assigned to. Input channel assignments can be verified on the T/P screen shown in the Safety I/O Assignment section above.  
Once the assigned input channel is confirmed, refer to the site’s electrical diagram or wiring diagram to verify proper wiring. While checking the actual wiring, also confirm connector and assembly conditions.  

When reviewing the electrical diagram or wiring diagram, refer to Section 4.3.2.6 of the Hi7 Controller Maintenance Manual for the standard wiring of the Servo Safety Board CNSI1.

#### 2-2) If Assigned to Extended Safety Input  
If the automatic mode safety guard input is assigned to the extended safety input, it is connected to the CNSI2 connector (8 channels) of the Option Safety IO Board. For detailed pin mapping of this connector, refer to Section 5.4.6 of the Hi7 Controller Maintenance Manual.

![](../_assets/3-Safety-io/E02310/bd680_cnsi2_position.png)<br>
Figure 3.3.3. Position of the CNSI2 connector on the Hi7-N Controller Option Safety IO Board

Check which channel the automatic mode safety guard input is assigned to. The input channel assignment can be verified on the T/P screen in the Safety IO Allocation view, as shown in the figure above.<br>
Once the assigned input channel is confirmed, refer to the site electrical schematic or wiring diagram to ensure the wiring is correct. Additionally, inspect the actual wiring to verify proper connections and assembly.<br>
When checking the electrical schematic or wiring diagram, refer to Section 5.4.6 of the Hi7 Controller Maintenance Manual for the standard wiring of the Option Safety IO Board CNSI2.

#### 2-3) If assigned to Safety Communication Input  
If the external emergency stop input is assigned to a Safety Communication Input, refer to the "Hi7 Robot Controller Function Manual – Industrial Communication" for details.

### (3) If the Safety Input Assignment for the Automatic Mode Safety Guard Signal is Not Configured
If the automatic mode safety guard input has not been selected in the safety input assignment, activate the automatic mode safety guard function by selecting one of the following options:<br>
- Basic Safety Input  
- Extended Safety Input  
- Safety Communication Input<br>

The safety input assignment can be configured through the following menu:

System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety IO -> 1: Input/Output Assignment  
![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)<br>
Figure 3.3.4. T/P screen – Safety Input/Output Assignment

[__SOURCE](3-safety-board-part/E02320.md)
## 3.4. E02320 General Safety Guard Switch Activated

### 1. Overview
A general safety guard signal has been received.<br>
To ensure safety, all robot motion is immediately stopped, and the servo motors are switched to Motor OFF state.

### 2. Causes and Checks
{% hint style="info" %}<br>
(1) The general safety guard signal was actually triggered.<br>
(2) Abnormalities in the wiring or contacts of the general safety guard circuit.<br>
(3) The general safety guard signal has not been assigned to a safety input.<br>
{% endhint %}

### (1) If the general safety guard signal was actually triggered
Check whether the general safety guard (SGG) switch was physically activated. Another operator or manager may have triggered the general safety guard (SGG) switch.<br>
Also, since someone might be working inside the safety fence, check if any personnel are near the robot or if there are any potential hazards (tools, jigs, etc.).<br>
If it is judged safe to restart the robot, release the external emergency stop button and operate the robot in manual mode first.

### (2) If there is an abnormality in the wiring or contacts of the general safety guard circuit
To inspect the wiring related to the general safety guard, first check which input channel the general safety guard signal is assigned to using the [Safety I/O Allocation] function.<br>
By default, the general safety guard input is assigned to the basic safety input.

System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety I/O -> 1: Safety I/O Allocation<br>
![](../_assets/3-Safety-io/N00088/base_add_comm_si_func_sel.png)<br>
Figure 3.4.1. T/P screen – Safety I/O Allocation

#### 2-1) If assigned to Basic Safety Input
If the general safety guard (SGG) switch input is assigned to the basic safety input, it is connected to the servo safety board CNSI1 connector (4 channels). Refer to section 4.3.2.6 of the Hi7 controller maintenance manual for the detailed pin map of this connector.

![](../_assets/3-Safety-io/E02320/bd642_cnsi1_position.png)<br>
Figure 3.4.2. Hi7-N Controller – Servo Safety Board CNSI1 Location

Check which channel the general safety guard (SGG) switch input is assigned to. The input channel assignment can be confirmed in the T/P screen shown above in the Safety I/O Allocation.

Once the assigned input channel is confirmed, refer to the site’s electrical schematics or wiring diagrams to verify proper wiring. Additionally, physically inspect the wiring for proper connection and assembly.

When checking the electrical schematics or wiring diagrams, refer to section 4.3.2.6 of the Hi7 controller maintenance manual for the wiring standard of the servo safety board CNSI1.

#### 2-2) When Assigned to Extended Safety Input

If the general safety guard (SGG) switch input is assigned to the extended safety input, it is connected to the option Safety I/O board CNSI2 connector (8 channels). Refer to section 5.4.6 of the Hi7 Controller Maintenance Manual for the detailed pinout of this connector.

![](../_assets/3-Safety-io/E02320/bd680_cnsi2_position.png)<br>
Figure 3.4.3. Hi7-N Controller – Option Safety I/O Board CNSI2 Location

Check which channel the general safety guard (SGG) switch input is assigned to. The input channel assignment can be confirmed in the T/P screen shown above in the Safety I/O Allocation.

Once the assigned input channel is confirmed, refer to the site’s electrical schematics or wiring diagrams to verify proper wiring. Additionally, physically inspect the wiring for proper connection and assembly.

When checking the electrical schematics or wiring diagrams, refer to section 5.4.6 of the Hi7 Controller Maintenance Manual for the wiring standard of the option Safety I/O board CNSI2.

#### 2-3) When Assigned to Safety Communication Input
If the external emergency stop input is assigned to the safety communication input, refer to the "Hi7 Robot Controller Function Manual – Industrial Communication" for details.

### (3) When Safety Input Assignment for the General Safety Guard Signal Is Not Configured
If the general safety guard input is not selected in the safety input assignment, activate the general safety guard function by selecting one of the following options:<br>
- Basic Safety Input  
- Extended Safety Input  
- Safety Communication Input<br>

The safety input assignment can be configured via the following menu:<br>

System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety I/O -> 1: I/O Allocation<br>
![](../_assets/3-Safety-io/N00088/base_add_comm_si_func_sel.png)<br>
Figure 3.4.4. T/P Screen – Safety I/O Allocation

[__SOURCE](3-safety-board-part/E51431.md)
## 3.5. E51431 (A ch) Abnormal Feedback of Magnetic Contactor

### 1. Overview
The magnetic contactor (MC) did not operate as expected.

### 2. Cause and Inspection

{% hint style="info" %}
(1) Check the monitoring system.<br>
(2) Inspect the magnetic contactor (MC).<br>
(3) Inspect the electrical board.<br>
(4) Check the power supply module (H6PSM30).<br>
(5) Inspect the servo amplifier.<br>
{% endhint %}

### (1) Check the Monitoring System
Verify the cabling between the electrical module where the magnetic contactor is installed (PSM or PDM) and the servo safety board that collects monitoring signals.  
The cable names are CNPRC and CNPRC1. The servo safety board signals enter the electrical module through the backplane board. Check the connector connections of this cable.

![](../_assets/3-Safety-io/E51431/cnprc_cable.png)<br>
Figure 3.5.1 Hi7-N Controller

### (2) Inspect the Magnetic Contactor (MC)
Check whether the magnetic contactors MC1 and MC2 inside the electrical module are operating properly.

![](../_assets/3-Safety-io/E51431/psm_mc1_mc2.png)<br>
Figure 3.5.2 Hi7-N Controller (Magnetic contactors MC1 and MC2 installed inside the electrical module)

### (3) Inspect the Electrical Board

Check or replace the electrical board and cable wiring that relay signals between the servo safety board and the magnetic contactors, as issues may exist.

![](../_assets/3-Safety-io/E51431/psm_inner_cables.png)<br>
Figure 3.5.3 Hi7-N Controller (Electrical board installed inside the electrical module)

### (4) Test by Replacing the Servo Safety Board

If the error does not occur after replacing the servo safety board, it can be concluded that the issue lies in the electronic contactor control or feedback section of the servo safety board.

![](../_assets/3-Safety-io/E51431/hi7_controller_bd642.png)<br>
Figure 3.5.4 Hi7-N Controller Servo Safety Board Replacement

[__SOURCE](3-safety-board-part/E52042.md)
## 3.6. E52042 (0 ch) Safety Input Signal Mismatch

{% hint style="warning" %}
When checking the safety input wiring, always ensure that the controller power is **OFF** before performing the inspection.
{% endhint %}

### 1. Overview

A mismatch has been detected between the redundant safety input signals on the basic safety input channel.  
To ensure safety, the affected input signal is treated as **Fail-Safe (Open or 0)**.

### 2. Causes and Inspection

{% hint style="info" %}
(1) Signal differences caused by wiring errors or disconnections  
(2) Noise caused by terminal blocks or cable conditions  
(3) Incorrect safety signal parameters (filter settings, allowed mismatch time)
{% endhint %}

### (1) Signal Differences Caused by Wiring Errors or Disconnections

A safety input signal mismatch indicates a discrepancy between the safety input signals connected to the Servo Safety Board CNSI1 connector (total 4 channels).  
For detailed pin mapping of this connector, refer to **Hi7 Controller Maintenance Manual, Section 4.3.2.6**.

![](../_assets/3-Safety-io/E52042/bd642_cnsi1_position.png)<br>
Figure 3.6.1. Hi7-N Controller Servo Safety Board CNSI1 Position

1) When the safety input signal is not used  
If the error occurs on a channel that is not in use, verify that the external wiring is as shown below. Also, check that the connector and wires are properly assembled and making good contact.

![](../_assets/3-Safety-io/E52042/bd642_cnsi1_notused.png)<br>
Figure 3.6.2. Wiring Diagram for Unused Servo Safety Board CNSI1 Channel
<br>

2) When the safety input signal is in use  
If the error occurs on a channel that is being used, first check which input channel the signal is assigned to. Input channel assignments can be verified through the following menu:

<br>
System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety IO -> 1: Input/Output Assignment

![](../_assets/3-Safety-io/E52042/io_alloc_param1.png)<br>
Figure 3.6.3. T/P Screen – Safety Input Assignment

Once the input channel assignment is confirmed, refer to the site’s electrical schematics or wiring diagrams to ensure proper wiring. Also, inspect the actual wiring for correct connections and assembly.  
For wiring standards of the Servo Safety Board CNSI1, refer to **Hi7 Controller Maintenance Manual, Section 4.3.2.6**.

### (2) Noise caused by terminal blocks or cable condition

#### Safety Input Signal Monitoring Function  
A monitoring screen for safety input signals is available on the T/P. It can monitor at 0.5-second intervals, allowing for basic verification.

System -> 8: Safety System -> 3: Monitoring -> 3: Safety IO Status  
![](../_assets/3-Safety-io/E52042/safety_io_status.png)<br>
Figure 3.6.4. T/P Screen – Safety IO Monitoring

### (3) Safety Signal Parameter Setting Error (Filter, Mismatch Allow Time)

If the filter time for the safety input signal is too short, or the allowed mismatch time is set excessively short, safety input signal mismatch alarms may occur frequently.  
The recommended default settings for safety input signals are as follows. These values can be adjusted according to the field environment and application conditions.

- Filter Time: 100 (msec)  
- Allowed Mismatch Time: 1000 (msec)  

System -> 8: Safety System -> 2: Parameter Setting -> 3: Safety IO -> 2: Basic IO  
![](../_assets/3-Safety-io/E52042/def_input.png)<br>
Figure 3.6.5. T/P Screen – Basic IO Settings

[__SOURCE](3-safety-board-part/E52043.md)
## 3.7. E52043 (0 ch) Additional Safety Input Signal Mismatch

{% hint style="warning" %}
When checking the wiring of Additional safety inputs, ensure that the controller power is **OFF** before performing any verification work.
{% endhint %}

### 1. Overview

A mismatch has been detected between the redundant signals of the Additional safety input channel.  
To ensure safety, the affected input signal is treated in a **Fail-Safe state (Open or 0)**.

### 2. Causes and Inspection

{% hint style="info" %}
(1) Signal differences due to wiring errors or disconnections  
(2) Noise caused by terminal blocks or cable conditions  
(3) Safety signal parameter setting errors (filter, allowed mismatch time)
{% endhint %}

### (1) Signal Differences Due to Wiring Errors or Disconnections

The Additional safety input signal mismatch indicates a discrepancy in the Additional safety input signals connected to the Option Safety IO Board CNSI2 connector (total 8 channels).  
For detailed pin assignments of this connector, refer to **Hi7 Controller Maintenance Manual, Section 5.4.6**.

![](../_assets/3-Safety-io/E52043/bd680_cnsi2_position.png)<br>
**Figure 3.7.1. Hi7-N Controller Option Safety IO Board CNSI2 Location**

1) When using the Additional safety input signal  
If the error occurs on a channel that is in use, verify which input channel the signal is assigned to. Assignment of Additional safety input channels can be checked through the following menu:

System -> 8: Safety System -> 2: Parameter Setting -> 3: Safety IO -> 1: Input/Output Assignment -> Additional Input <br>

![](../_assets/3-Safety-io/E52043/add_si_func_sel.png)<br>
**Figure 3.7.2. T/P Screen – Additional Safety Input/Output Assignment**

Once the Additional safety input channel assignment is confirmed, refer to the site’s electrical schematic or wiring diagram to verify that the actual wiring matches the design.  
Also, check the physical wiring for proper connection and assembly status.  

When verifying the electrical schematic or wiring diagram, follow the wiring standards for the Option Safety IO Board CNSI2 as specified in **Hi7 Controller Maintenance Manual, Section 5.4.6**.

### (2) Noise Caused by Terminal Blocks or Cable Conditions

#### Monitoring Function for Additional Safety Input Signals
A monitoring screen for the Additional safety input signals is provided on the T/P.  
Monitoring occurs every 0.5 seconds, allowing for basic verification.

**Navigation:**  
`System -> 8: Safety System -> 3: Monitoring -> 3: Safety IO Status`  

![](../_assets/3-Safety-io/E52043/add_si_monitoring.png)<br>
**Figure 3.7.3. T/P Screen – Safety IO Monitoring**

### (3) Incorrect Safety Signal Parameter Settings (Filter, Mismatch Allowance Time)

If the filter time for the Additional safety input signals is set too short or the mismatch allowance time is excessively short, alarms for Additional safety input signal mismatch may occur frequently.  

The recommended default settings for Additional safety input signals are as follows. These values can be adjusted depending on site conditions and application requirements:

- **Filter Time:** 100 (msec)  
- **Mismatch Allowance Time:** 1000 (msec)  

**Navigation:**  
`System -> 8: Safety System -> 2: Parameter Settings -> 3: Safety IO -> 3: Additional IO`  

![](../_assets/3-Safety-io/E52043/add_io.png)<br>
**Figure 3.7.4. T/P Screen – Additional Safety IO Settings**

[__SOURCE](4-servo-board-part/README.md)
# 4. Servo Safety Board (Servo Part)
[__SOURCE](4-servo-board-part/E02470.md)
## 4.1. E02470. (O Axis) Encoder Error: Reset Required

### 1. Overview

In order for the encoder to preserve the motor's position data, power must be supplied to the encoder at all times.

Power is supplied to the encoder by keeping the controller power ON or by an encoder backup battery. If the controller power is turned OFF while the encoder backup battery is discharged, an error occurs because the encoder loses its position data.

Similarly, when replacing a motor, the same error occurs because the encoder of the new motor has already been in a state where power was not supplied.

Since resetting the encoder changes the reference position data of the corresponding axis, you must move the robot to the reference posture through manual operation of the axis coordinate system and re-perform the encoder calibration for that axis.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder battery voltage.<br>
(2)	Inspect the encoder battery wiring status.<br>
(3)	Perform a motor replacement test.<br>
(4)	After resetting the encoder, encoder calibration must be re-performed at the robot's reference position.<br>

{% endhint %}

(1)	Check the encoder battery voltage.<br>
The encoder battery is 3.6V. If this voltage drops to 3.0V~3.2V, it is displayed as "W0104 ○ Axis Encoder Battery voltage low." The encoder battery should be replaced when this warning occurs. The encoder battery must be replaced while the controller power is ON. If the battery is replaced with a normal encoder battery in this state, the robot can continue to be used without any problems.

If the encoder battery replacement time is passed and the encoder battery voltage drops to 2.5V~3.0V, the error "E2470 Axis ○ Encoder Abnormality: Encoder Reset Required" occurs. When this error occurs, the encoder's position data has already been lost. After replacing the encoder battery and resetting the encoder, you must move the robot to the reference posture through manual operation of the axis coordinate system and re-perform the encoder calibration for that axis.

![](../_assets/4.서보보드/battery_replace_position.png)<br>
Figure 4.1.1 Encoder Battery Replacement Position

Encoder reset is executed in the menu below.

    System -> 5. Initialization -> 4. Serial Encoder Reset

![](../_assets/4.서보보드/enc_reset.png)<br>
Figure 4.1.2 Serial Encoder Reset

(2)	Inspect the encoder battery wiring status.<br>
Check the battery wiring status connecting from the encoder battery location to the motor.

(3)	Perform a motor replacement test.<br>
If the problem is not resolved by the above measures, it is highly likely that the encoder itself is faulty. Perform a motor replacement test.

    

[__SOURCE](4-servo-board-part/E02670.md)
## 4.2. E02670. (O Axis) command value abnormal

### 1. Overview

Errors may occur due to communication abnormalities between the main board and the servo safety board or due to abrupt motion changes.<br> 
If a communication problem between boards occurs, normal commands cannot be transmitted from the main board to the servo safety board. At this time, since the robot may operate abnormally due to incorrect commands, an error is generated and the robot is stopped.<br>
In addition, in the case of abrupt motion, the drive unit may fail to follow the position command, so an error is generated and the robot is stopped.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the main board and servo safety board are installed correctly.<br>
* Check if the boards are installed correctly.<br>
* Check the boards for abnormalities.<br>

(2)	Check if there is a job program where the robot moves abruptly.<br>

{% endhint %}


(1)	Check if the main board and servo safety board are installed correctly.

If the main board and servo safety board are not correctly installed in the rack or if there is a problem with the boards, communication problems may occur, resulting in an error.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**To protect previous job programs, make sure to back up all files on the main board using a USB memory before removing the board from the rack.**

</div>

---

The method for backing up main board files to a USB memory is as follows.

![](../_assets/4.서보보드/USB_connector.png)<br>
Figure 4.2.1 TP USB Connection

When the USB is recognized by the TP, it is displayed as the following icon at the top of the screen.

![](../_assets/4.서보보드/usb.png)<br>
Figure 4.2.2 TP USB Recognition

Enter the following path to back up files.

    Service -> 5. File Manager

![](../_assets/4.서보보드/filemanage.png)<br>
Figure 4.2.3 Backup Step 1

![](../_assets/4.서보보드/filemanage2.png)<br>
Figure 4.2.4 Backup Step 2

Copy the Project folder to the USB.

* Check if the board is installed correctly.<br>
Check the connection status of the EtherCAT cable, which is the interface between the boards. Please remove and reinstall it.

![](../_assets/4.서보보드/ethercat_cable_hicom_bd642_r1.png)<br>
Figure 4.2.5 N Controller EtherCAT Cable Connection

* Check the boards for abnormalities.<br>
Please replace the board to determine if the board is faulty.

(2)	Check if there is a job program where the robot moves abruptly.<br>
Check if the error occurs in a section where the motion changes abruptly during robot operation.
If the error occurs during abrupt motion, modification of the job program is required.<br>
The causes of errors occurring during abrupt motion are as follows. When executing a job program, there are cases where the robot's posture changes significantly while moving a short distance inevitably. At this time, the robot's axis speed suddenly increases, and if the servo board fails to follow this, an error occurs. The solution is to modify the teaching point at the point where the posture changes abruptly or change the robot posture.


[__SOURCE](4-servo-board-part/E02680.md)
## 4.3. E02680. (O Axis) Maximum Speed Exceeded

### 1. Overview

The robot axis operated at a speed exceeding the maximum speed. Since the robot is in a state where it is not controlled normally, it is treated as an error and the robot is stopped.

When sending commands from the main board to the servo safety board, limited commands are sent to ensure the maximum speed is not exceeded. A maximum speed exceeded error may occur when the robot fails to follow these generated commands and speed overshoot occurs.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the tool data is entered correctly.<br>
(2)	Check if the robot model is set correctly.<br>
(3)	Check the versions of the servo board (BD640) and main com.<br>
(4)	Check if the robot posture is near a singularity.<br>
(5)	For external axes, check the acceleration/deceleration parameter settings and the load factor during operation.<br>
(6)	Adjust the job program.<br>

{% endhint %}

(1)	Check if the tool data is entered correctly.<br>
If the tool weight or inertia differs significantly from the values registered in the controller, robot control performance may deteriorate, and a maximum speed exceeded error may occur. Tool weight and inertia can be registered according to the tool number in the menu below.

        System -> 3. Robot Parameter -> Tool Data

![](../_assets/4.서보보드/tool.png)<br>
Figure 4.3.1 Check Tool Data

To automatically set the tool weight or inertia, you can use the load estimation function in the menu below. 

* Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation Function

![](../_assets/4.서보보드/estimation1.png)<br>
Figure 4.3.2 Load Estimation Function 1

![](../_assets/4.서보보드/estimation2.png)<br>
Figure 4.3.3 Load Estimation Function 2

![](../_assets/4.서보보드/estimation3.png)<br>
Figure 4.3.4 Load Estimation Function 3

* Select the tool number to save after estimating the load using the load estimation function.

![](../_assets/4.서보보드/estimation4.png)<br>
Figure 4.3.5 Load Estimation Function 4

* Click Normal Operation to execute.<br>
Press the Motor On switch, hold the deadman switch, and then click Normal Operation.

![](../_assets/4.서보보드/estimation5.png)<br>
Figure 4.3.6 Load Estimation Function 5

* When the load estimation operation is completed, the estimation result is displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)<br>
Figure 4.3.7 Load Estimation Function 6

(2)	Check if the robot model is set correctly.

![](../_assets/4.서보보드/robot_model.png)<br>
Figure 4.3.8 Check Robot Model

Check if the robot model registered on the TP screen matches the actually installed robot.

(3)	Check the versions of the servo safety board (BD642) and main com.<br>
This may occur due to broken compatibility between the servo safety board (BD642) and the main com version. Especially if a module has been replaced, proceed with a version update to match the version of each module to the current main com version.

The version of each module can be checked in the path below.

        Service -> 7. System Diagnosis -> 1. System Version


![](../_assets/4.서보보드/version.png)<br>
Figure 4.3.9 Module Version Check

(4)	Check if the robot posture is near a singularity.<br>
If L interpolation or C interpolation, rather than PtP interpolation, is executed in a posture near a singularity, an error may occur. A singularity occurs when the B-axis is close to 0 deg and when the center of the wrist is close to the S-axis rotation center axis. When passing near a singularity, please change the corresponding step to PtP interpolation.

![](../_assets/4.서보보드/robot_special_action.png)<br>
Figure 4.3.10 Singularity Posture Check

(5)	For external axes, check the acceleration/deceleration parameter settings and the load factor during operation.<br>
The motor torque may be insufficient because the maximum speed of the external axis acceleration/deceleration parameter is too high or the acceleration time is too short. While observing the load factor during robot operation, you must lower the I/Ip maximum speed or significantly increase the acceleration time.

        System -> 3. Robot Parameter -> 34. Acc/Dec Parameter

![](../_assets/4.서보보드/acc.png)<br>
Figure 4.3.11 External Axis Acc/Dec Check

(6)	Adjust the job program.<br>
Change the step conditions of the corresponding step or the immediately preceding step in the job program. First, try changing it to “Acc=0”, second, try lowering the speed of the step, and third, try adding a step to the movement path to change the program conditions.


[__SOURCE](4-servo-board-part/E50101.md)
## 4.4. E50101. (O Axis) Invalid encoder command field setting

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the data received from the encoder does not comply with the specified communication standard.<br>

The above error may occur due to failure of components related to encoder data transmission and reception, wiring defects, or problems with encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	Inspect the encoder wiring.<br>
(3)	Perform a servo board replacement test.<br>
(4)	Perform a motor (encoder) replacement test.<br>
(5)	After completing the measures, check the communication status of the wiring.<br>

{% endhint %}

(1)	Check the encoder supply voltage.<br>
The power voltage supplied to the encoder must be within the range of 5.0V±5% (4.75V ~ 5.25V) at the encoder-side connector. If the encoder-side connector voltage drops below 4.75V, the encoder will not operate normally, and there is a possibility that the above error may occur.

Measure the voltage of the encoder-side connector pins (3-4).

![](../_assets/4.서보보드/encoder_connector_pin_info_en.png)<br>
Figure 4.4.1 Encoder Connector Pin Information

If the measured voltage is lower than the reference voltage, turn the VR1 variable resistor on the servo safety board (BD642) to adjust the encoder-side connector voltage so that it falls within the reference voltage range.

![](../_assets/4.서보보드/BD642_encoder_voltage_adjustment.png)<br>
Figure 4.4.2 BD642 Encoder Voltage Variable Resistor

(2)	Inspect the encoder wiring.
The inspection sequence for encoder wiring is as follows.<br>
1st: Check for poor contact in the connectors related to the encoder wiring.<br>
2nd: Check for short circuits in the encoder wiring. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester).<br>
3rd: Perform an encoder wiring replacement test.<br>

If there is no disconnection in the encoder wiring but issues such as poor contact of the shield wire or contact between the encoder signal wire and other power lines or metal parts of the robot body exist, these cannot be detected by a short circuit check. Therefore, perform a wiring replacement test.

* Check the internal wiring of the controller.<br>
Check the wiring between the CNEN13,46 (BD642) connector and CEC1.

![](../_assets/4.서보보드/hi7_controller_encoder_cable.png)<br>
Figure 4.4.3 Hi7-N Controller Encoder Wiring Inspection

* Check the wiring between the controller and the robot.<br>
In the case of the Hi7-N controller, check the wiring between CEC1 and CER1.

![](../_assets/4.서보보드/hi7_robot_encoder_cable.png)<br>
Figure 4.4.4 Basic Installation Configuration Diagram between Hi7-N Controller and Robot

![](../_assets/4.서보보드/hi7_robot_encoder_cable_detail.png)<br>
Figure 4.4.5 Detail of Basic Installation Configuration Diagram between Hi7-N Controller and Robot

* Check the internal wiring of the robot body.<br>
Check the wiring between CER1 and the encoder-side connector.
For wiring inspection, please refer to the wiring connection diagram in the robot maintenance manual.

![](../_assets/4.서보보드/robot_inner_cable.png)<br>
Figure 4.4.6 Robot Internal Wiring

(3)	Perform a servo safety board replacement test.<br>
If the error does not occur after replacing the servo safety board, the encoder receiving section of the servo safety board is faulty. Please replace the servo safety board with a normal unit.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.4.7 Hi7-N Controller Servo Board Replacement

(4)	Perform a motor (encoder) replacement test.<br>
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.4.8 Motor Positions for Each Axis of Robot

(5)	Check the communication status of the wiring after completing the measures.<br>
After the measures for the problematic part are completed, check the communication status by referring to the 『Encoder Communication Failure Count Display Function Manual』.

![](../_assets/4.서보보드/encoder_comm.png)<br>
Figure 4.4.9 Encoder Communication Failure Monitoring

![](../_assets/4.서보보드/encoder_comm_fail_number_en.png)


[__SOURCE](4-servo-board-part/E50102.md)
## 4.5. E50102. (O Axis) Encoder Received Data Length Abnormality

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the length of the data received from the encoder does not comply with the specified value.<br>

Cases where the length of data received from the encoder does not match can occur mainly when noise enters the encoder signal line due to wiring defects or problems with encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring.<br>
(2) Perform a motor (encoder) replacement test.<br>
(3)	Perform a servo safety board replacement test.<br>
(4)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

(1)	Inspect the encoder wiring.<br>
The inspection sequence for encoder wiring is as follows.<br>
1st: Check for poor contact in the connectors related to the encoder wiring.<br>
2nd: Check for short circuits in the encoder wiring. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester).<br>
3rd: Perform an encoder wiring replacement test.<br>

If there is no disconnection in the encoder wiring but issues such as poor contact of the shield wire or contact between the encoder signal wire and other power lines or metal parts of the robot body exist, these cannot be detected by a short circuit check. Therefore, perform a wiring replacement test.

* Check the internal wiring of the controller.<br>
Check the wiring between the CNEN13,46 (BD642) connector and CEC1.

![](../_assets/4.서보보드/hi7_controller_encoder_cable.png)<br>
Figure 4.5.1 Hi7-N Controller Encoder Wiring Inspection

* Check the wiring between the controller and the robot.<br>
In the case of the Hi7-N controller, check the wiring between CEC1 and CER1.

![](../_assets/4.서보보드/hi7_robot_encoder_cable.png)<br>
Figure 4.5.2 Basic Installation Configuration Diagram between Hi7-N Controller and Robot

![](../_assets/4.서보보드/hi7_robot_encoder_cable_detail.png)<br>
Figure 4.5.3 Detail of Basic Installation Configuration Diagram between Hi7-N Controller and Robot

* Check the internal wiring of the robot body.<br>
Check the wiring between CER1 and the encoder-side connector. For wiring inspection, please refer to the wiring connection diagram in the robot maintenance manual.

![](../_assets/4.서보보드/robot_inner_cable.png)<br>
Figure 4.5.4 Robot Internal Wiring

(2)	Perform a motor (encoder) replacement test.<br>
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.5.5 Motor Positions for Each Axis of Robot

(3)	Perform a servo safety board replacement test.<br>
If the error does not occur after replacing the servo safety board, the servo safety board is faulty. Please replace the servo safety board with a normal unit.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.5.6 N Controller Servo Safety Board Replacement

(4)	Check the communication status of the wiring after completing the measures.<br>
After the measures for the problematic part are completed, check the communication status by referring to the 『Encoder Communication Failure Count Display Function Manual』.

![](../_assets/4.서보보드/encoder_comm.png)<br>
Figure 4.5.7 Encoder Communication Failure Monitoring

![](../_assets/4.서보보드/encoder_comm_fail_number_en.png)


[__SOURCE](4-servo-board-part/E50103.md)
## 4.6. E50103. (O Axis) Invalid encoder data termination signal

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the signal indicating the end of the data frame (Ser_End) is not received from the encoder.<br>

Cases where the data frame end signal is not received from the encoder can occur mainly when noise enters the encoder signal line due to wiring defects or problems with encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring.<br>
(2)	Perform a motor (encoder) replacement test.<br>
(3)	Perform a servo safety board replacement test.<br>
(4)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".
[__SOURCE](4-servo-board-part/E50104.md)
## 4.7. E50104. (O Axis) CRC error deteced in encoder data

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the CRC value of the data received from the encoder does not match the CRC value calculated by the servo safety board.<br>

Cases where CRC errors occur in data received from the encoder can occur mainly when noise enters the encoder signal line due to wiring defects or problems with encoder shield line processing.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring.<br>
(2)	Perform a motor (encoder) replacement test.<br>
(3)	Perform a servo safety board replacement test.<br>
(4)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".

[__SOURCE](4-servo-board-part/E50105.md)
## 4.8. E50105. (O Axis) Encoder line open detected (Motor Off)

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when communication between the encoder and the servo safety board is unstable or when no signal is received at all.<br>
Cases where communication from the encoder to the servo safety board is unstable or signals are not received can occur mainly due to disconnection or poor contact of the encoder cable.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	Inspect the encoder wiring.<br>
(3)	Perform a servo board replacement test.<br>
(4)	Perform a motor (encoder) replacement test.<br>
(5)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".
[__SOURCE](4-servo-board-part/E50106.md)
## 4.9. E50106. (O Axis) Encoder data abnormal variation detected

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the position data received from the encoder fluctuates abnormally.<br>

Cases where the position data received from the encoder fluctuates abnormally can occur mainly when noise enters the encoder signal line due to wiring defects or problems with encoder shield line processing.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring.<br>
(2)	Perform a motor (encoder) replacement test.<br>
(3)	Perform a servo board replacement test.<br>
(4)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".
[__SOURCE](4-servo-board-part/E50107.md)
## 4.10. E50107. (O Axis) Encoder line open detected (Motor On)

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when communication between the encoder and the servo safety board is unstable or when no signal is received at all.<br>

Cases where communication between the encoder and the servo safety board is unstable or signals are not received can occur mainly due to disconnection or poor contact of the encoder cable.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	Inspect the encoder wiring.<br>
(3)	Perform a servo board replacement test.<br>
(4)	Perform a motor (encoder) replacement test.<br>
(5)	Check the communication status of the wiring after completing the measures.<br>

{% endhint %}

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".
[__SOURCE](4-servo-board-part/E50108.md)
## 4.11. E50108. (O Axis) Encoder Counting error (CE Bit Detected)

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when a rotation value calculation error occurs inside the encoder and the CE (Counter Error) bit is set.<br>
This error may occur when the data received from the encoder itself is normal, but the encoder internal status monitoring result determines it as an error state (CE).<br>

**CE (Counter Error)**: Set when a position misalignment occurs in the single-turn data due to malfunction or failure when the main power is applied to the encoder.


### 2. Cause and Inspection

{% hint style="info" %}

(1) Check the encoder supply voltage.<br>
(2) After resetting the serial encoder error, turn the controller power off and on again.<br>
(3) If the error persists, perform a motor (encoder) replacement test.<br>

{% endhint %}

(1) Check the encoder supply voltage.<br>
The power voltage supplied to the encoder must be within the range of 5.0V±5% (4.75V ~ 5.25V) at the encoder-side connector. If the voltage at the encoder-side connector drops below 4.75V, the encoder will not operate normally, and there is a possibility that the above error may occur.

Measure the voltage of the encoder-side connector pins (3-4).

![](../_assets/4.서보보드/encoder_connector_pin_info_en.png)<br>
Figure 4.11.1 Encoder Connector Pin Information

If the measured voltage is lower than the reference voltage, turn the VR1 variable resistor on the servo safety board (BD642) to adjust the encoder-side connector voltage so that it falls within the reference voltage range.

![](../_assets/4.서보보드/BD642_encoder_voltage_adjustment.png)<br>
Figure 4.11.2 BD642 Encoder Voltage Variable Resistor

(2) After resetting the serial encoder error, turn the controller power off and on again.<br>
If the error persists upon main power OFF/ON after resetting the error, perform a motor (encoder) replacement test.
Error reset is performed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Error Release

![](../_assets/4.서보보드/enc_error_clear.png)<br>
Figure 4.11.3 Serial Encoder Error Release

(3) If the error persists, perform a motor (encoder) replacement test.<br>
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.11.4 Motor Positions for Each Axis of Robot


[__SOURCE](4-servo-board-part/E50109.md)
## 4.12. E50109. (O Axis) Encoder Overspeed

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the encoder rotation speed exceeds the allowable range and the OS (OverSpeed) bit is set. This may be an actual overspeed condition or a false detection of overspeed due to signal abnormalities.<br>

This error may occur when the data received from the encoder itself is normal, but the encoder internal status monitoring result determines it as an error state (OS).

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	Inspect the encoder wiring.<br>
(3)	After resetting the serial encoder error, turn the controller power off and on again.<br>
(4)	If the error persists, perform a motor (encoder) replacement test. 

{% endhint %}

For detailed inspection methods, refer to "E50108 (O Axis) Encoder Counting error".

[__SOURCE](4-servo-board-part/E50110.md)
## 4.13. E50110. (O Axis) Encoder Full absolute status

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the Full Absolute status is not reached inside the encoder, meaning accurate position information has not yet been secured. This can occur immediately after encoder power-on due to data initialization failure or loss of backup information.<br>
This error may occur when the data received from the encoder itself is normal, but the encoder internal status monitoring result determines it as an error state (FS).<br>

**FS (Full Absolute)**: If this bit is 0, it means the position data has not been initialized or backup information is incomplete; if this bit is 1, it indicates that the encoder internal data is complete and in a normal state.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	After resetting the serial encoder error, turn the controller power off and on again.<br>
(3)	If the error persists, perform a motor (encoder) replacement test.<br>

{% endhint %}

For detailed inspection methods, refer to "E50108 (O Axis) Encoder Counting error".
[__SOURCE](4-servo-board-part/E50111.md)
## 4.14. E50111. (O Axis) Encoder Counting error (ME Bit Detected)

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the ME bit is set because the multi-turn (rotation count) data is not saved normally due to causes such as battery backup failure, internal storage circuit error, or unexpected power cutoff during operation.<br>

This error may occur when the data received from the encoder itself is normal, but the encoder internal status monitoring result determines it as an error state (ME).


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	After resetting the serial encoder error, turn the controller power off and on again.<br>
(3)	If the error persists, perform a motor (encoder) replacement test.<br>

{% endhint %}

For detailed inspection methods, refer to "E50108 (O Axis) Encoder Counting error".

[__SOURCE](4-servo-board-part/E50112.md)
## 4.15. E50112. (O Axis) Encoder Battery error

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.<br>
This error occurs when the BE (Battery Error) bit is set because the voltage of the battery connected to the encoder drops below the standard value or a problem occurs with the battery connection.<br>
This error may occur when the data received from the encoder itself is normal, but the encoder internal status monitoring result determines it as an error state (BE).

**BE (Battery Error)**: Set when the external battery voltage drops to 3.1V or lower while the encoder main power is Off.


### 2. Cause and Inspection

{% hint style="info" %}

(1) After resetting the serial encoder error, turn the controller power off and on again.<br>
(2) Check the encoder backup battery voltage.<br>
(3) Inspect the encoder battery connection status.<br>
(4) Perform a motor (encoder) replacement test.<br>

{% endhint %}

(1) After resetting the serial encoder error, turn the controller power off and on again.<br>
If the error persists upon main power OFF/ON after resetting the error, perform a motor (encoder) replacement test.
Error reset is performed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Error Release

![](../_assets/4.서보보드/enc_error_clear.png)<br>
Figure 4.15.1 Encoder Error Release

(2) Check the encoder battery voltage.<br>
The encoder battery is 3.6V. If this voltage drops to 3.0V~3.2V, “W0104 ○ Axis Encoder Battery Voltage Low” is displayed. When this warning occurs, the encoder battery must be replaced. Encoder battery replacement must be performed while the controller power is ON. If you replace it with a normal encoder battery in this state, you can continue to use the robot without any problems.

If the encoder battery replacement time is passed and the voltage drops to 2.5V~3.0V, the error “E2470 ○ Axis Encoder Abnormal: Encoder Reset Required” occurs when the controller power is turned ON. If this error occurs, the encoder position data has already been lost. After replacing the encoder battery and resetting the encoder, you must move the robot to the reference posture using manual operation in the axis coordinate system and perform encoder calibration for the corresponding axis again.

![](../_assets/4.서보보드/battery_replace_position.png)<br>
Figure 4.15.2 Encoder Battery Replacement Position

Encoder reset is performed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Encoder Reset

![](../_assets/4.서보보드/enc_reset.png)<br>
Figure 4.15.3 Encoder Reset

(3) Check the encoder battery connection status.<br>
Check the status of the battery wiring connecting from the encoder battery location to the motor.


(4) Perform a motor (encoder) replacement test.<br>
If the error persists upon main power OFF/ON after resetting the error, perform a motor (encoder) replacement test. If the error does not occur after replacement, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.15.4 Motor Positions for Each Axis of Robot


[__SOURCE](4-servo-board-part/E50113.md)
## 4.16. E50113. (O Axis) Encoder Overheat Detection (OH Bit Detection)

### 1. Overview

The servo safety board performs serial communication with the encoder for servo motor control and receives encoder data periodically.
This error occurs when the OH bit is detected from the encoder.<br>
The OH bit is set when the internal temperature of the encoder exceeds the allowable range. The threshold temperature is around 90 ℃ to 100 ℃, and since specifications vary depending on the encoder model, please check the manufacturer's manual.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Perform a motor (encoder) replacement test.<br>
(2)	Check the operating conditions (speed, load, etc.).<br>
(3)	Check the ambient temperature around the encoder.<br>
(4)	Replace the servo safety board (BD642).

{% endhint %}

(1)	Perform a motor (encoder) replacement test.<br>
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.16.1 Motor (Encoder) Replacement Position

(2)	Check the operating conditions (speed, load, etc.).<br>
Check the saturated encoder temperature while running the Job program. Encoder temperature can be checked as follows.

    Engineering Mode -> Window Adjustment -> System Characteristics -> System Characteristics List - Motor/Encoder

![](../_assets/4.서보보드/enc_tmp.png)<br>
Figure 4.16.2 Checking Encoder Temperature

(3)	Check the ambient temperature around the encoder.<br>
Errors may occur if the encoder's internal temperature rises due to the external temperature.

(4)	Perform a servo safety board replacement test.<br>
If the error does not occur after replacing the servo safety board, it can be determined that the encoder data receiving section of the servo board is faulty.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.16.3 N Controller Servo Board Replacement


[__SOURCE](4-servo-board-part/E50200.md)
## 4.17. E50200. (O Axis) Motor overload

### 1. Overview

This occurs when the motor current accumulates exceeding the set continuous rated current or overload judgment criteria during servo control.<br>
This can occur when excessive torque is required from the motor due to causes such as mechanical overload, increased friction, or excessive acceleration/deceleration conditions. The servo safety board detects this and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1) Check if the installed load is within the robot's rating.<br>
(2) Check if there are any collision factors during robot operation.<br>
(3) Check if the axis brake is operating normally.<br>
(4) Inspect the connection status of the motor cable and connector.<br>
(5) Replace the servo board to check for abnormalities.<br>
(6) Check if the drive unit is operating normally.<br>

{% endhint %}

(1) Check if the installed load is within the robot's rating.<br>
Confirm that the installed load is within the robot's maximum specifications. If the specifications are exceeded, an error may occur (here, "load" includes not only the tool installed at the robot end but also cables and all other parts attached to the robot mechanism).<br>
The most accurate way to check the load is to use a measuring instrument, but if that is not feasible, you can check using the load estimation function among the controller functions. The load estimation function can only estimate the tool installed at the robot end.

The load estimation method is as follows.

* Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation Function

![](../_assets/4.서보보드/estimation1.png)<br>
Figure 4.17.1 Load Estimation Function 1

![](../_assets/4.서보보드/estimation2.png)<br>
Figure 4.17.2 Load Estimation Function 2

![](../_assets/4.서보보드/estimation3.png)<br>
Figure 4.17.3 Load Estimation Function 3

* Select the tool number to save after estimating the load using the load estimation function.

![](../_assets/4.서보보드/estimation4.png)<br>
Figure 4.17.4 Load Estimation Function 4

* Click Normal Operation to execute.
Press the Motor On switch, hold the deadman switch, and then click Normal Operation.

![](../_assets/4.서보보드/estimation5.png)<br>
Figure 4.17.5 Load Estimation Function 5

* When the load estimation operation is completed, the estimation result is displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)<br>
Figure 4.17.6 Load Estimation Function 6

(2) Check if there are any collision factors during robot operation.<br>
Check if there is any interference or collision with the robot in the robot's workspace. If interference occurs between the robot and other mechanisms, an error may occur. In this case, modify the work program to prevent interference.

(3) Check if the brake release is operating normally.<br>
There may be a problem with the release function of the brake for the corresponding axis or an abnormality in the brake release voltage.
 * Inspection of individual axis brake release anomalies<br>
Use the Axis Lock function to verify the operation of the brake release function for the corresponding axis.
Lock the axes except for the axis you want to verify, then repeat Motor ON/OFF to check if the brake release sound ("click") is heard from the motor of the mechanical unit.

The method to use the Axis Lock function is as follows.<br>
        System -> 5. Initialization -> 9. Axis Lock Setting -> Confirm -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)<br>
Figure 4.17.7 Axis Lock Setting Screen 1

![](../_assets/4.서보보드/axis_lock2.png)<br>
Figure 4.17.8 Axis Lock Setting Screen 2

![](../_assets/4.서보보드/axis_lock3.png)<br>
Figure 4.17.9 Axis Lock Setting Screen 3

If the brake of the corresponding axis is not released, the brake output status of the servo board must be checked. Disconnect the brake wiring (CNBRK16, CNBRK78 connectors) and output the brake voltage. Measure whether the brake voltage of the corresponding axis is output as 20V or higher at the CNBRK16 and CNBRK78 connectors. If there is an axis outputting a voltage of 20V or lower, it is a failure of the servo safety board (BD642), so replace it.

![](../_assets/4.서보보드/bd642_brake_connector.png)<br>
Figure 4.17.10 Pin Layout of CNBRK16, CNBRK78 Connectors

* Inspection of Brake Power Supply Abnormalities<br>
The sequence for inspecting brake power wiring is as follows.<br>
1st: Check for poor contact in connectors related to brake power wiring.<br>
2nd: Check for short circuits in the brake power wiring. Check 1:1 using equipment such as a multimeter (tester).<br>
Inspect the internal wiring of the power electric module.<br>

![](../_assets/4.서보보드/psm_psbd.png)<br>
Figure 4.17.11 Power Electric Module and Power Board

* Check the servo safety board (BD642).<br>
If the power electric module is normal, measure the brake power (DC24V) on the servo safety board. It is normal if the measured value across the capacitor (EC9) or across the connector (J12) in the red area of the figure below is DC24V or higher. If it is less than 20V, there is a malfunction in the power supply device generating the brake power. Replace the electric module.

![](../_assets/4.서보보드/bd642_brake_power.png)<br>
Figure 4.17.12 Servo Safety Board Brake Power

(4) Inspect the connection status of the motor cable and connector.<br>
* Inspect the internal wiring of the controller.
* Inspect the wiring between the controller and the robot.
* Inspect the internal wiring of the robot.

(5) Replace the servo safety board to check for abnormalities.<br>
An error may occur if there is an abnormality in the servo safety board. Replace the board to verify.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.17.13 N Controller Servo Board Replacement

(6) Check if the drive unit is operating normally.<br>
Check if the drive unit (motor, reducer) of the corresponding axis is operating normally.

![](../_assets/4.서보보드/robot_axis_motor_brake.png)<br>
Figure 4.17.14 Verification of Normal Drive Unit Operation

[__SOURCE](4-servo-board-part/E50201.md)
## 4.18. E50201. (O Axis) Motor overload (Increased Friction Due to Low Temperature)

### 1. Overview

This occurs when the current flowing in the motor or drive unit exceeds the set continuous rated current criteria and is determined to be in an overload state.<br>
If an excessive load is applied to the motor during servo control, the servo safety board detects this as an error and stops the robot.

This error primarily occurs when there is an overload condition while the encoder temperature is low.<br>
Generally, in a low-temperature environment (encoder temperature 5 ℃ or lower), friction components increase due to increased grease viscosity, requiring a larger driving torque than in the normal state. If the robot is operated at high speed in this state, this error may occur.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Operate at low speed (playback speed 30% or less) until the encoder temperature reaches a normal level (approx. 15℃ or higher), then restart at normal speed. 

{% endhint %}

(1)	Operate at low speed (playback speed 30% or less) until the encoder temperature reaches a normal level (approx. 15℃ or higher), then restart at normal speed.

![](../_assets/4.서보보드/enc_tmp2.png)<br>
Figure 4.18.1 Encoder Temperature Check Screen

[__SOURCE](4-servo-board-part/E50205.md)
## 4.19. E50205. (O Axis) Unable to sustain servo lock – abnormal current output

### 1. Overview

This occurs when the current required for the motor or drive unit is not applied normally.<br>
It can be caused by poor wiring between the motor and the controller, or failures in the current command and feedback circuits.<br>
It can also occur when parameters required for motor control (gain, maximum current, etc.) do not match the actual motor specifications due to a robot model registration error.

### 2. Cause and Inspection

{% hint style="info" %}

(1) Check if the robot model is set correctly.<br>
(2) Inspect the motor power line and encoder communication line.<br>
* Check the wiring connecting the robot and the controller.
* Check the internal wiring of the robot.
* Check the internal wiring of the controller.

(3) Inspect the cable or connection connector between the servo safety board and the amplifier board inside the controller.<br>
(4) Replace other components.<br>

{% endhint %}

(1)	Check if the robot model is set correctly.<br>
Check if the registered robot model on the TP screen matches the actually installed robot.

![](../_assets/4.서보보드/robot_model.png)<br>
Figure 4.19.1 Robot Model Check

(2)	Inspect the motor power and encoder communication lines.<br>
Turn off the controller power, disconnect U, V, W of the corresponding axis drive unit, and check for short circuits or open circuits in each phase. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester). Check for disconnection of the encoder communication line.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**Be careful as there is a risk of electric shock when inspecting while the power is on.**

</div>

---

* Check the wiring connecting the robot and the controller.
Disconnect the wiring connecting the controller and the robot or drive unit, and check if each phase (U phase, V phase, W phase) is shorted to each other or to ground. If any short circuit is found, the corresponding wiring must be replaced.

![](../_assets/4.서보보드/hi7_robot_power_cable.png)<br>
Figure 4.19.2 Wiring between N Controller and Robot

* Inspect the internal wiring of the robot.<br>
It is necessary to check if there are any short circuits or incorrect wiring in the wiring connected to the motor inside the robot.

![](../_assets/4.서보보드/robot_inner_cable.png)<br>
Figure 4.19.3 Robot Internal Wiring

* Inspect the internal wiring of the controller.<br>
It is necessary to inspect the wiring installed with the amplifier inside the controller.

![](../_assets/4.서보보드/hi7_brake_cable.png)<br>
Figure 4.19.4 N Controller Internal Wiring Inspection

(2)	Inspect the connector (Board to Board) between the servo safety board and the amplifier board inside the controller.<br>
Check if the installation of the connector (Board to Board) connecting and fastening the servo safety board and the amplifier board is correct. If the fastening status is poor, this error may occur.

![](../_assets/4.서보보드/conncet_bd642_amp.png)<br>
Figure 4.19.5 Connection between Hi7-N Controller Servo Board and Amplifier Board

(3)	Replace other components.<br>
Replace components in the order of Servo Safety Board (BD642) → Amplifier Board → Wire Harness → Motor → PSM to check for error occurrence.

![](../_assets/4.서보보드/hi7_robot_brake_power_check.png)<br>
Figure 4.19.6 N Controller Drive Components

[__SOURCE](4-servo-board-part/E50206.md)
## 4.20. E50206. (O Axis) Unable to sustain servo lock – abnormal parameter

### 1. Overview

This occurs when the current required for the motor or drive unit is not applied normally.<br>
It can be caused by poor wiring between the motor and the controller, or failures in the current command and feedback circuits.<br>
It can also occur when parameters required for motor control (gain, maximum current, etc.) do not match the actual motor specifications due to a robot model registration error.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the robot model is set correctly.<br>
(2)	Inspect the motor power line and encoder communication line.<br>
* Check the wiring connecting the robot and the controller.
* Check the internal wiring of the robot.
* Check the internal wiring of the controller.

(3) Inspect the cable between the servo board and the amplifier board inside the controller.<br>
(4) Replace other components.<br>

{% endhint %}

(1)	Check if the robot model is set correctly.<br>
Check if the registered robot model on the TP screen matches the actually installed robot.

![](../_assets/4.서보보드/robot_model.png)<br>
Figure 4.20.1 Robot Model Check

(2)	Inspect the motor power and encoder communication lines.<br>
Turn off the controller power, disconnect U, V, W of the corresponding axis drive unit, and check for short circuits or open circuits in each phase. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester). Check for disconnection of the encoder communication line.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**Be careful as there is a risk of electric shock when inspecting while the power is on.**

</div>

---

* Check the wiring connecting the robot and the controller.<br>
Disconnect the wiring connecting the controller and the robot or drive unit, and check if each phase (U phase, V phase, W phase) is shorted to each other or to ground. If any short circuit is found, the corresponding wiring must be replaced.

![](../_assets/4.서보보드/hi7_robot_power_cable.png)<br>
Figure 4.20.2 Wiring between N Controller and Robot

* Inspect the internal wiring of the robot.<br>
It is necessary to check if there are any short circuits or incorrect wiring in the wiring connected to the motor inside the robot.

![](../_assets/4.서보보드/robot_inner_cable.png)<br>
Figure 4.20.3 Robot Internal Wiring

* Inspect the internal wiring of the controller.<br>
It is necessary to inspect the wiring installed with the amplifier inside the controller.

![](../_assets/4.서보보드/hi7_brake_cable.png)<br>
Figure 4.20.4 Hi7-N Controller Internal Wiring Inspection

(2)	Inspect the connector (Board to Board) between the servo board and the amplifier board inside the controller.<br>
Check if the installation of the connector (Board to Board) connecting and fastening the servo safety board and the amplifier board is correct. If the fastening status is poor, this error may occur.

![](../_assets/4.서보보드/conncet_bd642_amp.png)<br>
Figure 4.20.5 Connection between N Controller Servo Board and Amplifier Board

(3)	Replace other components.<br>
Replace components in the order of Servo Safety Board (BD642) → Amplifier Board → Wire Harness → Motor → PSM to check for error occurrence.

![](../_assets/4.서보보드/hi7_robot_brake_power_check.png)<br>
Figure 4.20.6 Hi7-N Controller Drive Components



[__SOURCE](4-servo-board-part/E50400.md)
## 4.21. E50400. (O Axis) Position Deviation exceeded

### 1. Overview

This occurs when the position deviation exceeds the set value during robot operation.<br>
While the robot is operating under servo control, if the difference between the movement command position and the actual position exceeds the allowable range, the servo board detects this as an error and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the axis where the error occurred has mechanical interference with other equipment.<br>
(2)	Check if the robot model is set correctly.<br>
(3)	Check if the brake release is operating normally.<br>
* Inspection of individual axis brake release anomalies.
* Inspection of brake power supply abnormalities.

(4)	Inspect the wiring status.<br>
(5)	Check if the rated load is being used.<br>
(6)	Check the position deviation setting level.<br>
(7)	Check the versions of the servo safety board (BD642) and the main com.<br>
(8)	Replace other components.<br>

{% endhint %}

(1) Check if the axis where the error occurred has mechanical interference with other equipment.<br>
This error may occur if there is mechanical interference or collision involving the robot. If the robot is outside the restricted area, you must move it to a safe area using manual operation.

(2) Check if the robot model is set correctly.<br>

![](../_assets/4.서보보드/robot_model.png)<br>
Figure 4.21.1 TP Robot Model Check

Check if the registered robot model on the TP screen matches the actually installed robot.

(3) Check if the brake release is operating normally.<br>
There may be a problem with the release function of the brake for the corresponding axis or an abnormality in the brake release voltage.

* Inspection of individual axis brake release anomalies<br>
Use the Axis Lock function to verify the operation of the brake release function for the corresponding axis.
Lock the axes except for the axis you want to verify, then repeat Motor ON/OFF to check if the brake release sound ("click") is heard from the motor of the mechanical unit.<br>
The method to use the Axis Lock function is as follows.

        System -> 5. Initialization -> 9. Axis Lock Setting -> Confirm -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)<br>
Figure 4.21.2 Axis Lock Setting Screen 1

![](../_assets/4.서보보드/axis_lock2.png)<br>
Figure 4.21.3 Axis Lock Setting Screen 2

![](../_assets/4.서보보드/axis_lock3.png)<br>
Figure 4.21.4 Axis Lock Setting Screen 3

If the brake of the corresponding axis is not released, the brake output status of the servo safety board must be checked. Disconnect the brake wiring (CNBRK16, CNBRK78 connectors) and output the brake voltage. Measure whether the brake voltage of the corresponding axis is output as 20.0V or higher at the CNBRK16, CNBRK78 connectors. If there is an axis outputting a voltage of 20.0V or lower, it is a failure of the servo safety board (BD642), so replace it.

![](../_assets/4.서보보드/bd642_brake_connector.png)<br>
Figure 4.21.5 CNBRK16, CNBRK78 Connector Pin Layout

* Inspection of Brake Power Supply Abnormalities<br>
The sequence for inspecting brake power wiring is as follows.<br>
1st: Check for poor contact in connectors related to brake power wiring.<br>
2nd: Check for short circuits in the brake power wiring. Check 1:1 using equipment such as a multimeter (tester).<br>
Inspect the internal wiring of the power electric module.<br>

![](../_assets/4.서보보드/psm_psbd.png)<br>
Figure 4.21.6 Power Electric Module and Power Board

* Check the servo safety board (BD642).<br>
If the power electric module is normal, measure the brake power (DC24V) on the servo safety board. It is normal if the measured value across the capacitor (EC9) or across the connector (J12) in the red area of the figure below is DC24V or higher. If it is less than 20V, there is a malfunction in the power supply device generating the brake power. Replace the electric module.

![](../_assets/4.서보보드/bd642_brake_power.png)<br>
Figure 4.21.7 Servo Board Brake Power

(4) Inspect the wiring status.<br>
Check if the motor wiring (U, V, W phases) is connected correctly.
Also, check if the motor wiring is shorted to other wiring or the ground wire (FG).

(5) Check if the rated load is being used.<br>
If the total weight including the workpiece exceeds the rated load, refer to the robot's specification sheet and adjust the load to be within the rating.

(6) Position Deviation Setting Level Error<br>
If the position deviation setting value is smaller than the following maximum measured value, adjust the setting value upward.

        Maximum measured position deviation after operating for more than a cycle x 1.5

![](../_assets/4.서보보드/pos_dev.png)<br>
Figure 4.21.8 Position Deviation Max Measurement Monitoring Screen<br>

![](../_assets/4.서보보드/pos_dev2.png)<br>
Figure 4.21.9 Position Deviation Setting Change Screen

(7) Check the versions of the servo safety board (BD642) and the main com.<br>
This may occur if the compatibility between the servo safety board (BD642) and the main com version is broken. Especially, if a module has been replaced, proceed with a version upgrade to match the version of each module to the current main com version. The version of each module can be checked in the path below.<br>

        Service -> 7. System Diagnosis -> 1. System Version

![](../_assets/4.서보보드/version.png)<br>
Figure 4.21.10 TP Module Version Check Window

(8) Replace other components.<br>
Replace components in the order of Servo Safety Board (BD642) → Servo Drive Unit → Power Electric Module → Motor to check for error occurrence.

![](../_assets/4.서보보드/hi7_robot_brake_power_check.png)<br>
Figure 4.21.11 Hi7-N Controller Motor and Drive Module





[__SOURCE](4-servo-board-part/E50401.md)
## 4.22. E50401. (O Axis) Speed-Based Position Deviation Exceeded

### 1. Overview

This occurs when the position deviation generated during jog operation or low-speed operation exceeds the set value.<br>
If the difference between the movement command position and the actual position is outside the allowable range while the robot is operating under servo control, the servo safety board detects this as an error during servo calculation and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the axis where the error occurred has mechanical interference with other equipment.<br>
(2)	Check if the brake release is operating normally.<br>
* Inspection of individual axis brake release anomalies.<br>
* Inspection of brake power supply abnormalities.<br>

(3)	Inspect the wiring status.<br>
(4)	Check if the rated load is being used.<br>
(5)	Check the position deviation setting level.<br>
(6)	Check the versions of the servo safety board (BD642) and the main com.<br>
(7)	Replace other components.<br>

{% endhint %}

For detailed inspection methods, please refer to "E50400 (O Axis) Position Deviation exceeded".
[__SOURCE](4-servo-board-part/E50402.md)
## 4.23. E50402. (O Axis) Position Deviation Exceeded (Cold Temperature Friction Increase)

### 1. Overview

This occurs when the position (speed) deviation exceeds the set value.
If the difference between the movement command position and the actual position is outside the allowable range while the robot is operating under servo control, the servo safety board detects this as an error during servo calculation and stops the robot.<br>
This error primarily occurs when the position deviation is large while the encoder temperature is low.

Generally, in a low-temperature environment (encoder temperature 5 ℃ or lower), friction components increase due to increased grease viscosity, requiring a larger driving torque than in the normal state. If the robot is operated at high speed in this state, this error may occur.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Operate at low speed (playback speed 30% or less) until the encoder temperature reaches a normal level (approx. 15℃ or higher), then restart at normal speed.<br>
(2)	Check if the robot model is set correctly.<br>\

{% endhint %}

(1)	Operate at low speed (playback speed 30% or less) until the encoder temperature reaches a normal level (approx. 15℃ or higher), then restart at normal speed.

![](../_assets/4.서보보드/enc_tmp2.png)<br>
Figure 4.23.1 Encoder Temperature Check Screen

(2)	Check if the robot model is set correctly.

![](../_assets/4.서보보드/robot_model.png)<br>
Figure 4.23.2 Robot Model Check

Check if the registered robot model on the TP screen matches the actually installed robot.
[__SOURCE](4-servo-board-part/E51429.md)
## 4.24. E51429 Initial Charging Resistor Relay Feedback Error

### 1. Overview

The Servo Safety Board (BD642) activates the initial charge relay during the process of applying motor power and monitors the operation status of the initial charge relay to generate an error. Since the initial charge relay functions to suppress inrush current, an error occurs for safety in case of relay operation abnormality, and the motor power application is blocked.

### 2. Cause and Inspection

{% hint style="info" %}

(1)    Inspect the monitoring system.<br>
(2)    Inspect the power board.<br>
(3)    Inspect the Servo Safety Board (BD642).<br>

{% endhint %}

(1)    Inspect the monitoring system.<br>
Check the cabling between the power electric module (PSM or PDM), where the initial charging resistor and relay are installed, and the servo safety board (BD642) that collects monitoring signals. The cable name is CNPRC, and it enters the power electric module from the servo safety board through the backplane board. Inspect the connection status of this cable's connector.

![](../_assets/4.서보보드/cnprc_cable.png)<br>
Figure 4.24.1 CNPRC Cable Connection

(2)    Inspect the power board.<br>
In the case of the Hi7-N controller, there may be a problem with the servo board, power board, or cable wiring, so inspect or replace them.

![](../_assets/4.서보보드/psm_psbd.png)<br>
Figure 4.24.2 Power Board inside Power Electric Module

(3)    Replace and test the servo safety board.<br>
If the error does not occur after replacing the servo safety board, it can be determined as a failure of the encoder data receiving part of the servo board.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.24.3 Replacement of Hi7-N Controller Servo Safety Board

[__SOURCE](4-servo-board-part/E51441.md)
## 4.25. E51441 (0 Axis) Brake Feedback Error

### 1. Overview

The Servo Safety Board (BD642) monitors the brake operation command and the signal from the brake feedback circuit, and generates an error if the two signals do not match.<br>
If the output of the brake circuit is not executed normally, brake operation may fail, so the servo board detects this and stops the robot. 

### 2. Cause and Inspection

{% hint style="info" %}

(1)    Inspect the brake wiring.<br>
(2)    Inspect the Servo Safety Board (BD642).<br>

{% endhint %}

(1)    Inspect the brake wiring.<br>
The sequence for inspecting brake wiring is as follows.<br>
1st: Check for poor contact in connectors related to brake wiring.<br>
2nd: Check for short circuits in the brake wiring. Check the wiring of each axis 1:1 using equipment such as a multimeter (tester).<br>
3rd: Perform a replacement test of the brake wiring.<br>

If the brake wiring is not disconnected but has poor contact, or if there is contact between the brake power line and other power lines or the metal part of the robot body, it cannot be detected by a short circuit test, so please perform a wiring replacement test.

* Inspect the internal wiring of the controller.<br>
In the case of the Hi7-N controller, inspect the wiring between the CNBRK16 (BD642) connector and CMC1, CMC2.

![](../_assets/4.서보보드/hi7_brake_cable.png)<br>
Figure 4.25.1 Hi7-N Controller Brake Output Wiring

* Inspect the wiring between the controller and the robot.<br>
In the case of the Hi7-N controller, inspect the wiring between CMC1 and CMR1, and between CMC2 and CMR2.

![](../_assets/4.서보보드/hi7_robot_power_cable.png)<br>
Figure 4.25.2 N Controller Brake Output Wiring

(2)    Check the servo safety board.<br>
The sequence for checking the servo safety board is as follows.<br>
1st: Check for blown fuses in the brake circuit.<br>
2nd: If there are no issues with the fuses of all brake channels, replace the servo safety board and check.<br>

* Inspect the brake-related fuses.<br>
In the case of the servo safety board, fuses are designed for each brake in the dotted area shown in the figure below. Inspect using a tester or by checking the blinking of the LEDs on the servo safety board.<br>

![](../_assets/4.서보보드/bd642_brake_fuse.png)<br>
Figure 4.25.3 Servo Safety Board Brake Fuse

* Perform a replacement test of the servo safety board.<br>
If the error does not occur after replacing the servo safety board, it can be determined as a failure of the encoder data receiving part of the servo board.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.25.4 Hi7-N Controller Servo Board Replacement


[__SOURCE](4-servo-board-part/E51443.md)
## 4.26. E51443 Brake Power Error

### 1. Overview

This error occurs when the Servo Safety Board monitors the brake power supply (24.0V) and it deviates from the set normal voltage range.<br>
If the brake power is not supplied normally, the holding of the robot axis may become unstable, so the servo controller detects this, generates an error, and safely stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)    Check if the brake power (24V) is being supplied normally.<br>
(2)    Check for disconnection or poor contact in the brake power cable.<br>
(3)    Replace the Servo Safety Board (BD642).<br>

{% endhint %}

(1)    Check if the brake power (24V) is being supplied normally.<br>
The sequence for inspecting brake power wiring is as follows.<br>
1st: Check for poor contact in connectors related to brake power wiring.<br>
2nd: Check for short circuits in the brake power wiring. Check 1:1 using equipment such as a multimeter (tester).<br>

* Inspect the internal wiring of the power electric module.<br>

![](../_assets/4.서보보드/psm_psbd.png)<br>
Figure 4.26.1 Power Electric Module

(2)    Check for disconnection or poor contact status of the brake power cable.<br>
Inspect the internal wiring of the controller. In the case of the Hi7-N controller, inspect the wiring between the J12(BD642) connector and the CNOBK(power board) connector.

![](../_assets/4.서보보드/brake_pwr_cable.png)<br>
Figure 4.26.2 N Controller Brake Power Inspection

(3)    Perform a replacement test of the servo safety board.<br>
If the error does not occur after replacing the servo safety board, it can be determined as a failure of the encoder data receiving part of the servo board.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.26.3 N Controller Servo Board Replacement


[__SOURCE](5-communication/README.md)
# 5. Communication
[__SOURCE](5-communication/E29003.md)
## 5.1. E29003 Board Communication Error (EtherCAT Disconnected)

### 1. Summary

Board communication error (EtherCAT Disconnected) has occurred.
Communication between the main control module (H6COM-T) and the boards (BD642, BD681, etc.) has been disconnected.

### 2. Causation

{% hint style="info" %}

(1) Check the inter-board communication cable connection and the cable condition.<br>
(2) Inspect the board.<br>

<br>
The board connection configuration varies depending on the operating environment.<br>
- Servo safety board (BD642) used alone<br>
- Servo safety board (BD642) and User DIO board (BD681) used<br>

{% endhint %}

### (1)	Check the inter-board communication cable connection status.
### [Check the Ethernet cable connection status between each module (Main Control Module (H6COM-T) and boards)]

![](../_assets/5-Communication/ethercat_cable_hicom_bd642_r2.png)<br>
Figure 5.1.1 EtherCAT cable connection between the H6COM-T and BD642

<br>

![](../_assets/5-Communication/BD642_BD681_cable_connection.png)<br>
Figure 5.1.2 EtherCAT cable connection between BD642 and BD681 **(When using BD681)**

1)	Inspection Targets<br>
A. Ethernet cable between the main control module (H6COM-T) and the servo safety board (BD642).<br>
B.	Ethernet cable between the servo safety board (BD642) and the user DIO board (BD681). **(When using the BD681).**<br>
2)	Inspection Items<br>
A.	Check that the connectors at both ends of the cable are securely fastened.<br>
B.	Visually inspect the cable for breaks, crimping damage, bends, or damage.<br>
C.	Check the connector pins (terminals) for corrosion, contamination, or bending.<br>
3)	Inspection Method<br>
A.	With the power turned OFF, disconnect and reconnect the cable.<br>
B.	When inserting, ensure it is fully seated until a “click” sound is heard.<br>
C.	If necessary, replace the cable with a spare cable and try again.<br>
D.	Recheck the connection order and verify that it is connected to the correct LAN port.<br>
4)	Additional Checks<br>
A.	If disconnections occur repeatedly, consider the possibility of an internal cable break → Cable replacement may be necessary.<br>
B.	Also check for possible damage to the Ethernet connector (PCB terminal area).<br>
C.	Check the Link/Act LED status on the board.<br>
    * Normal: Green (left) blinking, Yellow (right) ON <br>
    * Abnormal: Green (left) & Yellow (right) lights remain OFF or ON.<br>
    
![](../_assets/5-Communication/E29003/그림2.png)<br>


### (2) Inspect the board.
#### [Servo safety board (BD642) inspection procedure]
![](../_assets/5-Communication/BD642_LED.png)<br> 
Figure 5.1.3 BD642 Board LED, Segment 

<br>

![](../_assets/5-Communication/BD642_7-Segment.png)<br> 
Figure 5.1.4 7-Segment Status information

<br>

1) Check the communication connection status<br>
   Verify that LEDs No. 4 to 5 (green) in 'Figure 5.1.3' are ON. <br>

2) Check the normal boot status<br>
   After the Main Control Module (H6COM-T) has completely booted (approximately 50 seconds after power-on), <br>
   LEDs No. 1 to 5 (green) in 'Figure 5.1.3' should be ON, LEDs No. 6 to 10 (red) should be OFF, <br> and the 7-segment display should show '2. Safe State' with the decimal point blinking.

If a communication connection problem still exists even though there are no abnormalities in the inspection items 1 and 2, replace the board.<br>

 
#### [User DIO board (BD681) inspection procedure]
![](../_assets/5-Communication/BD681_LED.png)<br> 
Figure 5.1.5 BD681 Board LED 

<br>
 
1)	Check the communication connection status<br>
A.	Verify that LED No. 3 (green) in 'Figure 5.1.5' is ON.<br>

2)	Check the normal operation status<br>
A.	Verify that LEDs No. 1 to 2 (green) in 'Figure 5.1.5' are blinking.<br>

If a communication connection problem still exists even though there are no abnormalities in the inspection items 1 and 2, replace the board.<br>

[__SOURCE](5-communication/E29016.md)
## 5.2. E29016 Board Communication (EtherCAT) Master Disconnection Detected

### 1. Summary

The connection with the first device connected to the EtherCAT master has been lost.

### 2. Causation

{% hint style="info" %}

(1) Check the inter-board communication cable connection and the cable condition.<br>
(2) Inspect the Servo safety board (BD642).<br>

{% endhint %}

### (1) Check the inter-board communication cable connection status.

#### [Check the Ethernet cable connection status between each module (Main Control Module (H6COM-T) and Servo safety board (BD642))]
![](../_assets/5-Communication/ethercat_cable_hicom_bd642_r1.png)<br>
Figure 5.2.1 EtherCAT cable connection between the H6COM-T and BD642

1)	Inspection Targets<br>
A.	Ethernet cable between the main control module (H6COM-T) and the servo safety board (BD642).<br>
2)	Inspection Items<br>
A.	Check that the connectors at both ends of the cable are securely fastened.<br>
B.	Visually inspect the cable for breaks, crimping damage, bends, or damage.<br>
C.	Check the connector pins (terminals) for corrosion, contamination, or bending.<br>
3)	Inspection Method<br>
A.	With the power turned OFF, disconnect and reconnect the cable.<br>
B.	When inserting, ensure it is fully seated until a “click” sound is heard.<br>
C.	If necessary, replace the cable with a spare cable and try again.<br>
D.	Recheck the connection order and verify that it is connected to the correct LAN port.<br>
4)	Additional Checks<br>
A.	Check the Link/Act LED status on the board.<br>
- Normal: Green (left) blinking, Yellow (right) ON <br>
- Abnormal: Green (left) & Yellow (right) lights remain OFF or ON.<br>
![](../_assets/5-Communication/E29016/그림2.png)<br>
B.	If disconnections occur repeatedly, consider the possibility of an internal cable break → Cable replacement may be necessary.<br>
C.	Also check for possible damage to the Ethernet connector (PCB terminal area).<br>

### (2) Inspect the Servo safety board (BD642).
#### [Servo safety board (BD642) inspection procedure]
![](../_assets/5-Communication/BD642_LED.png)<br> 
Figure 5.2.2 BD642 Board LED, Segment 

<br>

![](../_assets/5-Communication/BD642_7-Segment.png)<br> 
Figure 5.2.3 7-Segment Status information

<br>

1) Check the communication connection status<br>
   Verify that LEDs No. 4 to 5 (green) in 'Figure 5.2.2' are ON. <br>

2) Check the normal boot status<br>
   After the Main Control Module (H6COM-T) has completely booted (approximately 50 seconds after power-on), <br>
   LEDs No. 1 to 5 (green) in 'Figure 5.2.2' should be ON, LEDs No. 6 to 10 (red) should be OFF, <br> and the 7-segment display should show '2. Safe State' with the decimal point blinking.

If a communication connection problem still exists even though there are no abnormalities in the inspection items 1 and 2, replace the board.<br>

[__SOURCE](5-communication/EtherCAT_ENI_Missmatch.md)
## 5.3. Board communication (EtherCAT) master ENI mismatch

### 1. Summary

Controller communication configuration and ENI file mismatch.<br>
(ENI : EtherCAT Network Information)

### 2. Causation

{% hint style="info" %}

The controller communication configuration does not match the configured ENI file.<br>

{% endhint %}

### Verify the controller communication configuration.

The controller supports predefined communication configurations. If the communication connection is configured incorrectly, normal operation is not possible.<br>
In addition, distinguish between the [IN] and [OUT] communication connectors when connecting.
To ensure proper communication, connect the '[OUT] connector of the first board' to the '[IN] connector of the second board'.<br>

<strong>< Example of a correct communication configuration ></strong><br>

- Main Control Module(H6COM-T) ↔ **[IN]** Servo safety board (BD642)
- Main Control Module(H6COM-T) ↔ **[IN]** Servo safety board (BD642) **[OUT]** ↔ **[IN]** User DIO board(BD681)

<br>

<strong>< Example of an incorrect communication configuration ></strong><br>

- Main Control Module(H6COM-T) ↔ **[OUT]** Servo safety board(BD642)
- Main Control Module(H6COM-T) ↔ **[IN]** Servo safety board(BD642) **[OUT]** ↔ **[OUT]** User DIO board(BD681)
- Main Control Module(H6COM-T) ↔ **[IN]** User DIO board(BD681) **[OUT]** ↔ **[IN]** Servo safety board(BD642)

<br>

![](../_assets/5-Communication/BD642_EtherCAT_Connector.png)<br>
Figure 5.3.1 BD642 EtherCAT Connector

<br>

![](../_assets/5-Communication/BD681_EtherCAT_Connector.png)<br>
Figure 5.3.2 BD681 EtherCAT Connector

<br>

When the communication connection is configured correctly, the controller automatically selects the ENI file and attempts a connection at power-on.<br>

If the internal settings of the ENI file are incorrect, communication may be established but the functions may not operate properly.
In this case, update the version of the Main Control Module (H6COM-T) of the controller or contact our company.<br>

To manually change the ENI file selection, configure it in the TP menu below.
After changing the setting, reboot the controller for the changes to take effect.

**- The location of the menu : [system]-[5:Initialization]-[10:Controller Setting]**


[__SOURCE](appendices/README.md)
# Appendices
  



[__SOURCE](appendices/rules-occupational-safety.md)
# Rules on Occupational Safety and Health Standards and Safety Inspection Notification

This industrial robot shall be installed in consideration of the inspection requirements specified in the Rules on Occupational Safety and Health Standards and the Safety Inspection Notification, where applicable.

"[Rules on Occupational Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/en/README)"

[__SOURCE](quality-assurance.md)
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/en/README)"
