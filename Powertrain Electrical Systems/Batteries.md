# Hacky Racers Build Guide

This project is under construction, and not yet complete.
Guidance for anyone wishing to build a Hacky Racer!
http://www.hackyracers.co.uk

# Batteries

Hacky Racers are electric vehicles, therefore they need some sort of power supply. In a traditional combustion engined go kart this would be petrol stored in a tank. While we could race with various extension leads, or scalextrix style power lines batteries are a much better option.

More detailed information about batteries can be found in the rules.

There are a few different types of batteries that are applicable and allowed for use in Hacky Racers. These are:

	* SLA: Sealed Lead acid
	* AGM: Abosrbed Glass Mat Lead acid
	* Ni-Cd: Nickel-Cadmium
	* Ni-Mh: Nickel-Metal Hydride
	* LiFePO4: Lithium Ion Phosphate
	* LiPO/Li-Ion: Lithium Polymer/Ion

Most racers choose to use SLA or AGM for lower power/slower vehicles. These batteries are fundamentally simple, however are heavy and less power dense than Lithium Options. They require a very basic charger and are very safe, unless you drop one on your toes.

Lithium can often also supply more current, and can do so very quickly, leading to faster acceleration in some cases.

Lithium batteries are generally incredibly power dense, and beginning to become less expensive thanks to readily available RC hobby batteries.
Lithium Ion Phosphate batteries are generally very safe and are much better than lead-acid style batteries.

Lithium Polymer/Ion Batteries are currently the best battery technology available in terms of power density, output and form factor. These do however require more care to use safely. If you are not sure what you are doing with Lithium Polymer/Ion, don't use them. Do your own research, and we can help you learn. Lithium Batteries can be extremely dangerous if mishandled.

Lithium Polymer batteries must be "balanced" between all cells. This means they require a more complex charger however these can be purchased relatively inexpensively now. The racer should supply a sufficiently fire resistant enclosure for use while charging LiPo/LiIon batteries. This could be a dedicated lipo charging bag, or a metal container such as a ammo can with a suitable vent.

These batteries are sensitive to the amount of charge stored. For long periods with no use, the batteries should be stored at a storage charge. Typically this is about 3.8V per cell, but check your own battery datasheet as this can vary. Each battery has a maximum and minimum voltage. Do not ever overcharge, or overdischarge a lithium ion or polymer battery. You should have measures in place to prevent over discharge, whether this is an alarm or a physical cut off(Some motor drivers include this natively). Typical minimum and maximum values are 3.4V and 4.2V per cell respectively, but once again check your batteries datasheet.

# Battery ratings

All batteries have ratings that specify their characteristics.

* Voltage: This can be stated directly, such as "12V", or is commonly given as a "series" value for lithium batteries. If a 4.2V max lithium cell is used in a 10S pack, the maximum pack voltage is 42V. (10 4.2V cells in series, 4.2 + 4.2 + 4.2 ...)

* Amps: The number of amperes a battery can push out is typically listed in a few ways. Continuous discharge current is as it sounds, the maximum discharge current that the battery can supply constantly. A peak  discharge current is often listed too, for a specific amount of time. For lead acid this is usually stated directly in the datasheet, for lithium batteries a shorthand is used. "C" rating. A lithium battery may be rated with a 10C constant rating, or 20C burst for 15 seconds for example. The value of C relates to the amp-hour capacity of the battery. A 5ah Lipo with 10C continuous rating can output 50A continuously, and with a 20C burst, 100A for the specified time.

	These batteries will also have charge currents listed, and it is important this is not exceeded. For lithium batteries this will also be listed as a "C" rating commonly.

* Amp-hours: The capacity of batteries is usually listed in amp hours, and this simply can be thought of as how many amps can be output for 1 hour. Ie a 5ah battery can discharge 5 amps for an hour before running out of energy. As hacky races are often 10-20 minutes, battery capacity is usually optimised for this. The same 5ah battery, that can discharge 5 amps for an hour, could discharge 15 amps for 20 minutes, if it has sufficient C rating.