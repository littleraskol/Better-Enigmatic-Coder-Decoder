This is a small combat tweak that hopefully will make the Enigmatic Encoder and Decoder more worthwhile when used with my other mod that improves afterburners. It makes the Encoder's evasion much better and makes the Decoder all about tracking (anti-evasion) and much better at it.

---

I need to explain the function in a bit more math depth because the in-game tooltip might be deceptive. We'll use the Enigmatic Encoder as our example, but the math is the same for the Decoder. The way it's presented, it seems like it will add 30 to the evasion rate percentage, but that's not what it really does as it uses "ship_evasion_mult" (a multiplier) rather than "ship_evasion_add" (an added value). What's meant by a "multiplier" here is that it multiplies the evasion rate by a certain percentage. For the Enigmatic Encoder this is 130%. That's what the displayed +30% actually means. In other words, it will multiply whatever evasion rate a ship has by 1.3.

Example: Base corvettes have an evasion of 60%. The Enigmatic Encoder increases this to 60% * 1.3 = 78%. This is applied to evasion after other added values. In this example, if our corvette has ion thrusters ("+3 chance to evade"), giving it the Enigmatic Encoder will increase its evasion to (60% + 3%) * 1.3 = 81.9%.

I would welcome feedback about how this affects combat in the game. I don't want it to be OP and don't really have enough testing to tell whether this makes these components "too good." Mostly I just wanted to make these components competitive when using my other mod that improves afterburners.

Compatibility note: This mod unavoidably replaces component_templates/00_guardian_utilities.txt and will likely conflict with any other mod changing how components (but not weapons) gained from defeating Guardians work.