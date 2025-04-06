# RCWL-0516 Microwave Motion Sensor

This is the RCWL-0516, a mini-radar motion sensor module that features the RCWL-9196 chip. The modules function is based on doppler radar and has a range of about 5 to 8m. They put out very low levels of microwaves at 3.2GHz.

## Specification
* Operating voltage: 4 to 28V dc
* Operating current: 2.8mA typical, 3mA max
* Detection range: 5 to 8m
* Output voltage (trigger active): 3.2 to 3.4V
* Output current: 100mA max
* Operating frequency: ~3.2GHz
* Pin 12 on U1, (is the output of the 2nd OpAmp) can be used to understand a motion dynamics

The PCB has an onboard 3.3V voltage regulator that can supply up to 100mA if required. I don't plan to use this capability but it is useful when testing, to power local visual or audible indicators.

## Tests and ideas

If wind can trigger Pin12 is it possible to use RCWL-0516 for understanding the speed of the wind?

## Literature

1. [RCWL-0516 Microwave Motion Sensor Review](https://www.dreamgreenhouse.com/reviews/sensors/RCWL0516.php) - with ideas how to make a case and a bit about how to stop the signal propagation. Useful.
2. [RCWL-0516 information](https://github.com/jdesbonnet/RCWL-0516) - contains description of pins (like using photo-resistor to prevent alarm on a daylight)
3. [excellent video by Andreas Spiess on YouTube](https://www.youtube.com/watch?v=9WiJJgIi3W0)
