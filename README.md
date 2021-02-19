# INTRODUCTION TO ADC

Data convertors act like a mediator in between the digital and analog world. They are used to convert analog signals to digital signals. They form the critical component of all the systems. The digital signals are considered dominant over analog signals as they improve the modern circuit performance. ADC is required as most signals in the physical world are analog.

## SPECIFICATIONS: 
### 10 Bit ADC, 3.3V Analog Voltage, 1.8V Digital Voltage and 1 off-chip external voltage reference

## WHY SAR?

SAR ADC is selected as it provided with a perfect balance of speed, power and area consumption.

![WhatsApp Image 2021-02-05 at 9 41 54 AM](https://user-images.githubusercontent.com/77826778/108491401-ddcb1900-72c9-11eb-9ab0-5ffe619149d3.jpeg)

## BLOCK DIAGRAM OF ADC

![Capture3](https://user-images.githubusercontent.com/77826778/108491563-1539c580-72ca-11eb-95b6-4b71cb6aba58.PNG)


## DETAILED BLOCK DIAGRAM OF ADC

The ADC consists of five parts-
1.  Comparator
2.  SAR Logic
3.  R-2R DAC
4.  Sample and Hold

![Capture4](https://user-images.githubusercontent.com/77826778/108491680-38647500-72ca-11eb-870a-72871763f5e0.PNG)


## SAR ADC Parameters

| Parameter| Description| Min | Typ | Max | Unit | Condition |
| :---:  | :-: | :-: | :-: | :---:  | :-: | :-: |
|VDDA|Analog Supply Voltage||3.2||V|T=40C to 85C|
|VDD|Digital Supply Voltage||1.8||V|T=40C to 85C|
|VREFH|Reference Voltage High|||3.3|V|T=40C to 85C|
|VREFL|Reference Voltage Low|0|||V|T=40C to 85C|
|FCLK|Clock Frequency|0.01|1|2|MHz|T=40C to 85C|
|RES|Resolution||10||Bits|For all above typical conditions (T=27C)|
|INL|Integral Non-Linearity||||LSB|For all above typical conditions (T=27C)|
|DNL|Differential Non-Linearity||-14.9||LSB|For all above typical conditions (T=27C)|
|RIN|Analog Input Resistance||110||kohm|T=-40C - 85C|
|CL|Analog Input Capacitance||||pF|VT=-40C - 85C|
|IVREF|Current through Reference Source||1.06||mA|For all above typical conditions (T=27C)|
|T1|Start signal duration||0.5||Clock Cycles|T=-40C - 85C|
|TCONV|Conversion Time||12||Clock Cycles|T=-40C - 85C|
|T4|Tracking Time||4||us|T=-40C - 85C|
|IDDA|Analog Supply Current||2.97619||mA|T=27C, EN=1,FCLK=2MHz|
|IDDA|Analog Supply Current||||pA|T=27C, EN=0,FCLK=2MHz|
|IDDD|Digital Supply Current||2.833||mA|T=27C, EN=1,FCLK=2MHz|

## LAYOUT

* ### Layout of SAR Logic

![sarlogic](https://user-images.githubusercontent.com/79297655/108503550-939e6380-72da-11eb-9ad3-bb6b60ca8b25.PNG)

* ### Layout of Comparator

![comparator](https://user-images.githubusercontent.com/79297655/108503621-b3ce2280-72da-11eb-8537-53a94bb97bb3.PNG)

* ### Layout of complete ADC

![layout of sar](https://user-images.githubusercontent.com/79297655/108504744-63f05b00-72dc-11eb-9d29-43123b8f416f.PNG)


## TRANSFER FUNCTION

![transfer](https://user-images.githubusercontent.com/79297655/108503697-d3654b00-72da-11eb-837f-946879784247.PNG)

