Some WIP work on cheating the power management chip so the unit will boot without a chip.

## 

## The Capacitor Method

Put a large capacitor between +BAT and GND. This method requires an actual battery connected to the capacitor in parallel for several seconds when the unit is booting; after it has been working steadily you can disconnect the battery. 

## The Voltage Emulation Method

This method emulates a full battery by providing a ~4V voltage to the PMIC. 
![](assets/ams1117_4v.png)

Credit: circuit is from [rgwan](https://github.com/rgwan).

To get +5V on the board:
![](https://user-images.githubusercontent.com/443972/95324804-f43b7f80-08a8-11eb-8e4c-c37299dc9ac0.jpg)

Credit: [bamx23](https://github.com/bamx23)([#5](https://github.com/Jamesits/sound-blaster-e5-battery/issues/5))

+5V can also be acquired by directly inputing 5V to the USB host (USB-A) port. (Credit: from [pbjacob](https://github.com/pbjacob). His implementation details: [English](https://github.com/Jamesits/sound-blaster-e5-battery/issues/1) [Chinese](https://zhuanlan.zhihu.com/p/90036682)). Assuming a PMIC can accept a 5V voltage from battery, the LDO might not be necessary.
