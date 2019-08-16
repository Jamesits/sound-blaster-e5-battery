This repo provides some information on the battery issue of [Creative Sound Blaster E5](https://us.creative.com/p/sound-blaster/sound-blaster-e5).

## The Problem

* The unit can be used as a desktop DAC (always plugged in)
* Power management issues causing the battery is always in charging state as long as the microUSB port is connected
* The unit gets very hot on normal operation
* The battery is directly touching the PCB and there are a lot of sharp pieces on the PCB

So nearly every E5 would get a swollen battery every 1-2 years of daily use, but Creative only provides a limited warranty.

### Identify The Problem

Do your unit have this problem too? You can find out by the following methods:

* Is The front side of your unit (the one with NFC logo) curved? Place it on a flat surface and see if it fits.
* Is the metal bar (with SoundBlaster logo on it) not firmly attached to the plastic plate under it?

## The DIY Solution 

### Replace A Battery

See [BATTER_REPLACEMENT.md](BATTERY_REPLACEMENT.md).

### Fake A Battery (WIP)

See [FAKE_BATTERY.md](FAKE_BATTERY.md).

### Develop Your Own Solution

You know EE and wanna try it yourself? [Here are some PCB pictures](PCB.md) so you can plan before getting your hands dirty. If you found a better solution, please share with us. 

## Resources

### The Recovery Mode

(From [/u/ridicalis](https://www.reddit.com/user/ridicalis))

The [recovery mode](https://support.creative.com/kb/ShowArticle.aspx?sid=129772&c) allows a unit with its battery completely drained to charge without bootloop. It also provides some kind of DFU thing.

To enter the recovery mode:

1. Shut it down
2. Unplug the MicroUSB cable
3. Press and hold the SBX button
4. Plug in the MicroUSB cable
5. Release the SBX button if you see the middle one of the battery status LEDs start blinking. 

To exit the recovery mode:

1. Long press the power button until all LEDs are off

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />All text and media from this repository are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.