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
