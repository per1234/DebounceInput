# ButtonDebounce
This is a library for the Arduino IDE for debouncing digital inputs (buttons, switches).

Two classes are provided, DebounceFilter and DebouncedButton.

For more information, see `ButtonDebounce.h`.

**DebounceFilter**

An implementation of cactusjack's [Elegant debouncing solution with software Schmitt trigger emulation](http://forum.arduino.cc/index.php?topic=125297), with a few tweaks.

**DebouncedButton**

A class which is constructed on a digital input pin, and which uses a DebounceFilter to sense the state of the pin. The pin is sampled no more than every 4ms to provide consistent behaviour. Methods are provided to query the state of the pin and to sense button down and button up events.
 