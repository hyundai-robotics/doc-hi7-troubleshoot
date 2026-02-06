# Hi7 Controller Maintenance Manual – Troubleshooting

The controller is designed with primary emphasis on high precision and high-speed performance.
In the event of a malfunction, the system is structured to allow easy identification of the cause and rapid recovery. Please read and fully understand this manual to ensure effective and efficient troubleshooting.

## Troubleshooting Procedures

This section describes the troubleshooting procedures for each error code that may occur in the Hi7-N Controller.
# 1. 전장## 1.1. 전압점검1 – Hi7-N 제어기 내부 3상 전압 점검절차

(1) 제어기 내부의 3상 전원 전압을 확인하십시오.

제어기 전면에 부착된 전장모듈(PSM)은 각종 전원의 분배 및 중계를 담당하고 있으며, 3상 전원은 전장모듈 내 마그네트 스위치를 통하여 온/오프 됩니다. 모터 오프 상태에서 전장모듈에 입력되는 전압이 AC 220V 기준으로 오차범위가 10%이내인지 점검합니다. 만약 측정된 전압이 허용 범위를 벗어나는 경우에는 아래와 같이 점검하십시오.

![](../_assets/1.전장/전압점검/전압점검1.PNG)<br>
그림 1.1 전장모듈에 입력되는 3상 전원


{% hint style="warning" %}
경고(Warning)
고전압 측정 시 주변 부품 및 상간 단락 가능성이 있으므로 주의하십시오.
{% endhint %}

1) 제어기 명판의 전압이 220V 인 경우
제어기 입력 전압이 AC 220V인 경우에는 외부에서 전원 스위치 또는 터미널 블록으로 입력되는 전압과 내부의 전장모듈에 측정된 전압이 동일해야 합니다. 만약 차이가 있다면 3상 전원 배선을 점검하시기 바랍니다.

2)	제어기 명판의 전압이 220V가 아닌 경우
제어기 입력전원이 AC 220V 사양이 아닌 경우에는 내장된 트랜스포머를 사용하여 3상 전원을 AC220V로 변환하여 전장모듈에 연결됩니다. 전장모듈 측에서 측정된 전압이 AC 220V 기준으로 오차범위가 10%이내인지 점검합니다. 만약 측정된 전압이 허용 범위를 벗어나는 경우에는 내장된 트랜스포머의 입력과 출력 단자의 연결 상태를 점검하십시오. 내장된 트랜스포머의 1차단은 제어기 명판에 표기된 전압으로 연결되어야 합니다. 트랜스포머의 2차단은 항상 AC 3상 220V로 설정되어 있습니다. 입력단자와 출력단자가 올바르게 연결된 상태에서도 출력단자에서 AC 3상 220V가 정상적으로 출력되지 않으면 트랜스포머 불량입니다. 이때의 트랜스포머의 출력전압 오차는 5% 이내이어야 합니다.
## 1.2. 전압점검2 – Hi7-N 제어기 입력 3상 전압 점검절차

(1)	제어기에 부착된 명판의 전압과 실제 입력전압을 확인하십시오.

제어기에 실제로 공급되는 전압이 명판에 표기된 전압의 허용 범위 이내인지를 확인하십시오. 입력전압의 허용 범위는 명판에 표기된 값의 10% 이내이고, AC 220V 기준으로 AC 198V 이상이어야 합니다. 아래의 그림은 제어기의 입력전압의 측정방법을 나타낸 것입니다. 측정된 전압이 허용 범위를 벗어나는 경우에는 전원 설비를 점검하여 주십시오.

*	전면 스위치의 전원라인 측 측정

![](../_assets/1.전장/전압점검/전압점검2.PNG)<br>
(a) Hi7-N 제어기<br>
그림 1.2 전원 스위치의 전원라인 측 측정

{% hint style="warning" %}
고전압 측정 시 주변 부품 및 상간 단락 가능성이 있으므로 주의하십시오.
{% endhint %}
## 1.3. 부품 교환 요령

고장수리(troubleshooting)시 각 부품 및 기판의 교환요령을 설명합니다.

### 1. 모듈 교환 요령

{% hint style="warning" %}
모듈 교환시 작업자는 다음의 주의 사항을 유념하여 주십시오.
{% endhint %}

①	작업전에 반드시 전원장치의 전원을 꺼 주십시오.

②	작업자의 손을 청결하게 하여 기름이나 수분이 기판에 묻지 않도록 주의하십시오. 기판을 잡아야 할 경우에는 그 주위를 잡도록 하십시오. 전자 부품이나 패턴, 그리고 특히 커넥터의 접촉부분에는 손이 닿지 않도록 주의하여 주십시오.

③	작업자의 몸(손)과 제어기와는 동전위(同電位)가 되도록 하여 주십시오.

④	각 기판에는 다수의 커넥터가 있습니다. 교환시에 오삽입, 누락 또는 헐렁한 상태가 되지 않도록 정확히 삽입하여 주십시오. 커넥터의 명판과 기판상에 인쇄된 이름을 맞추어 삽입하십시오.

### 1.1. 메인모듈 교환 요령

{% hint style="warning" %}
메인모듈을 빼기 전에 반드시 먼저 다음 사항을 조치하여 주십시오.
{% endhint %}

①	메인모듈를 교환하고자 할 때는 먼저 필요한 프로그램 / 정수 데이터를 (Notebook) PC의 HR-VIEW S/W 또는 USB Memory를 이용하여 백업한 후에 교체하여 주십시오.

②	티칭한 프로그램 / 정수 데이터는 메인모듈의 RAM상에 저장되어 있으므로, 새로운 기판으로 교체하였을 때는 원하는 기존의 프로그램 / 정수 데이터가 없습니다.  

③	교체한 후에는 앞서 백업(backup)받은 내용을 새로운 기판에 로드(load)하여 사용하시면 됩니다.

이상의 주의사항을 지키고, 다음의 순서에 따라 기판을 교환하여 주십시오. 

#### 1.1.1 컨트롤 모듈의 분리

①	먼저 전원 장치의 입력 전원을 제거해 주십시오.

②	모듈에 연결된 각종 커넥터를 빼십시오. 이때 나사로 체결되어 있는 커넥터의 경우에는 알맞은 드라이버를 이용하여 풀며, 커넥터에 무리가 가지 않도록 하여 빼십시오.

③	상하에 있는 고정 나사를 약간만 풀고, 모듈을 위로 이동시킨 후 당겨 빼냅니다.

#### 1.1.1 컨트롤 모듈의 결합

①	먼저 제어기 입력전원이 OFF 상태임을 확인해 주십시오.

②	상하에 있는 고정 나사에 교체할 모듈을 걸어서 장착한 후 고정나사를 체결합니다.

③	모듈에 연결된 각종 커넥터를 연결하십시오. 이때 나사로 체결되어 있는 커넥터의 경우에는 알맞은 드라이버를 이용하여 연결하고, 커넥터에 무리가 가지 않도록 연결하십시오.

④	통신선이 잘못 연결되진 않았는지, 빠트린 작업이 없는지 한번 더 확인하십시오.

### 1.2. 구동장치(Drive Module) 교환 요령

{% hint style="warning" %}
서보 구동장치 교환 시 작업자는 다음의 주의 사항을 유념하여 주십시오.
{% endhint %}

다른 기종의 서보 구동장치와 호환성이 없는 경우가 있으므로, 앞면 패널의 명판을 반드시 확인 하십시오.

#### 1.2.1 서보 구동장치(Drive Unit)의 분리
①	먼저 전원 장치의 입력 전원을 꺼 주십시오.
②	서보 구동장치의 보호 커버의 고정볼트를 풀어서 떼어 냅니다.
③	단자대에 나사로 고정된 배선을 떼어 냅니다.
④	접속되어 있는 커넥터를 모두 떼어 냅니다.
⑤	서보 구동장치를 고정하고 있는 나사를 떼어 냅니다.
⑥	서보 구동장치를 꺼냅니다. 서보 구동장치는 무거우므로 꺼낼 때 다치지 않도록 주의하십시오. 또한 옆의 배선들도 손상되지 않도록 주의하십시오.

#### 1.2.2 서보 구동장치(Drive Unit)의 결합
①	먼저 전원 장치의 입력 전원을 꺼 주십시오.
②	서보 구동장치를 잘 들어서 밀어 넣습니다. 서보 구동장치는 무거우므로 밀어 넣을 때 다치지 않도록 주의하십시오. 또한 옆의 배선들도 손상되지 않도록 주의하십시오.
③	서보 구동장치를 나사로 고정시키십시오.
④	배선들을 단자대에 나사로 조이십시오.
⑤	커넥터를 모두 접속시키십시오.
⑥	서보 구동장치 보호 커버을 볼트로 체결합니다.
⑤	빠트린 작업이 없는지 한번 더 확인하십시오.

### 1.3. 1.1.4. PSM(Power Supply Module)의 교환 요령 

{% hint style="warning" %}
PSM는 주 제어전원으로 이용되는 복합전원장치로서 정밀장치이므로 취급에 특별한 주의를 바랍니다.
{% endhint %}

#### 1.2.1 PSM(Power Supply Module)의 분리
①	먼저 전원 장치의 입력 전원을 꺼 주십시오.
②	모듈에 연결된 각종 커넥터를 빼십시오.
③	상하에 있는 고정 나사를 약간만 풀고, 모듈을 위로 이동시킨 후 당겨 빼냅니다. PSM은 무거우므로 꺼낼 때 다치지 않도록 주의하십시오. 또한 옆의 배선들도 손상되지 않도록 주의하십시오. 이때 너무 갑자기 세게 잡아당기면 다칠 수도 있으니 주의하십시오.

#### 1.2.2 PSM(Power Supply Module)의 결합
①	먼저 제어기 입력전원이 OFF 상태임을 확인해 주십시오.
②	상하에 있는 고정 나사에 교체할 모듈을 걸어서 장착한 후 고정나사를 체결합니다. PSM은 무거우므로 장착할 때 다치지 않도록 주의하십시오. 또한 옆의 배선들도 손상되지 않도록 주의하십시오. 이때 너무 갑자기 세게 집어넣으면 다칠 수도 있으니 주의하십시오.
③	모듈에 연결된 각종 커넥터를 연결하십시오. 이때 나사로 체결되어 있는 커넥터의 경우에는 알맞은 드라이버를 이용하여 연결하고, 커넥터에 무리가 가지 않도록 연결하십시오.
④	커넥터가 잘못 연결되진 않았는지, 빠트린 작업이 없는지 한번 더 확인하십시오.

## 1.4. 조정 요령

본 제어기는 출하시에 기본적으로 모든 것이 조정이 되어 있으므로 별도로 조정할 필요 없습니다. 그러나 부품을 교환할 경우에는 일부 조정이 필요하며 그 조정위치와 요령을 설명합니다. 필요한 경우를 제외하고는 조정하지 말고 문제가 발생하였더라도 그 원인이 밝혀지지 않은 경우에는 절대로 건드리지 않도록 하십시오. 

### 1. 전원계통의 조정 

전원계통에 고장이 발생한 경우, 혹은 전원을 변경한 경우는 각 전원 전압을 측정하여 기준치를 벗어나는 것은 조정해 주십시오(디지털 전압계를 사용하여 측정하십시오). 

### 1.1. Hi7-N 제어기 전원계통의 조정


![](../_assets/1.전장/조정요령/Hi7-N제어기%20전원%20기준치.PNG)

그림 1. Hi7-N 제어기 전원 기준치


(주1) 기준치에 들어있지 않은 경우는 PSM을 교환하십시오. 

(주2) 일단 측정장소에서의 기준치를 확인하고, 가능한 로봇의 엔코더에 가장 가까운 단자대, 커넥터의 핀 사이에서 측정하여 주십시오. 이때 기준치는 DC5.1V±0.1V이어야 합니다. 

### 2. 변압기 (TR2)

{% hint style="warning" %}
Hi7-N제어기 : 변압기(TR2)의 출력 전원은 반드시 AC220V 로 이용하여야 합니다.
2차측 단자는 내부 부품들의 사양에 맞는 전원으로 연결되어 있으니, 절대로 손대지마십시오.
{% endhint %}

본 제어기내 입력전원은 반드시 AC220V 3상을 사용해야 합니다. 그외 전압 사양의 제어기는 출하 시 조정 완료된 상태이오니, 당사 요원의 허락 없이 절대로 탭을 변경할 수 없습니다.
# 2. Servo AMP Board## 2.1. E02500 AMP Regenerative Discharge Resistor Overheat

### 1. Overview

This error relates to the overheating of the resistor used to dissipate regenerative power generated during robot deceleration or downward movement in the direction of gravity. It can be caused by decreased cooling fan performance, temporary rapid movements, or exceeding the regenerative discharge capacity due to continuous robot operation.

### 2. Causes and Inspection Methods

{% hint style="info" %}

The temperature of the regenerative discharge resistor has risen above the reference value. This is due to excessive robot playback speed or issues with the cooling system.

* <If the error occurs at a specific step depending on the robot's playback speed>

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

Table 1-1 Installation Locations of Hi7-N00 Controller Fans

* Inspection of Fan Operational Status

If a fan is not rotating or its speed is abnormally low, please replace the corresponding fan. The lifespan of a cooling fan varies depending on the operating environment and total usage hours.


* Inspection of Fan Power Supply Voltage

If all fans are inoperative, please verify the fan input voltage. The fan input voltage is set to AC 220V, with an allowable range within 10% of the rated voltage. If the voltage is more than 10% below the rating, the cooling efficiency will decrease due to the reduced fan rotation speed. If the voltage is low, please inspect the fan power connector (CNFN2) and the overall input voltage of the controller.

(4)	Please inspect the robot's regenerative power load.

* Verify the error according to the robot's playback speed.

If an overheat error occurs during continuous playback for 5 minutes or longer, it is likely because the robot's repetitive motions have exceeded the controller's cooling capacity. Please reduce the robot's playback speed and verify if the error persists. If the overheat error is resolved by lowering the speed but the required cycle time for the task cannot be achieved, please contact our technical support department.
## 2.2. E02501 AMP Regenerative Discharge Resistor Open Circuit, Resistor or Circuit Error

### 1. Overview

This error occurs during the dissipation of regenerative power generated during robot deceleration or downward movement in the direction of gravity. It can be caused by a failure in the overheat detection sensor circuit, an open circuit in the resistor, or an overvoltage in the 3-phase power supply.

### 2. Causes and Inspection Methods

{% hint style="info" %}
Overheat errors can also occur due to an open circuit in the resistor or an anomaly in the discharge control system. Additionally, an increase in the regenerative resistance value or a surge in the 3-phase power supply voltage may trigger this error.

* <If the error consistently occurs at the moment the motor is turned ON>

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

![](../_assets/2.서보AMP/E02501/E02501_1.PNG)

(a) Hi7-N Controller (BD651 / BD653 Board)

(b) Hi7-T Controller (To be included in the future)

(c) Hi7-NX Controller (To be included in the future)

Figure 1.1 Measuring Resistance at the CNDR Connector

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
## 2.3. E02502 AMP Regenerative Discharge Resistor Detection Circuit Error

### 1. Overview

This error relates to the overheating of the resistor used to dissipate regenerative power generated during robot deceleration or downward movement in the direction of gravity. It is typically caused by a failure in the overheat detection sensor circuit or a cable-related issue.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly has occurred in the path used to detect overheat errors, or the resistance value has changed.

* <If the error consistently occurs even when the motor is OFF>

(1)	Inspect the cables related to overheat error detection.

-> Check the resistance of the CNTR cable.

(2)	Inspect the components related to overheat error detection.

-> Hi7-N Controller: Replace the Control Module (including the BD642 board) and verify if the error persists.

-> Hi7-T Controller: (To be included in the future)

-> Servo Drive Unit: Replace the servo drive unit and verify if the error persists.

{% endhint %}

(1)	Please inspect the overheat error detection cable.

The regenerative resistor overheat error is detected by the servo drive unit by monitoring the ON/OFF status of the overheat sensor attached to the resistor via the CNTR connector. In the Hi7-N controller, the detected error signal is transmitted from the BD651/BD653 board through the BD652/BD654 and is finally processed by the software on the BD642 board.

![](../_assets/2.서보AMP/E02502/E02502_1.PNG  )

Figure 1.1 Component Layout for Regenerative Resistor Overheat Error (Hi7-N Controller)

* CNTR Cable Inspection

Check for any anomalies in the sensor at the CNTR connector that connects to the overheat detection sensor. Under normal conditions, the sensor resistance should measure less than 0.1 ohm.

![](../_assets/2.서보AMP/E02502/E02502_2.PNG  )

Figure 1.2 Measuring Resistance at the CNTR Connector (Hi7-N Controller)

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
## 2.4. E02503 AMP PN Overvoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error can occur when the robot's motion changes abruptly or if the resistance value of the regenerative discharge resistor has increased.

* <If the error occurs at a specific step depending on the robot's playback speed>

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

(2)-2 Hi6-T Controller

-> To be included in the future (TBD)

(2)-3 Hi6-NX Controller 

-> To be included in the future (TBD)

![](../_assets/2.서보AMP/E02503/E02503_1.PNG  )

Figure 1.1 Measuring Resistance at the CNDR Connector (Hi6-N Controller)## 2.5. E02504 AMP Diode Module Error or AC Input Voltage Exceeded

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold of DC 395V.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly in the diode module has caused the PN voltage to fall outside the allowable range. This error can also occur if the 3-phase AC voltage supplied to the servo drive unit (AMP) is abnormally high.

* <If the error consistently occurs at the moment the motor is turned ON>

(1)	Inspect the power-related components.

-> Replace the servo drive unit and verify if the error persists.

(2) Inspect the power supply voltage.

-> Check the internal 3-phase voltage of the controller.

-> Check the input 3-phase voltage supplied to the controller.

{% endhint %}

(1)	Please inspect the power-related components.

* Replacement Inspection of the Servo Drive Unit

Replace the module responsible for detecting the AMP overvoltage error and verify if the error recurs. A circuit failure within the module may cause the error to persist.

(1)-1. Hi6-N Controller

-> Servo drive unit for mid-sized robots: H7D6X

-> Servo drive unit for small-sized robots: H7D6A

(1)-2. Hi6-T Controller

-> Servo drive unit for electronics industry robots: To be included in the future (TBD)

(1)-3. Hi6-NX Controller

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

## 2.6. E02505 AMP PN Overvoltage Detection Path Error or Discharge Error

Former Error Code: E0011 AMP P-N Overvoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has exceeded the preset threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An anomaly has occurred in the path used to detect PN voltage drops from the diode module, or a failure has occurred in the PN discharge circuit.

* <If the error consistently occurs even when the motor is OFF>

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

![](../_assets/2.서보AMP/E02505/E02505_1_en.PNG)

Figure 1.1 Component Layout for Overvoltage Error (Hi7-N Controller)

<br>

(2)	Hi7-T Controller

->	To be included in the future (TBD)

(3)	Hi7-NX Controller

->	To be included in the future (TBD)## 2.7. E02506 AMP PN Undervoltage Generated

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error may occur at a specific step depending on the robot's playback speed. It indicates that the PN voltage has dropped due to high energy consumption. It can also be caused by an unstable 3-phase input power supply to the controller.

* <If the error occurs at a specific step depending on the robot's playback speed>

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



## 2.8. E02507 AMP Diode Module Error or AC Input Voltage Insufficient


Former Error Code: E0033 AMP PN Undervoltage Generated


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

The PN voltage failed to charge due to an anomaly in the diode module. This error can also occur if the AC voltage supplied to the servo drive unit is insufficient.

* <If the error occurs at the moment the motor is turned ON>

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

-> Specifications and inspection procedures for the Hi7-NX model will be updated in a future revision.## 2.9. E02508 AMP PN Undervoltage Detection Path Error or Discharge Error


Former Error Code: E0033 AMP PN Undervoltage Generated


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motors has been measured below the preset undervoltage threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

A problem has occurred in the path used to detect PN voltage drops starting from the diode module. Alternatively, an anomaly has occurred in the PN discharge circuit.

* <If the error occurs even when the motor is OFF>

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


![](../_assets/2.서보AMP/E02508/E02508_1_en.PNG  )

Figure 1.1 Replacement of Control Module and Servo Drive Unit

<br>


(2) Please inspect the components related to undervoltage error detection.

-> To be included in the future (TBD)
## 2.10. E02522 (Axis ○) IPM Fault – Specific Step

### 1. Overview

A fault output has been triggered from the IPM (Intelligent Power Module), which is the switching element within the servo drive unit that powers the motor. An IPM fault can be caused by a temperature rise in the heat sink, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Methods

{% hint style="info" %}

* < If the error occurs at a specific step>

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

Figure 1.1 Internal Wiring Inspection Points by Axis for HS165


-> Verify the error by reducing the robot's playback speed

If the error occurs at a step where a posture change causes a sudden fluctuation in axis speed, reduce the playback speed to verify the error. If the error is resolved after lowering the playback speed, adjust the taught speed for that specific step and save the task program before further use.

->  Verify the error by changing the interpolation of the taught step

If the axis speed continues to fluctuate drastically even after reducing the playback speed to 75% or lower, change the interpolation of the taught step to 'P' (PTP: Point-to-Point) and verify the error. If the error is resolved by changing the interpolation at the same playback speed, please modify the teaching points accordingly.
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


*   <If both the Board LEDs and PSM LEDs are OFF>

    (2)	Please inspect the output of the control power supply (PSM).

    -> Hi7-N Controller

    *  Disconnect the CN24VB1 connector connected to the BD604 of the Control Module, then check the 24V output status LED on the PSM.

    *   Remove the BD642 board, then check if the 'POW' LED on the servo drive unit lights up.

    ->  Hi7-T Controller: To be included in the future (TBD)

    -> Hi7-NX Controller: To be included in the future (TBD)


    (3)	Please inspect the control power supply unit (CMSMPS).

    ->  Check the input voltage supplied to the CMSMPS.

    ->  Replace the CMSMPS and check the status LEDs.

    * <If only the Board LEDs are OFF>

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

![](../_assets/2.서보AMP/E02541/E02541_1.PNG)

Figure 1.1 Location of Controller Power LEDs (Location of the ‘POW LED’ on the Hi7-N Servo Drive Unit)

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

## 2.12. E50300 (Axis ○) IPM Fault

### 1. Overview

An IPM (Intelligent Power Module) fault output has occurred within the switching element of the servo drive unit that operates the motor. An IPM fault can be triggered by an increase in heat sink temperature, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Procedures

{% hint style="info" %}

* <If the error occurs at the moment the motor is turned on or occurs intermittently>

(1)	Inspect the motor drive components.

->	Check the output cables connected to the servo drive unit.

->	Inspect the terminals of the switching elements inside the servo drive unit.

->	Replace the servo board and verify if the error persists.

*	Hi7-N Controller : BD642

*	Hi7-T Controller : To be included in the future (TBD)

*	Hi7-NX Controller : To be included in the future (TBD)

->	서보 구동장치를 교체한 후 에러를 확인하여 주십시오.

*	Hi7-N Controller : 중형 H7D6X, 소형 : H7D6A (서보보드 제외)

*	Hi7-T Controller : To be included in the future (TBD)

*	Hi7-NX Controller : To be included in the future (TBD)

->	Replace the servo motor and verify if the error persists.


<If the error occurs after the robot has been operating for 5 minutes or longer>

(2)	Inspect the controller's cooling fans.

->	Check the operating status of each fan.

->	Check the power supply voltage of the fans.

{% endhint %}

(1)	Inspect the motor drive components.

The servo drive unit that operates the motor receives commands from the servo board (BD642) through a direct board-to-board connector. The current output from the internal amplification circuit is then delivered to the motor via the wiring connected to each axis connector.

->	Inspect the output cables connected to the servo drive unit.

Check the condition of the wiring connecting the servo drive unit to the motor. When inspecting, ensure the controller power is OFF, then disconnect the connector from the servo drive unit. Measure the resistance between each phase and the ground on the cable side to check for any short circuits.

![](../_assets/2.서보AMP/E02520/E02520_1_en.PNG)


Figure 1.1 Inspection of the output cable for the Hi7-N controller servo drive unit

<br>


->	Inspect the switching elements of the servo drive unit.

The switching elements of the servo drive unit output AC current for each phase by switching the DC voltage supplied from the diode module. If a short circuit occurs at the internal terminals of the switching element, overcurrent flows, triggering an IPM fault error. With the connectors disconnected, check for a short circuit between the output terminals (U, V, or W) and the P or N terminals of the switching element. If a short circuit is confirmed, the servo drive unit must be replaced, and the cable connecting the servo drive unit to the motor should also be inspected.

*	Hi7-N Controller

    -	Servo drive unit for mid-sized robots: H7D6X

    -	Servo drive unit for small-sized robots: H7D6A 


*	Hi6-T제어기 (To be included in the future)

*	Hi6-NX제어기 (To be included in the future)

![](../_assets/2.서보AMP/E02520/E02520_2.PNG)


Figure 1.2 Inspection for short circuits in the switching elements of the Hi7-N controller

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

If the error does not recur after replacing the servo motor, the original servo motor is defective. Please replace the servo motor with a known-good unit. The figure below shows the location of the motors for each axis of the HS165 robot. For other robot models, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/2.서보AMP/E02520/E02520_3.PNG)

Figure 1.3 Servo motor locations for each axis of the HS165 robot

<br>

(2)	Inspect the controller’s cooling fans.

If an IPM fault error occurs after the robot has been operating for 5 minutes or longer, it indicates that the controller's cooling system is malfunctioning, causing the IPM to exceed its specified operating temperature range. The rear of the controller is equipped with fans to cool the heat sinks of the servo drive units and the regenerative discharge resistors.

<br>


Table 1-1 Installation locations of Hi6 controller fans

![](../_assets/2.서보AMP/E02520/E02520_4.PNG)


->	Check the operating status of each fan.

If a fan is not rotating or the rotation speed is abnormally low, please replace the affected fan. The lifespan of a fan varies depending on the operating environment and total usage hours.


->	Check the fan power supply voltage.

If all fans are not operating, please check the input voltage supplied to the fans. The input voltage for the fans is set to 220V AC, with an allowable tolerance of within 10% of the rated voltage. If the voltage is more than 10% lower than the rating, the cooling efficiency will decrease due to the reduced fan rotation speed. If the voltage is low, please check the power connector for the rear cooling fans and the main input voltage of the controller.
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


![](../_assets/2.서보AMP/E02521/E02521_1_en.PNG)

Figure 1.1 Inspection of the output cable for the Hi7-N controller servo drive unit

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
*   Hi7-NX Controller: To be included in the future# 3. 서보안전 보드(안전파트)## 3.1. N00088 외부비상정지 입력
### 1. 개요
외부 비상정지(E-Stop) 신호가 입력되었습니다.<br>
안전을 확보하기 위해 로봇의 모든 모션은 즉시 정지되며,서보 모터는 모터 오프(Motor OFF) 상태로 전환됩니다.

### 2. 원인 및 점검
{% hint style="info" %}
(1) 실제 외부 비상정지(E-Stop) 버튼이 작동한 경우<br>
(2) 외부 비상정지 회로의 배선 또는 접점에 이상이 발생한 경우<br>
(3) 외부 비상정지 신호에 대한 안전 입력 할당이 설정되지 않은 경우<br>
{% endhint %}<br>

### (1) 실제 외부 비상정지 버튼이 작동한 경우
외부 비상정지(E-Stop) 버튼이 실제로 작동했는지 확인하십시오. 다른 작업자 또는 관리자가 외부 비상정지 버튼을 작동시켰을 수 있습니다.<br>
또한, 안전 펜스 내부에서 작업자가 작업 중일 가능성이 있으므로 로봇 주변에 인원이 있는지, 또는 위험 요소(공구, 지그 등)가 존재하는지 확인하십시오.<br>
로봇을 재가동해도 안전하다고 판단되는 경우, 외부 비상정지 버튼을 해지한 후 수동 운전 모드에서 로봇을 먼저 동작시키십시오.<br>

### (2)	외부 비상정지 회로의 배선 또는 접점에 이상이 발생한 경우
외부 비상정지 관련 배선을 점검하기 위해서는 외부 비상정지 입력이 [안전 입출력 할당] 기능을 통해 어떤 입력 채널에 할당되어 있는지 확인하십시오.<br>
기본 설정의 경우(공장출하 시), 외부 비상정지 입력은 기본 안전입력 0번 채널에 할당되어 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:안전 입출력 할당<br>
![](../_assets/3-Safety-io/N00088/base_add_comm_si_func_sel.png)<br>
그림 3.1.1. T/P 화면 안전 입출력 할당 화면<br>

#### 2-1) 기본 안전입력에 할당되어 있는 경우
외부 비상정지 입력이 기본 안전입력에 할당되어 있는 경우, 서보안전 보드 CNSI1 커넥터(4채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

![](../_assets/3-Safety-io/N00088/bd642_cnsi1_position.png)<br>
그림 3.1.2. Hi7-N제어기 서보안전 보드 CNSI1 위치<br>

외부 비상정지 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 그림 3.1.1.을 통해 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 서보안전 보드 CNSI1의 결선 표준은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

#### 2-2) 부가 안전입력에 할당되어 있는 경우 
외부 비상정지 입력이 부가 안전입력에 할당되어 있는 경우, 옵션 안전IO 보드 CNSI2 커넥터(8채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

![](../_assets/3-Safety-io/N00088/bd680_cnsi2_position.png)<br>
그림 3.1.3. Hi7-N제어기 옵션 안전IO 보드 CNSI2 위치<br>

외부 비상정지 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 그림 3.1.1.을 통해 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 옵션 안전 IO 보드 CNSI2의 결선 표준은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

#### 2-3) 안전 통신입력에 할당되어 있는 경우
외부 비상정지 입력이 안전 통신입력에 할당되어 있는 경우, 'Hi7 로봇제어기 기능설명서-산업용 통신'메뉴얼을 참고하세요.

### (3) 외부 비상정지 신호에 대한 안전입력 할당이 설정되지 않은 경우
외부 비상정지 입력이 안전입력 할당에서 선택되지 않은 경우, 다음 항목 중 하나를 선택하여 외부 비상정지 기능을 활성화하십시오.<br>

- 기본 안전 입력 (Basic Safety Input)<br>
- 부가 안전 입력 (Extended Safety Input)<br>
- 안전 통신 입력 (Safety Communication Input)<br>

안전 입력 할당 기능은 아래의 메뉴를 통해 설정할 수 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:안전 입출력 할당<br>
![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)<br>
그림 3.1.4. T/P 화면 안전 입출력 할당 화면<br>

## 3.2. E00002 주축 리밋 스위치 작동중

### 1. 개요

로봇 각 축의 동작영역 끝에 설치한 리밋스위치가 작동하였습니다. 안전을 위하여 로봇은 즉각적으로 정지하며 적절한 방법으로 안전한 동작영역으로 이동할 때까지는 정상적인 운전을 할 수 없습니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1)	실제로 동작영역을 이탈한 것인지 확인하십시오.<br>
* 동작영역 이탈시의 복구방법<br>
(2)	동작영역 이탈이 아님에도 불구하고 에러가 발생하는 경우<br>
* 시스템보드 커넥터(CNLS)에서 점검하는 방법
* 와이어 하니스(C(M)ER1 또는 C(M)EC1)에서 점검하는 방법
* 리밋스위치 및 본체 내부 배선을 점검하는 방법
* 안전보드(BD632)를 점검하는 방법<br>
(3) 주축 리밋 스위치 회로의 배선 또는 접점에 이상이 발생한 경우<br>
(4) 주축 리밋 스위치에 대한 안전 입력 할당이 설정되지 않은 경우<br>
{% endhint %}

### (1) 실제로 동작영역을 이탈한 것인지 확인하십시오.

실제로 로봇이 동작영역 밖으로 벗어났는지 확인하십시오. 소프트리밋 에러도 동시에 발생하였다면 로봇은 동작영역을 이탈한 것입니다. 적절한 조작으로 로봇을 동작영역 안으로 이동시키십시오. 동작영역은 로봇 모델에 따라 다릅니다. 따라서, 리밋스위치의 설치위치도 다를 수 있으므로 해당 로봇의 보수설명서에서 “동작범위 제한” 부분을 참조하십시오.

![](../_assets/3-Safety-io/E00002/그림1.jpg)<br>
그림 3.2.1. 하드웨어 리밋스위치 설치 위치의 예(HS165/HS200 로봇)

![](../_assets/3-Safety-io/E00002/그림2.png)<br>
그림 3.2.2. 하드웨어 리밋스위치 작동 범위의 예(HS165/HS200 S축)

#### [동작영역 이탈시의 복구방법]
하드웨어 리밋스위치가 걸려있는 상태에서 로봇을 움직이기 위해서는 다음과 같은 조건과 순서로 실행해야 합니다.<br>
A)	수동모드에서 시스템 모드로 진입합니다. <br>
B)	티치펜던트에서 인에이블링스위치를 잡습니다.<br>

『수동모드』+ 『시스템』+ 『TP의 인에이블링 스위치 ON』<br>

C)	이 상태에서 모터 ON 시킵니다.<br>
D)	조그키를 사용하여 로봇을 동작영역 안으로 이동시킵니다.<br>

### (2)	동작영역 이탈이 아님에도 불구하고 에러가 발생하는 경우
우선 티칭펜던트의 전용 입력신호 창에서 리밋(Over-Travel) 항목이 계속 입력되고 있는지를 확인합니다. 이 창은 “『창조정』→『선택』→『시스템입력』”를 선택하면 볼 수 있습니다. 리밋(Over-Travel) 항목이 황색 표시가 되어 있는면 에러발생를 나타냅니다.<br>
### [주의]
수동모드에서는 티칭펜던트의 인에이블링 스위치를 ON 시켜야 모니터링이 됩니다. 자동모드에서는 인에이블링 스위치 상태와 관계없이 모니터링 됩니다.

![](../_assets/3-Safety-io/E00002/그림3.png)<br>
그림 3.2.3. 시스템 입력창에서 리밋(Over-Travel) 모니터링 표시

이와 같은 경우는 리밋스위치와 관계된 구성품들에서 원인을 찾을 수 있습니다. 리밋스위치는 다음 그림과 같이 본체로부터 CEC1 – CER1 케이블을 통하여 제어기의 서보안전 보드 또는 옵션 안전 IO 보드에 연결됩니다.

![](../_assets/3-Safety-io/E00002/hw_limit_sw_wire_0_en.png)<br>
그림 3.2.4. 하드웨어 리밋SW 배선 구조<br>

주요 점검 포인트와 순서는<br>
A1)	서보안전 보드(CNSI1) 또는<br>
A2) 옵션 안전 IO 보드(CNSI2)<br>
B)	제어기 내부의 배선 및 커넥터<br>
C)	와이어하니스 및 커넥터<br>
D)	리밋스위치 및 본체배선<br>

이며, 적절한 부위에서 리밋스위치의 입력선을 점퍼하여 모니터링 창에서 리밋(Over-Travel) 항목이 백색으로 변화하는지를 확인해야 합니다.<br>
다음의 순서에 따라 진행하십시오.

### [서보안전 보드 커넥터(CNSI1) 또는 옵션 안전IO 보드 커넥터(CNSI2)에서 점검하는 방법]

{% hint style="warning" %}
케이블의 연결 및 제거 시에는 반드시 제어기의 전원이 꺼진 상태에서 실행하십시오. 전기적 위험은 인명사고 및 재산사고를 일으킬 수 있습니다.<br>
{% endhint %}

#### * 서보안전 보드 커넥터(CNSI1) 점검 방법
서보안전 보드의 CNSI1 커넥터를 통해서 보드의 고장인지 판단하는 것입니다. 할당된 입력 채널과 관련된 핀을 점퍼쇼트 하십시오. 이 상태에서 전용입력신호 모니터링 창을 통하여 리밋(Over-Travel) 항목을 확인하십시오.<br>
① 백색으로 바뀌었다면, 서보안전 보드 고장입니다. 보드를 교체하십시오.<br>
② 황색으로 여전히 에러상태라면, 서보안전 보드 이후 본체 리밋스위치까지의 영역에서 고장을 체크하십시오.<br>
아래 그림은 리밋 스위치가 1번 채널에 할당되었을 때의 점퍼쇼트의 예입니다. 실제 할당된 채널에 점퍼쇼트 연결하여 시험하십시오.

![](../_assets/3-Safety-io/E00002/bd642_cnsi1_short.png)<br>
그림 3.2.5. 서보안전 보드 커넥터(CNSI1)<br>

#### * 옵션 안전IO 보드 커넥터(CNSI2) 점검 방법
옵션 안전IO 보드의 CNSI2 커넥터를 통해서 보드의 고장인지 판단하는 것입니다. 할당된 입력 채널과 관련된 핀을 점퍼쇼트 하십시오. 이 상태에서 전용입력신호 모니터링 창을 통하여 리밋(Over-Travel) 항목을 확인하십시오.<br>
① 백색으로 바뀌었다면, 옵션 안전IO 보드의 고장입니다. 보드를 교체하십시오.<br>
② 황색으로 여전히 에러상태라면, 옵션 안전IO 보드 이후 본체 리밋스위치까지의 영역에서 고장을 체크하십시오.<br>
아래 그림은 리밋 스위치가 3번 채널에 할당되었을 때의 점퍼쇼트의 예입니다. 실제 할당된 채널에 점퍼쇼트 연결하여 시험하십시오.

![](../_assets/3-Safety-io/E00002/bd680_si_short.png)<br>
그림 3.2.6. 하드웨어 리밋SW 배선 구조<br>

### [와이어하니스(C(M)ER1 또는 C(M)EC1)에서 점검하는 방법]
{% hint style="warning" %}<br>
케이블의 연결 및 제거 시에는 반드시 제어기의 전원이 꺼진 상태에서 실행하십시오. 전기적 위험은 인명사고 및 재산사고를 일으킬 수 있습니다.<br>
{% endhint %}

와이어하니스 커넥터 C(M)ER1 또는 C(M)EC1을 통해서 케이블 고장인지를 판단하는 것입니다. 우선 제어기로부터 C(M)EC1 와이어하니스 제거한 후, 제어기에 부착되어 있는 C(M)EC1 커넥터에서 리밋SW 관련 핀을 점퍼 쇼트하십시오. 이 상태에서 전용입력신호 모니터링 창을 통하여 리밋Over-Travel) 항목을 확인하십시오.<br>

① 백색으로 바뀌었다면,<br>
제어기 내부의 C(M)EC1 커넥터 – 시스템보드 간 케이블 또는 커넥터의 고장입니다. 이를 점검하거나 교체 하십시오.<br>
② 황색으로 여전히 에러상태라면,<br>
C(M)EC1 커넥터 이후 본체 리밋스위치까지의 영역에서 고장을 체크하십시오.<br>

C(M)EC1 와이어하니스를 다시 연력하고 본체로부터 C(M)ER1 와이어하니스를 제거한 후, 와이어하니스의C(M)ER1커넥터에서 리밋SW관련 핀을 점퍼쇼트하십시오. 이 상태에서 전용입력신호 모니터링 창을 통하여 리밋(Over-Travel) 항목의 상태를 확인하십시오.<br>

① 백색으로 바뀌었다면,<br>
C(M)ER1커넥터-C(M)EC1 커넥터 간 와이어하니스 케이블 또는 커넥터의 고장입니다. 이를 점검하거나 교체하십시오.<br>
② 황색으로 여전히 에러상태라면,<br>
본체 쪽 C(M)ER1 커넥터 이후 리밋SW까지의 영역에서 고장을 체크하십시오.<br>

### [리밋SW 및 본체 내부 배선을 점검하는 방법]

{% hint style="warning" %}<br>
케이블의 연결 및 제거 시에는 반드시 제어기의 전원이 꺼진 상태에서 실행하십시오. 전기적 위험은 인명사고 및 재산사고를 일으킬 수 있습니다.<br>
{% endhint %}

본체로부터 CER1 와이어하니스를 제거한 후, 본체의 CER1 커넥터에서 리밋SW 관련 라인에 이상이 있는지 멀티미터를 사용하여 쇼트 테스트하십시오.<br>
① 저항이 오픈상태로 측정되었다면,<br>
리밋SW 또는 리밋SW – CER1 간 커넥터 또는 커넥터의 고장입니다.
이를 점검하거나 교체하십시오.<br>
② 저항이 쇼트상태로 측정되었다면,<br>
다른 부분의 고장을 체크하여야 합니다. 당사에 문의하십시오.<br>

![](../_assets/3-Safety-io/E00002/그림8_en.png)<br>
그림 3.2.7. 하드웨어 리밋SW 하네스 C(M)ER 구조

### (3) 주축 리밋 스위치 회로의 배선 또는 접점에 이상이 발생한 경우
주축 리밋 스위치 배선을 점검하기 위해서는,먼저 주축 리밋 스위치 입력이 [안전 입출력 할당] 기능을 통해 어떤 입력 채널에 할당되어 있는지 확인하십시오.<br>
기본 설정의 경우, 주축 리밋 스위치는 비활성화 되어 있어 점검이 필요하지 않습니다. <br>
만약 사용이 필요하신 경우 [안전 입출력 할당] 기능을 통해 1)기본 안전, 2)부가 안전, 3)안전 통신 중 하나를 선택하여 사용이 가능합니다.

#### 3-1) 기본 안전 입력에 할당되어 있을 경우
주축 리밋 스위치 입력이 기본 안전입력에 할당되어 있는 경우, 서보안전 보드 CNSI1 커넥터(4채널)에 연결되어 있습니다. 위 항목 (1)의 CNSI1 커넥터에 할당된 채널을 확인하십시오. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.<br>

#### 3-2) 부가 안전 입력에 할당 되어 있는 경우 
주축 리밋 스위치 입력이 부가 안전입력에 할당되어 있는 경우, 옵션 안전IO 보드 CNSI2 커넥터(8채널)에 연결되어 있습니다. 위 항목 (1)의 CNSI2 커넥터에 할당된 채널을 확인하십시오. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 5.4.6.절을 참고하세요.<br>

#### 3-3) 안전 통신 입력에 할당 되어 있는 경우
주축 리밋 스위치 입력이 안전 통신입력에 할당되어 있는 경우, 'Hi7 로봇제어기 기능설명서-산업용 통신'메뉴얼을 참고하세요.<br>

### (4) 주축 리밋 스위치에 대한 안전 입력 할당이 설정되지 않은 경우<br>
외부 비상정지 입력이 안전 입력 할당에서 선택되지 않은 경우, 다음 항목 중 하나를 선택하여 외부 비상정지 기능을 활성화하십시오.

- 기본 안전 입력 (Basic Safety Input) 
- 부가 안전 입력 (Extended Safety Input)
- 안전 통신 입력 (Safety Communication Input)

안전 입력 할당 기능은 아래의 메뉴를 통해 설정할 수 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:입출력 할당<br>
![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)<br>
그림 3.2.8. T/P 화면 안전 입출력 할당 화면<br>

## 3.3. E02310 자동모드 안전가드 스위치 동작중

### 1. 개요
자동모드 안전가드 신호가 입력되었습니다.<br>
자동모드일 경우 안전을 확보하기 위해 로봇의 모든 모션은 즉시 정지되며,서보 모터는 모터 오프(Motor OFF) 상태로 전환됩니다.<br>

### 2. 원인 및 점검
{% hint style="info" %}<br>
(1)	실제로 자동모드 안전가드 신호가 입력된 경우<br>
(2) 자동모드 안전가드 회로의 배선 또는 접점에 이상이 발생한 경우<br>
(3) 자동모드 안전가드 신호에 대한 안전 입력 할당이 설정되지 않은 경우<br>
{% endhint %}

### (1)	실제로 자동모드 안전가드 신호가 입력된 경우
자동모드 안전가드(SGA) 스위치가 실제로 작동했는지 확인하십시오.
다른 작업자 또는 관리자가 자동모드 안전가드(SGA) 스위치을 작동시켰을 수 있습니다.<br>
또한, 안전 펜스 내부에서 작업자가 작업 중일 가능성이 있으므로 로봇 주변에 인원이 있는지, 또는 위험 요소(공구, 지그 등)가 존재하는지 확인하십시오.<br>
로봇을 재가동해도 안전하다고 판단되는 경우, 외부 비상정지 버튼을 해지한 후 수동 운전 모드에서 로봇을 먼저 동작시키십시오.

### (2) 자동모드 안전가드 회로의 배선 또는 접점에 이상이 발생한 경우
자동모드 안전가드 관련 배선을 점검하기 위해서는 먼저, 자동모드 안전가드 입력이 [안전 입출력 할당] 기능을 통해 어떤 입력 채널에 할당되어 있는지 확인하십시오.
기본 설정의 경우, 자동모드 안전가드 입력은 기본 안전 입력의 2번 채널에 할당되어 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:안전 입출력 할당<br>
![](../_assets/3-Safety-io/E02310/base_add_comm_si_func_sel.png)<br>
그림 3.3.1. T/P 화면 안전 입출력 할당 화면<br>

#### 2-1) 기본 안전입력에 할당되어 있는 경우
자동모드 안전가드 입력이 기본 안전입력에 할당되어 있는 경우, 서보안전 보드 CNSI1 커넥터(4채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

![](../_assets/3-Safety-io/E02310/bd642_cnsi1_position.png)<br>
그림 3.3.2. Hi7-N제어기 서보안전 보드 CNSI1 위치<br>

자동모드 안전가드 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 위 그림  T/P 화면 안전 입출력 할당 화면에서 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 서보안전 보드 CNSI1의 결선 표준은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

#### 2-2) 부가 안전입력에 할당되어 있는 경우 
자동모드 안전가드 입력이 부가 안전입력에 할당되어 있는 경우, 옵션 안전IO 보드 CNSI2 커넥터(8채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

![](../_assets/3-Safety-io/E02310/bd680_cnsi2_position.png)<br>
그림 3.3.3. Hi7-N제어기 옵션 안전IO 보드 CNSI2 위치<br>

자동모드 안전가드 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 위 그림  T/P 화면 안전 입출력 할당 화면에서 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 옵션 안전 IO 보드 CNSI2의 결선 표준은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

#### 2-3) 안전 통신입력에 할당되어 있는 경우
외부 비상정지 입력이 안전 통신입력에 할당되어 있는 경우, 'Hi7 로봇제어기 기능설명서-산업용 통신'메뉴얼을 참고하세요.

### (3) 자동모드 안전가드 신호에 대한 안전 입력 할당이 설정되지 않은 경우
자동모드 안전가드 입력이 안전 입력 할당에서 선택되지 않은 경우, 다음 항목 중 하나를 선택하여 자동모드 안전가드 기능을 활성화하십시오.<br>
- 기본 안전 입력 (Basic Safety Input) 
- 부가 안전 입력 (Extended Safety Input)
- 안전 통신 입력 (Safety Communication Input)<br>
안전 입력 할당 기능은 아래의 메뉴를 통해 설정할 수 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:입출력 할당
![](../_assets/3-Safety-io/N00088/io_alloc_param1.png)<br>
그림 3.3.4. T/P 화면 안전 입출력 할당 화면<br>

## 3.4. E02320 일반안전가드 스위치 동작중

### 1. 개요
일반안전가드 신호가 입력되었습니다.<br>
안전을 확보하기 위해 로봇의 모든 모션은 즉시 정지되며,서보 모터는 모터 오프(Motor OFF) 상태로 전환됩니다.

##### 2. 원인 및 점검
{% hint style="info" %}<br>
(1)	실제로 일반안전가드 신호가 입력된 경우<br>
(2) 일반안전가드 회로의 배선 또는 접점에 이상이 발생한 경우<br>
(3) 일반안전가드 신호에 대한 안전 입력 할당이 설정되지 않은 경우<br>
{% endhint %}

### (1)	실제로 일반안전가드 신호가 입력된 경우
일반안전가드(SGG) 스위치가 실제로 작동했는지 확인하십시오. 다른 작업자 또는 관리자가 일반안전가드(SGG) 스위치을 작동시켰을 수 있습니다.<br>
또한, 안전 펜스 내부에서 작업자가 작업 중일 가능성이 있으므로 로봇 주변에 인원이 있는지, 또는 위험 요소(공구, 지그 등)가 존재하는지 확인하십시오.<br>
로봇을 재가동해도 안전하다고 판단되는 경우, 외부 비상정지 버튼을 해지한 후 수동 운전 모드에서 로봇을 먼저 동작시키십시오.<br>

### (2) 일반안전가드 회로의 배선 또는 접점에 이상이 발생한 경우
일반안전가드 관련 배선을 점검하기 위해서는 먼저, 일반안전가드 입력이 [안전 입출력 할당] 기능을 통해 어떤 입력 채널에 할당되어 있는지 확인하십시오.<br>
기본 설정의 경우, 자동모드 안전가드 입력은 기본 안전 입력의 1번 채널에 할당되어 있습니다.

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:안전 입출력 할당<br>
![](../_assets/3-Safety-io/E02320/base_add_comm_si_func_sel.png)<br>
그림 3.4.1. T/P 화면 안전 입출력 할당 화면<br>

#### 2-1) 기본 안전입력에 할당되어 있는 경우
일반안전가드(SGG) 스위치 입력이 기본 안전입력에 할당되어 있는 경우, 서보안전 보드 CNSI1 커넥터(4채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

![](../_assets/3-Safety-io/E02320/bd642_cnsi1_position.png)<br>
그림 3.4.2. Hi7-N제어기 서보안전 보드 CNSI1 위치<br>

일반안전가드(SGG) 스위치 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 위 그림  T/P 화면 안전 입출력 할당 화면에서 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 서보안전 보드 CNSI1의 결선 표준은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

#### 2-2) 부가 안전입력에 할당되어 있는 경우 
일반안전가드(SGG) 스위치 입력이 부가 안전입력에 할당되어 있는 경우, 옵션 안전IO 보드 CNSI2 커넥터(8채널)에 연결되어 있습니다. 해당 커넥터의 자세한 핀맵은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

![](../_assets/3-Safety-io/E02320/bd680_cnsi2_position.png)<br>
그림 3.4.3. Hi7-N제어기 옵션 안전IO 보드 CNSI2 위치<br>

일반안전가드(SGG) 스위치 입력이 어떤 채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 위 그림  T/P 화면 안전 입출력 할당 화면에서 확인 가능합니다.<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 옵션 안전 IO 보드 CNSI2의 결선 표준은 'Hi7 제어기 보수 설명서' 5.4.6.절을 참고하세요.

#### 2-3) 안전 통신입력에 할당되어 있는 경우
외부 비상정지 입력이 안전 통신입력에 할당되어 있는 경우, 'Hi7 로봇제어기 기능설명서-산업용 통신'메뉴얼을 참고하세요.

### (3) 일반안전가드 신호에 대한 안전 입력 할당이 설정되지 않은 경우
일반안전가드 입력이 안전 입력 할당에서 선택되지 않은 경우, 다음 항목 중 하나를 선택하여 일반안전가드 기능을 활성화하십시오.<br>
- 기본 안전 입력 (Basic Safety Input) 
- 부가 안전 입력 (Extended Safety Input)
- 안전 통신 입력 (Safety Communication Input)<br>

안전 입력 할당 기능은 아래의 메뉴를 통해 설정할 수 있습니다.<br>

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:입출력 할당<br>
![](../_assets/3-Safety-io/E02320/io_alloc_param1.png)<br>
그림 3.4.4. T/P 화면 안전 입출력 할당 화면<br>
## 3.5. E51431 (A ch) 전자접촉기 피드백 이상

### 1. 개요
전자접촉기(Magnetic contactor)가 동작하지 않았습니다.

### 2. 원인 및 점검 방법
{% hint style="info" %}
(1)	모니터링 계통을 점검하십시오.<br>
(2)	마그네트 MC를 점검하십시오.<br>
(3)	전장보드를 점검하십시오.<br>
(4)	전원공급모듈(H6PSM30)를 점검하십시오.<br>
(5)	서보앰프를 점검하십시오.<br>
{% endhint %}

### (1)	모니터링 계통을 점검하십시오.
전자접촉기가 설치되어 있는 전장모듈(PSM or PDM)과 모니터링 신호를 수집하는 서보안전 보드 간의 케이블링을 확인합니다. 케이블 이름은 CNPRC, CNPRC1이며 서보안전 보드의 신호가 백플레인 보드를 통하여 전장모듈로 들어 갑니다. 이 케이블의 커넥터 접속상태를 점검하십시오.

![](../_assets/3-Safety-io/E51431/cnprc_cable.png)<br>
그림 3.5.1 Hi7-N제어기

### (2)	마그네트 MC를 점검하십시오.
전장모듈 내부에 있는 마그네트 MC1, MC2가 정상적으로 동작하는지 점검하십시오.

![](../_assets/3-Safety-io/E51431/psm_mc1_mc2.png)<br>
그림 3.5.2 Hi7-N제어기(전장모듈의 내부에 설치된 마그네트 MC1, MC2)

### (3)	전장보드를 점검하십시오.

서보안전 보드와 마그네트를 중계하는 전장보드, 케이블 배선에 문제가 있을 수 있으므로 점검 또는 교체하십시오.

![](../_assets/3-Safety-io/E51431/psm_inner_cables.png)<br>
그림 3.5.3 Hi7-N제어기(전장모듈의 내부에 설치된 전장보드)

### (4)	서보안전 보드를 교체 시험하십시오.

서보안전 보드를 교체한 후 에러가 발생하지 않으면 서보안전 보드의 전자접촉기 제어 및 피드백 부분의 고장으로 판단할 수 있습니다.

![](../_assets/3-Safety-io/E51431/hi7_controller_bd642.png)<br>
그림 3.5.4 Hi7-N제어기 서보안전보드 교체

## 3.6. E52042 (0 ch) 안전 입력 신호의 불일치

{% hint style="warning" %}
안전입력 결선 확인작업 시, 반드시 제어기 전원을 OFF한 상태에서 확인작업 하시기 바랍니다.
{% endhint %}

### 1. 개요

기본 안전입력 채널에서 이중화된 안전 입력 신호 간 불일치가 감지되었습니다.<br>
안전을 확보하기 위해 해당 입력 신호는 **Fail-Safe 상태(Open 또는 0)**로 처리됩니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1) 배선의 오류 또는 단선에 의한 신호 차이 발생
(2) 단자대 및 케이블 상태에 의한 노이즈 발생
(3) 안전 신호 파라미터의 설정 오류 (필터, 불일치 허용 시간)
{% endhint %}

### (1) 배선의 오류 또는 단선에 의한 신호 차이 발생

안전입력 신호 불일치는 서보안전 보드 CNSI1 커넥터(총 4채널)에 연결된 안전입력 신호의 불일치를 나타냅니다. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

![](../_assets/3-Safety-io/E52042/bd642_cnsi1_position.png)<br>
그림 3.6.1. Hi7-N제어기 서보안전 보드 CNSI1 위치

1) 안전 입력 신호를 사용하지 않는 경우<br>
해당 에러가 발생된 채널이 사용하지 않는 채널인 경우, 외부 결선은 아래와 같이 되어 있는지 배선을 확인합니다. 또한, 커넥터와 와이어 간 접촉이 제대로 조립되어 있는지 확인합니다.
<br>
![](../_assets/3-Safety-io/E52042/bd642_cnsi1_notused.png)<br>
그림 3.6.2. 서보안전 보드 CNSI1 사용하지 않는 경우 결선도<br>
<br>
2) 안전 입력 신호를 사용하는 경우<br>
해당 에러가 발생된 채널이 사용되는 경우, 해당 입력채널이 어떤 입력채널에 할당되어 있는지 확인하십시오. 입력채널의 할당은 아래 메뉴를 통해 확인 가능합니다.
<br>
<br>
시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:입출력 할당<br>
![](../_assets/3-Safety-io/E52042/io_alloc_param1.png)<br>
그림 3.6.3. T/P 화면 안전 입력 할당 화면<br>
<br>
해당 입력채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 제대로 배선되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 서보안전 보드 CNSI1의 결선 표준은 Hi7 제어기 보수 설명서 4.3.2.6.절을 참고하세요.

### (2) 단자대 및 케이블 상태에 의한 노이즈 발생
#### 안전입력 신호의 모니터링 기능<br>
안전입력 신호에 대한 모니터링 화면이 T/P에 구성되어 있습니다. 0.5초 주기로 모니터링이 가능하므로 기본적인 확인은 가능합니다.

시스템 -> 8: 안전시스템 -> 3: 모니터링 -> 3: 안전 IO 상태<br>
![](../_assets/3-Safety-io/E52042/safety_io_status.png)<br>
그림 3.6.4. T/P 화면 안전 IO 모니터링 화면<br>

### (3) 안전 신호 파라미터의 설정 오류 (필터, 불일치 허용 시간)
안전입력 신호의 필터 시간이 너무 짧거나, 불일치 허용시간이 과도하게 짧게 설정된 경우, 안전입력 신호 불일치 알람이 빈번하게 발생할 수 있습니다.<br>
기본적으로 권장하는 안전 입력 신호의 설정 값은 아래와 같습니다. 해당 값은 현장 환경 및 적용 조건에 따라 조정하여 사용할 수 있습니다.

- 필터 시간 : 100 (msec)
- 불일치 허용 시간 : 1000 (msec)

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 2:기본 입출력<br>
![](../_assets/3-Safety-io/E52042/def_input.png)<br>
그림 3.6.5. T/P 화면 기본 입출력 설정 화면<br>## 3.7. E52043 (0 ch) 부가 안전 입력 신호의 불일치

{% hint style="warning" %}
부가 안전입력 결선 확인작업 시, 반드시 제어기 전원을 OFF한 상태에서 확인작업 하시기 바랍니다.
{% endhint %}

### 1. 개요

부가 안전입력 채널에서 이중화된 안전 입력신호 간 불일치가 감지되었습니다.<br>
안전을 확보하기 위해 해당 입력 신호는 **Fail-Safe 상태(Open 또는 0)**로 처리됩니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1) 배선의 오류 또는 단선에 의한 신호 차이 발생
(2) 단자대 및 케이블 상태에 의한 노이즈 발생
(3) 안전 신호 파라미터의 설정 오류(필터, 불일치 허용 시간)
{% endhint %}

### (1) 배선의 오류 또는 단선에 의한 신호 차이 발생
부가 안전입력 신호 불일치는 옵션 안전IO 보드 CNSI2 커넥터(총 8채널)에 연결된 부가 안전입력 신호의 불일치를 나타냅니다. 해당 커넥터의 자세한 핀맵은 Hi7 제어기 보수 설명서 5.4.6.절을 참고하세요.

![](../_assets/3-Safety-io/E52043/bd680_cnsi2_position.png)<br>
그림 3.7.1. Hi7-N제어기 옵션 안전IO 보드 CNSI2 위치<br>

1) 부가 안전입력 신호를 사용하는 경우<br>
해당 에러가 발생된 채널이 사용되는 경우, 해당 입력채널이 어떤 입력채널에 할당되어 있는지 확인하십시오. 부가 안전입력 채널의 할당은 아래 메뉴를 통해 확인 가능합니다.
<br>
시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 1:안전 입출력 할당 -> 확장 입력<br>
![](../_assets/3-Safety-io/E52043/add_si_func_sel.png)<br>
그림 3.7.2. T/P 화면 부가 안전 입출력 할당 화면<br>
<br>
해당 부가 안전입력 채널 할당된 것이 확인되면 해당 현장의 전기도면 또는 배선도면을 참조하여 도면과 실제 배선이 제대로 되어 있는지 확인합니다. 또한, 실제 배선을 확인하면서 연결 또는 조립 상태를 확인합니다.<br>
전기도면 또는 배선도면 확인 시, 옵션 안전 IO 보드 CNSI2의 결선 표준은 Hi7 제어기 보수 설명서 5.4.6.절을 참고하세요.

### (2) 단자대 및 케이블 상태에 의한 노이즈 발생

#### 부가 안전입력 신호의 모니터링 기능<br>
부가 안전입력 신호에 대한 모니터링 화면이 T/P에 구성되어 있습니다. 0.5초 주기로 모니터링이 가능하므로 기본적인 확인은 가능합니다.

시스템 -> 8: 안전시스템 -> 3: 모니터링 -> 3: 안전 IO 상태<br>
![](../_assets/3-Safety-io/E52043/add_si_monitoring.png)<br>
그림 3.7.3. T/P 화면 안전 IO 모니터링 화면<br>

### (3) 안전 신호 파라미터의 설정 오류 (필터, 불일치 허용 시간)

부가 안전입력 신호의 필터 시간이 너무 짧거나, 불일치 허용 시간이 과도하게 짧게 설정된 경우, 부가 안전입력 신호 불일치 알람이 빈번하게 발생할 수 있습니다.<br>
기본적으로 권장하는 부가 안전입력 신호의 설정 값은 아래와 같습니다. 해당 값은 현장 환경 및 적용 조건에 따라 조정하여 사용할 수 있습니다.<br>
- 필터 시간 : 100 (msec)
- 불일치 허용 시간 : 1000 (msec)

시스템 -> 8: 안전시스템 -> 2: 파라미터 설정 -> 3: 안전 IO -> 3:확장 입출력<br>
![](../_assets/3-Safety-io/E52043/add_io.png)<br>
그림 3.7.4. T/P 화면 부가 안전 입출력 설정 화면<br>
# 4. Servo Safety Board (Servo Part)## 4.1. E02470. (O Axis) Encoder Error: Reset Required

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

![](../_assets/4.서보보드/encoder_reset.png)<br>
Figure 4.1.2 Serial Encoder Reset

(2)	Inspect the encoder battery wiring status.<br>
Check the battery wiring status connecting from the encoder battery location to the motor.

(3)	Perform a motor replacement test.<br>
If the problem is not resolved by the above measures, it is highly likely that the encoder itself is faulty. Perform a motor replacement test.

    
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

![](../_assets/4.서보보드/USB_check.png)<br>
Figure 4.2.2 TP USB Recognition

Enter the following path to back up files.

    Service -> 5. File Manager

![](../_assets/4.서보보드/backup_1.png)<br>
Figure 4.2.3 Backup Step 1

![](../_assets/4.서보보드/backup_2.png)<br>
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

![](../_assets/4.서보보드/tool_data_screen.png)<br>
Figure 4.3.1 Check Tool Data

To automatically set the tool weight or inertia, you can use the load estimation function in the menu below. 

* Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation Function

![](../_assets/4.서보보드/load_estimation_1.png)<br>
Figure 4.3.2 Load Estimation Function 1

![](../_assets/4.서보보드/load_estimation_2.png)<br>
Figure 4.3.3 Load Estimation Function 2

![](../_assets/4.서보보드/load_estimation_3.png)<br>
Figure 4.3.4 Load Estimation Function 3

* Select the tool number to save after estimating the load using the load estimation function.

![](../_assets/4.서보보드/load_estimation_4.png)<br>
Figure 4.3.5 Load Estimation Function 4

* Click Normal Operation to execute.<br>
Press the Motor On switch, hold the deadman switch, and then click Normal Operation.

![](../_assets/4.서보보드/load_estimation_5.png)<br>
Figure 4.3.6 Load Estimation Function 5

* When the load estimation operation is completed, the estimation result is displayed on the screen.

![](../_assets/4.서보보드/load_estimation_6.png)<br>
Figure 4.3.7 Load Estimation Function 6

(2)	Check if the robot model is set correctly.

![](../_assets/4.서보보드/robot_model_check.png)<br>
Figure 4.3.8 Check Robot Model

Check if the robot model registered on the TP screen matches the actually installed robot.

(3)	Check the versions of the servo safety board (BD642) and main com.<br>
This may occur due to broken compatibility between the servo safety board (BD642) and the main com version. Especially if a module has been replaced, proceed with a version update to match the version of each module to the current main com version.

The version of each module can be checked in the path below.

        Service -> 7. System Diagnosis -> 1. System Version


![](../_assets/4.서보보드/tp_version_check_screen.png)<br>
Figure 4.3.9 Module Version Check

(4)	Check if the robot posture is near a singularity.<br>
If L interpolation or C interpolation, rather than PtP interpolation, is executed in a posture near a singularity, an error may occur. A singularity occurs when the B-axis is close to 0 deg and when the center of the wrist is close to the S-axis rotation center axis. When passing near a singularity, please change the corresponding step to PtP interpolation.

![](../_assets/4.서보보드/robot_special_action.png)<br>
Figure 4.3.10 Singularity Posture Check

(5)	For external axes, check the acceleration/deceleration parameter settings and the load factor during operation.<br>
The motor torque may be insufficient because the maximum speed of the external axis acceleration/deceleration parameter is too high or the acceleration time is too short. While observing the load factor during robot operation, you must lower the I/Ip maximum speed or significantly increase the acceleration time.

        System -> 3. Robot Parameter -> 34. Acc/Dec Parameter

![](../_assets/4.서보보드/add_axis_accdec.png)<br>
Figure 4.3.11 External Axis Acc/Dec Check

(6)	Adjust the job program.<br>
Change the step conditions of the corresponding step or the immediately preceding step in the job program. First, try changing it to “Acc=0”, second, try lowering the speed of the step, and third, try adding a step to the movement path to change the program conditions.

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
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the HS165 robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.4.8 Motor Positions for Each Axis of HS165 Robot

(5)	Check the communication status of the wiring after completing the measures.<br>
After the measures for the problematic part are completed, check the communication status by referring to the 『Encoder Communication Failure Count Display Function Manual』.

![](../_assets/4.서보보드/encoder_comm_fail_screen.png)
Figure 4.4.9 Encoder Communication Failure Monitoring

![](../_assets/4.서보보드/encoder_comm_fail_number_en.png)

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
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the HS165 robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.5.5 Motor Positions for Each Axis of HS165 Robot

(3)	Perform a servo safety board replacement test.<br>
If the error does not occur after replacing the servo safety board, the servo safety board is faulty. Please replace the servo safety board with a normal unit.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.5.6 N Controller Servo Safety Board Replacement

(4)	Check the communication status of the wiring after completing the measures.<br>
After the measures for the problematic part are completed, check the communication status by referring to the 『Encoder Communication Failure Count Display Function Manual』.

![](../_assets/4.서보보드/encoder_comm_fail_screen.png)<br>
Figure 4.5.7 Encoder Communication Failure Monitoring

![](../_assets/4.서보보드/encoder_comm_fail_number_en.png)

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

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".## 4.7. E50104. (O Axis) CRC error deteced in encoder data

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

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".## 4.9. E50106. (O Axis) Encoder data abnormal variation detected

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

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".## 4.10. E50107. (O Axis) Encoder line open detected (Motor On)

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

For detailed inspection methods, refer to "E50101 (O Axis) Invalid encoder command field setting".## 4.11. E50108. (O Axis) Encoder Counting error (CE Bit Detected)

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

![](../_assets/4.서보보드/encoder_error_release.png)<br>
Figure 4.11.3 Serial Encoder Error Release

(3) If the error persists, perform a motor (encoder) replacement test.<br>
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the HS165 robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.11.4 Motor Positions for Each Axis of HS165 Robot

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

For detailed inspection methods, refer to "E50108 (O Axis) Encoder Counting error".## 4.14. E50111. (O Axis) Encoder Counting error

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

![](../_assets/4.서보보드/encoder_error_release.png)<br>
Figure 4.15.1 Encoder Error Release

(2) Check the encoder battery voltage.<br>
The encoder battery is 3.6V. If this voltage drops to 3.0V~3.2V, “W0104 ○ Axis Encoder Battery Voltage Low” is displayed. When this warning occurs, the encoder battery must be replaced. Encoder battery replacement must be performed while the controller power is ON. If you replace it with a normal encoder battery in this state, you can continue to use the robot without any problems.

If the encoder battery replacement time is passed and the voltage drops to 2.5V~3.0V, the error “E2470 ○ Axis Encoder Abnormal: Encoder Reset Required” occurs when the controller power is turned ON. If this error occurs, the encoder position data has already been lost. After replacing the encoder battery and resetting the encoder, you must move the robot to the reference posture using manual operation in the axis coordinate system and perform encoder calibration for the corresponding axis again.

![](../_assets/4.서보보드/battery_replace_position.png)<br>
Figure 4.15.2 Encoder Battery Replacement Position

Encoder reset is performed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Encoder Reset

![](../_assets/4.서보보드/encoder_reset.png)<br>
Figure 4.15.3 Encoder Reset

(3) Check the encoder battery connection status.<br>
Check the status of the battery wiring connecting from the encoder battery location to the motor.


(4) Perform a motor (encoder) replacement test.<br>
If the error persists upon main power OFF/ON after resetting the error, perform a motor (encoder) replacement test. If the error does not occur after replacement, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the HS165 robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.15.4 Motor Positions for Each Axis of HS165 Robot

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
If the error does not occur after replacing the servo motor, the servo motor is faulty. Please replace the servo motor with a normal unit. The figure below shows the positions of motors for each axis of the HS165 robot. For other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/HS165_motor_position.png)<br>
Figure 4.16.1 Motor (Encoder) Replacement Position

(2)	Check the operating conditions (speed, load, etc.).<br>
Check the saturated encoder temperature while running the Job program. Encoder temperature can be checked as follows.

    Engineering Mode -> Window Adjustment -> System Characteristics -> System Characteristics List - Motor/Encoder

![](../_assets/4.서보보드/encoder_temp.png)<br>
Figure 4.16.2 Checking Encoder Temperature

(3)	Check the ambient temperature around the encoder.<br>
Errors may occur if the encoder's internal temperature rises due to the external temperature.

(4)	Perform a servo safety board replacement test.<br>
If the error does not occur after replacing the servo safety board, it can be determined that the encoder data receiving section of the servo board is faulty.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.16.3 N Controller Servo Board Replacement

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

![](../_assets/4.서보보드/load_estimation_1.png)<br>
Figure 4.17.1 Load Estimation Function 1

![](../_assets/4.서보보드/load_estimation_2.png)<br>
Figure 4.17.2 Load Estimation Function 2

![](../_assets/4.서보보드/load_estimation_3.png)<br>
Figure 4.17.3 Load Estimation Function 3

* Select the tool number to save after estimating the load using the load estimation function.

![](../_assets/4.서보보드/load_estimation_4.png)<br>
Figure 4.17.4 Load Estimation Function 4

* Click Normal Operation to execute.
Press the Motor On switch, hold the deadman switch, and then click Normal Operation.

![](../_assets/4.서보보드/load_estimation_5.png)<br>
Figure 4.17.5 Load Estimation Function 5

* When the load estimation operation is completed, the estimation result is displayed on the screen.

![](../_assets/4.서보보드/load_estimation_6.png)<br>
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

![](../_assets/4.서보보드/axis_lock_1.png)<br>
Figure 4.17.7 Axis Lock Setting Screen 1

![](../_assets/4.서보보드/axis_lock_2.png)<br>
Figure 4.17.8 Axis Lock Setting Screen 2

![](../_assets/4.서보보드/axis_lock_3.png)<br>
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

![](../_assets/4.서보보드/엔코더온도및재생속도.png)<br>
Figure 4.18.1 Encoder Temperature Check Screen
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

![](../_assets/4.서보보드/robot_model_check.png)<br>
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

![](../_assets/4.서보보드/robot_model_check.png)<br>
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

![](../_assets/4.서보보드/robot_model_check.png)<br>
Figure 4.21.1 TP Robot Model Check

Check if the registered robot model on the TP screen matches the actually installed robot.

(3) Check if the brake release is operating normally.<br>
There may be a problem with the release function of the brake for the corresponding axis or an abnormality in the brake release voltage.

* Inspection of individual axis brake release anomalies<br>
Use the Axis Lock function to verify the operation of the brake release function for the corresponding axis.
Lock the axes except for the axis you want to verify, then repeat Motor ON/OFF to check if the brake release sound ("click") is heard from the motor of the mechanical unit.<br>
The method to use the Axis Lock function is as follows.

        System -> 5. Initialization -> 9. Axis Lock Setting -> Confirm -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock_1.png)<br>
Figure 4.21.2 Axis Lock Setting Screen 1

![](../_assets/4.서보보드/axis_lock_2.png)<br>
Figure 4.21.3 Axis Lock Setting Screen 2

![](../_assets/4.서보보드/axis_lock_3.png)<br>
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

![](../_assets/4.서보보드/position_error_monitor_screen.png)<br>
Figure 4.21.8 Position Deviation Max Measurement Monitoring Screen<br>

![](../_assets/4.서보보드/position_error_change_screen.png)<br>
Figure 4.21.9 Position Deviation Setting Change Screen

(7) Check the versions of the servo safety board (BD642) and the main com.<br>
This may occur if the compatibility between the servo safety board (BD642) and the main com version is broken. Especially, if a module has been replaced, proceed with a version upgrade to match the version of each module to the current main com version. The version of each module can be checked in the path below.

                Service -> 7. System Diagnosis -> 1. System Version

![](../_assets/4.서보보드/tp_version_check_screen.png)<br>
Figure 4.21.10 TP Module Version Check Window

(8) Replace other components.<br>
Replace components in the order of Servo Safety Board (BD642) → Servo Drive Unit → Power Electric Module → Motor to check for error occurrence.

![](../_assets/4.서보보드/hi7_robot_brake_power_check.png)<br>
Figure 4.21.11 Hi7-N Controller Motor and Drive Module




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

For detailed inspection methods, please refer to "E50400 (O Axis) Position Deviation exceeded".## 4.23. E50402. (O Axis) Position Deviation Exceeded (Cold Temperature Friction Increase)

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

![](../_assets/4.서보보드/엔코더온도및재생속도.png)<br>
Figure 4.23.1 Encoder Temperature Check Screen

(2)	Check if the robot model is set correctly.

![](../_assets/4.서보보드/robot_model_check.png)<br>
Figure 4.23.2 Robot Model Check

Check if the registered robot model on the TP screen matches the actually installed robot.## 4.24. E51429 Initial Charging Resistor Relay Feedback Error

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
Inspect the internal wiring of the controller. In the case of the Hi6-N controller, inspect the wiring between the CNPB1 (BD640) connector and the CNPB1 (power board) connector.

![](../_assets/4.서보보드/brake_pwr_cable.png)<br>
Figure 4.26.2 N Controller Brake Power Inspection

(3)    Perform a replacement test of the servo safety board.<br>
If the error does not occur after replacing the servo safety board, it can be determined as a failure of the encoder data receiving part of the servo board.

![](../_assets/4.서보보드/hi7_controller_bd642.png)<br>
Figure 4.26.3 N Controller Servo Board Replacement

# 5. 통신## 5.1. E29003 전장 보드 통신 오류 (EtherCAT 연결 끊김)

### 1. 개요

전장 보드 통신 오류 (EtherCAT 연결 끊김)가 발생하였습니다. 메인제어모듈(H6COM-T)과 전장 보드(BD642, BD681 등)간의 통신이 끊어졌습니다.

### 2. 원인

{% hint style="info" %}

(1) 보드 간 통신 케이블 결선상태 및 케이블을 확인하십시오.<br>
(2) 전장 보드를 점검하십시오.<br>

<br>
전장 보드는 사용하는 환경에 따라 연결 구성이 다릅니다.<br>
- 서보안전 보드(BD642) 단독 사용<br>
- 서보안전 보드(BD642), 사용자DIO 보드(BD681) 사용<br>

{% endhint %}

### (1)	보드 간 통신 케이블 결선 상태 확인.
### [각 모듈간(메인제어모듈(H6COM-T), 전장보드) Ethernet 케이블 결선 상태 확인]

![](../_assets/5-Communication/ethercat_cable_hicom_bd642_r2.png)<br>
그림 5.1.1 H6COM-T와 BD642의 EtherCAT 케이블 연결

<br>

![](../_assets/5-Communication/BD642_BD681_cable_connection.png)<br>
그림 5.1.2 BD642와 BD681 EtherCAT 케이블 연결 **(BD681 사용 시)**

1)	점검 대상<br>
A.	메인제어모듈(H6COM-T) ↔ 서보안전 보드(BD642) 간 Ethernet 케이블<br>
B.	서보안전 보드(BD642) ↔ 사용자DIO 보드(BD681) 간 Ethernet 케이블 **(BD681 사용 시)**<br>
2)	점검 항목<br>
A.	케이블 양쪽 커넥터가 확실히 체결되어 있는지 확인합니다.<br>
B.	케이블에 단선, 압착 손상, 꺾임, 파손이 없는지 육안 점검합니다.<br>
C.	커넥터 핀(단자)에 녹, 오염, 휘어짐이 없는지 확인합니다.<br>
3)	점검 방법<br>
A.	전원을 OFF한 상태에서 케이블 분리 및 재삽입을 수행합니다.<br>
B.	삽입 시 '딸깍' 소리가 나도록 완전히 체결되도록 합니다.<br>
C.	필요한 경우 예비 케이블로 교체 후 재시도합니다.<br>
D.	연결 순서 및 올바른 LAN Port와 연결되어 있는지 재확인합니다.<br>
4)	추가 확인<br>
A.	반복적으로 끊김이 발생할 경우, 케이블 내부 단선 가능성 고려 → 케이블 교체가 필요할 수도 있습니다.<br>
B.	이더넷 커넥터(PCB 단자부) 손상 가능성도 점검하시기 바랍니다.<br>
C.	전장 보드 장치 자체에 Link/Act LED 상태를 확인합니다.<br>
    * 정상: 녹색(좌) 점멸, 황색(우) 점등 <br>
    * 비정상: 녹색(좌) & 황색(우) 꺼짐 또는 점등 상태 유지<br>
    
![](../_assets/5-Communication/E29003/그림2.png)<br>


### (2) 전장 보드를 점검하십시오.
#### [서보안전 보드(BD642)를 점검하는 방법]
![](../_assets/5-Communication/BD642_LED.png)<br> 
그림 5.1.3 BD642보드 LED, Segment 

<br>

![](../_assets/5-Communication/BD642_7-Segment.png)<br> 
그림 5.1.4 7-Segment 상태 정보

<br>

1) 통신 연결 상태 확인<br>
   '그림 5.1.3'의 4 ~ 5번 초록색 LED가 켜져있는지 확인하십시오. <br>

2) 정상 부팅 상태 확인<br>
   메인제어모듈 (H6COM-T)이 완전히 부팅되고 난 후(전원투입후 약 50초 정도 소요) <br>
   '그림 5.1.3'의 1 ~ 5번 초록색 LED가 켜져있고 6 ~ 10번 빨간색 LED가 꺼저있으며,<br> 7-Segment가 '2. Safe State' 상태로 점이 점멸 되어야합니다.<br>

1~2번 항목의 점검사항이 모두 이상이 없는 경우에도 통신 연결에 문제가 있는 경우 보드를 교체 하십시오.<br>

 
#### [사용자DIO 보드(BD681)를 점검하는 방법]
![](../_assets/5-Communication/BD681_LED.png)<br> 
그림 5.1.5 BD681보드 LED 

<br>
 
1)	통신 연결 상태 확인<br>
A.	'그림 5.1.5'의 3번 초록색 LED가 켜져있는지 확인하십시오.<br>

2)	정상 동작 상태 확인<br>
A.	'그림 5.1.5'의 1 ~ 2번 초록색 LED가 점멸 상태 인지를 확인하십시오.<br>

1~2번 항목의 점검사항이 모두 이상이 없는 경우에도 통신 연결에 문제가 있는 경우 보드를 교체하십시오.<br>
## 5.2. E29016 전장보드 통신(EtherCAT) 마스터 연결 끊김 발생

### 1. 개요

전장보드 통신(EtherCAT) 마스터와 연결되는 첫번째 장치와의 연결이 끊어 졌습니다.

### 2. 원인

{% hint style="info" %}

(1) 보드 간 통신 케이블 결선 상태를 확인하십시오.<br>
(2) 서보안전 보드(BD642)를 점검하십시오.<br>

{% endhint %}

### (1) 보드 간 통신 케이블 결선 상태 확인.

#### [각 모듈간(메인제어모듈(H6COM-T), 서보안전 보드(BD642)) Ethernet 케이블 결선 상태 확인]
![](../_assets/5-Communication/ethercat_cable_hicom_bd642_r1.png)<br>
그림 5.2.1 Hi7-N제어기 EtherCAT 케이블 연결

1)	점검 대상<br>
A.	메인제어모듈(H6COM-T) ↔ 서보안전 보드(BD642) 간 Ethernet 케이블<br>
2)	점검 항목<br>
A.	케이블 양쪽 커넥터가 확실히 체결되어 있는지 확인<br>
B.	케이블에 단선, 압착 손상, 꺾임, 파손이 없는지 육안 점검<br>
C.	커넥터 핀(단자)에 녹, 오염, 휘어짐이 없는지 확인<br>
3)	점검 방법<br>
A.	전원을 OFF한 상태에서 케이블 분리 및 재삽입 수행<br>
B.	삽입 시 '딸깍' 소리가 나도록 완전히 체결<br>
C.	필요한 경우 예비 케이블로 교체 후 재시도<br>
D.	연결 순서 및 올바른 LAN Port와 연결되어 있는지 재확인<br>
4)	추가 확인<br>
A.	서보안전 보드(BD642) 장치 자체에 Link/Act LED 상태 확인<br>
- 정상: 녹색(좌) 점멸, 황색(우) 점등 <br>
- 비정상: 녹색(좌) & 황색(우) 꺼짐 또는 점등 상태 유지<br>
![](../_assets/5-Communication/E29016/그림2.png)<br>
B.	반복적으로 끊김이 발생할 경우, 케이블 내부 단선 가능성 고려 → 케이블 교체 필요<br>
C.	이더넷 커넥터(PCB 단자부) 손상 가능성도 점검<br>

### (2) 서보안전 보드(BD642)를 점검하십시오.
#### [서보안전 보드(BD642)를 점검하는 방법]
![](../_assets/5-Communication/BD642_LED.png)<br> 
그림 5.2.2 BD642보드 LED, Segment 

<br>

![](../_assets/5-Communication/BD642_7-Segment.png)<br> 
그림 5.2.3 7-Segment 상태 정보

<br>

1) 통신 연결 상태 확인<br>
   '그림 5.2.2'의 4 ~ 5번 초록색 LED가 켜져있는지 확인하십시오. <br>

2) 정상 부팅 상태 확인<br>
   메인제어모듈 (H6COM-T)이 완전히 부팅되고 난 후(전원투입후 약 50초 정도 소요) <br>
   '그림 5.2.2'의 1 ~ 5번 초록색 LED가 켜져있고 6 ~ 10번 빨간색 LED가 꺼저있으며,<br> 7-Segment가 '2. Safe State' 상태로 점이 점멸 되어야합니다.<br>

1~2번 항목의 점검사항이 모두 이상이 없는 경우에도 통신 연결에 문제가 있는 경우 보드를 교체 하십시오.<br>
## 5.3. 전장보드 통신(EtherCAT) 마스터 ENI 불일치

### 1. 개요

제어기 통신 연결 구성과 설정된 ENI파일이 불일치 합니다.<br>
(ENI : EtherCAT Network Information)

### 2. 원인

{% hint style="info" %}

설정된 ENI파일과 일치하지 않는 제어기 통신 연결 구성입니다.<br>

{% endhint %}

### 제어기 통신 연결 구성 확인.

기본적으로 제어기에서 사용할 수 있는 통신 연결 구성이 있습니다. 올바르지 않은 통신 연결로 구성할 경우 정상적으로 사용할 수 없습니다.<br>
또한 통신 커넥터의 [IN] / [OUT]을 구별하여 연결 해야 합니다. '1번 보드의 [OUT] 커넥터' - '2번 보드의 [IN] 커넥터' 이런 방식으로 올바른 커넥터에 연결해야 정상적으로 통신할 수 있습니다.<br>

<strong><올바른 통신 연결 구성 예시></strong><br>

- 메인제어모듈(H6COM-T) ↔ **[IN]** 서보안전 보드(BD642)
- 메인제어모듈(H6COM-T) ↔ **[IN]** 서보안전 보드(BD642) **[OUT]** ↔ **[IN]** 사용자DIO 보드(BD681)

<br>

<strong><올바르지 않은 통신 연결 구성 예시></strong><br>

- 메인제어모듈(H6COM-T) ↔ **[OUT]** 서보안전 보드(BD642)
- 메인제어모듈(H6COM-T) ↔ **[IN]** 서보안전 보드(BD642) **[OUT]** ↔ **[OUT]** 사용자DIO 보드(BD681)
- 메인제어모듈(H6COM-T) ↔ **[IN]** 사용자DIO 보드(BD681) **[OUT]** ↔ **[IN]** 서보안전 보드(BD642)

<br>

![](../_assets/5-Communication/BD642_EtherCAT_Connector.png)<br>
그림 5.3.1 BD642 EtherCAT 통신 커넥터

<br>

![](../_assets/5-Communication/BD681_EtherCAT_Connector.png)<br>
그림 5.3.1 BD681 EtherCAT 통신 커넥터

<br>

올바른 통신 연결을 구성하였을 경우, 제어기 전원을 켜면 ENI파일을 자동으로 선택하여 연결을 시도합니다.<br>

만약 ENI파일 내부 설정이 맞지 않는 경우, 정상적으로 통신은 연결 되었는데 기능이 정상동작 하지 않을 수 있습니다. 그럴 경우 제어기 메인제어모듈(H6COM-T) 버전업데이트를 진행하거나, 당사에 문의하십시오.<br>

사용자가 수동으로 ENI파일 선택을 변경하려면 아래의 TP 메뉴에서 설정할 수 있습니다.
변경 후에는 제어기를 재부팅해야 정상적으로 적용됩니다.

**- 메뉴 위치 : [시스템]-[5:초기화]-[10:제어기 설정]**

# Appendices
  


# Rules on Occupational Safety and Health Standards and Safety Inspection Notification

This industrial robot shall be installed in consideration of the inspection requirements specified in the Rules on Occupational Safety and Health Standards and the Safety Inspection Notification, where applicable.

"[Rules on Occupational Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/korean/README)"
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/korean/README)"
