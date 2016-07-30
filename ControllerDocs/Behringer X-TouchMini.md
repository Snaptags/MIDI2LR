Behringer X-Touch Mini USB DAW Controller
=========================================

http://www.music-group.com/Categories/Behringer/Computer-Audio/Desktop-Controllers/X-TOUCH-MINI/

Midi out messages recorded using MIDI-OX.
No additional software has been installed, controller using factory settings.

Encoders
--------
Endless, but do send 0-127 in factory setting. LEDs light up according to the value automatically.

| TIMESTAMP | IN | PORT | STATUS | DATA1 | DATA2 | CHAN | NOTE | EVENT |
| --------- | --:| ----:| ------:| -----:| -----:| ----:|:----:|:-----:|
| 00007CD5  |  1 |    6 |     BA |    01 |    00 |   11 |  --- | CC: Modulation |
| 00007CD5  |  1 |    6 |     BA |    01 |    7F |   11 |  --- | CC: Modulation |

DATA1: Encoder Number (01 to 08 for Layer a, 0B to 12 for layer B)
EVENT: Different for each encoder.

Layer A, starting from 01:
CC: Modulation,      CC: Breath,         Control Change, CC: Foot Controller, 
CC: Portamento Time, CC: Data Entry MSB, CC: Volume,     CC: Balance

Layer B, starting from 0B:
CC: Expression,      Control Change,     Control Change, Control Change, 
Control Change,      Control Change,     Control Change, Control Change,

Encoder pushing
---------------

| TIMESTAMP | IN | PORT | STATUS | DATA1 | DATA2 | CHAN | NOTE | EVENT |
| 000D0CFB  |  1 |   6  |     9A |    00 |    7F |   11 | C -1 | Note On |
| 000D0D87  |  1 |   6  |     8A |    00 |    00 |   11 | C -1 | Note Off |

Buttons
-------

| TIMESTAMP | IN | PORT | STATUS | DATA1 | DATA2 | CHAN | NOTE | EVENT |
| --------- | --:| ----:| ------:| -----:| -----:| ----:|:----:|:-----:|
| 000FBE9F  |  1 |   6  |     9A |    08 |    7F |   11 | G#-1 | Note On |
| 000FBF1E  |  1 |   6  |     8A |    08 |    00 |   11 | G#-1 | Note Off |

Layer A/B: different DATA1 and different NOTE values

Fader
-----

No touch message

| TIMESTAMP | IN | PORT | STATUS | DATA1 | DATA2 | CHAN | NOTE | EVENT |
| --------- | --:| ----:| ------:| -----:| -----:| ----:|:----:|:-----:|
| 001AB1E0  |  1 |   6  |     BA |    09 |    7F |   11 |  --- | Control Change |

DATA2: value 0 to 127.

Layer A, layer B
----------------

Do not send any MIDI messages!
