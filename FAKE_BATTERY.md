Some WIP work on cheating the power management chip so the unit will boot without a chip.

## 

## The Capacitor Method

Put a large capacitor between +BAT and GND. This method requires an actual battery connected to the capacitor in parallel for several seconds when the unit is booting; after it has been working steadily you can disconnect the battery. 

## The Voltage Emulation Method

This method emulates a full battery by providing a ~4V voltage to the PMIC. Since there is no obvious way to get an +5V from the PCB surface, +5V can be acquired by directly inputing 5V to the USB host (USB-A) port. (See: [English](https://github.com/Jamesits/sound-blaster-e5-battery/issues/1) [Chinese](https://zhuanlan.zhihu.com/p/90036682)). 

![](assets/ams1117_4v.png)

Credit: this method came from [rgwan](https://github.com/rgwan). 

~~If you found any way to access +5V on the E5 PCB without heavily modifying it, please contact us.~~

