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
Figure 5.3.1 BD681 EtherCAT Connector

<br>

When the communication connection is configured correctly, the controller automatically selects the ENI file and attempts a connection at power-on.<br>

If the internal settings of the ENI file are incorrect, communication may be established but the functions may not operate properly.
In this case, update the version of the Main Control Module (H6COM-T) of the controller or contact our company.<br>

To manually change the ENI file selection, configure it in the TP menu below.
After changing the setting, reboot the controller for the changes to take effect.

**- The location of the menu : [system]-[5:Initialization]-[10:Controller Setting]**

