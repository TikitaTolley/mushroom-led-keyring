# Mushroom LED Keyring

> A keyring of LEDs arranged in a mushroom cap, switched on and off by a slide switch.

[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=flat&logo=youtube&logoColor=white)][yt]
[![TikTok](https://img.shields.io/badge/TikTok-000000?style=flat&logo=tiktok&logoColor=white)][tt]
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white)][ig]
[![Tinkercad](https://img.shields.io/badge/Tinkercad-simulate-1477D1?style=flat)][tinkercad]

![Front of keyring](media/keyring-front.jpg)
![Keyring lit up](media/keyring-front-lit.jpg)
![Back of keyring](media/keyring-back.jpg)

## What it does

Green and yellow LEDs laid out as a mushroom cap, running off coin cells with a slide switch for on/off. Every LED has its own series resistor and sits in parallel across the rails, so they all light together and one failing doesn't take the rest out.

## Simulated

| Sim | Link | Notes |
| --- | --- | --- |
| Tinkercad | [Open][tinkercad] | Breadboard version of the circuit |

## Bill of materials

| Qty | Component | Part | Unit cost | Notes |
| --- | --- | --- | --- | --- |
| 2 | Coin cell | CR2032 3 V | £0.60 | Wired in series for 6 V |
| 2 | Battery holder | CR2032 holder | £0.40 | Or one 2-cell holder |
| 1 | Slide switch | SPDT | TBD | On/off, in the positive line |
| 6 | LED | 5 mm | from kit | 4 red, 2 amber in the sim |
| 6 | Resistor | 1 kΩ | from kit | One per LED |
| 1 | Mini solderable breadboard | | £1.50 | |
| 1 | Keyring hardware | Split ring | £0.30 | |

**Total: £3.80** for the parts bought, plus the slide switch.

## Wiring

Two CR2032 cells in series give 6 V across the breadboard rails. The slide switch sits in the positive line, so it cuts power to everything. Each LED runs anode to the positive rail through its own resistor, cathode straight to ground, with all six branches in parallel.

| From | To | Notes |
| --- | --- | --- |
| Cell 1 | Cell 2 | In series, 6 V total |
| Battery + | Slide switch | Switch breaks the positive line |
| Slide switch | + rail | |
| Battery - | - rail | |
| LED anode (×6) | + rail via resistor | One resistor per LED |
| LED cathode (×6) | - rail | |

## Notes

Even though it doesn't look like a typical mushroom, there turns out to be a green cap and yellow stem mushroom out there!
It's called the Chicken Lips (Leotia viscosa) mushroom. [See one][chicken-lips].

## Licence

MIT, see [LICENSE](LICENSE).

---

All projects at [github.com/TikitaTolley][gh].

[yt]: https://youtube.com/@tikitatech
[tt]: https://tiktok.com/@tikitatech
[ig]: https://instagram.com/tikitatech
[gh]: https://github.com/TikitaTolley

[tinkercad]: https://www.tinkercad.com/things/bni5gjmEZWk-mushroom-leds
[chicken-lips]: https://commons.wikimedia.org/wiki/File:Leotia_viscosa_539279562.jpg
