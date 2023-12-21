# Electrical Panel

The electrical panel is where the player can control the power distribution for the unit and its connection to the national grid. The E.P. consists of the following switches, from top-bottom, left-right;

## Breakers

### Breaker 52G1
This is the switch that synchronises the turbine to the grid, allowing for the site to provide power and start earning points.

### Breaker 52G2 
The only "switch" that can trip. It supplies the facility power from the startup transformer. It will trip at roughly 30MW (Based off of some rough math). It can be enabled and disabled at any time, but keep in mind, this may cause issues. This powers: Bus A, Safety Bus, DC Bus.

### Breaker 52BA1
This is the breaker that powers Bus A when the Startup Transformer is not connected, instead supplying it with power from the turbine. Breaker 51BA1 can only be enabled when the Turbine is capable of islanding.

### Breaker 52BB1
This breaker powers Bus B, and can only be enabled when the turbine is capable of islanding.

### Breaker 52BA2
This breaker powers the safety bus, and can be enabled and disabled at any time. It is recommended to always keep this enabled, as it charges the batteries and supplies the LPCI with power (so long as the breaker itself has power, either from the Startup Transformer or the Turbine via B-B2BB1.) if everything else fails. It can be turned off, but this will also turn off the lights, which must be then powered by the Emergency bus via Switch 59BDC1, or via the diesel generators.

### AC-DC (left)
No, this is not the band. It converts Alternating Current (AC) into Direct Current (DC). It is likely used to help charge the battery.

### AC-DC (right)
This supplies the DC bus with power from the Startup Transformer, from the turbine via Bus A, or from the Diesel Generators. This might as well be disabled if B-B2BA2 is disabled, since it does absolutely nothing without it enabled, unless the Diesel Generators are enabled.

### Breaker 52DG1
This connects the Diesel Generator to the Safety Bus once it has reached the required RPM (1800), allowing for it to be powered during an Offsite Power loss.

## Switches

### Switch 59BDC1
This connects the emergency bus to the DC bus, allowing for the lights to be on and the Diesel Generator to be kickstarted during an offsite, or when the Safety bus is disabled.

### Switch 59DG1
This connects the Diesel generator to the DC bus, allowing the D.G to be started up via:

### DG. Startup Spark
Spins up and ignites the diesel, starting up the generator. This will cause the RPM of it to slowly tick up, until it reaches 1800 RPM.

## Busses

So, Bus A?! Safety Bus?! What’s that?? Well, Wikipedia says that “for sufficiently large systems, these points represent physical busbars, so the diagram nodes are frequently called buses. A bus corresponds to a location where the power is either injected into the system (e.g., a generator) or consumed (an electrical load)" So, what bus powers what?

### Bus A
This bus powers the CST pumps, Hotwell Drain and Makeup, Pumps #1 of the Feedwaters, Condenser Circulation, the Condensate pump, and both pumps for the recirculation.

### Bus B
This bus powers the remaining pumps.

### Safety Bus
This powers most key systems for shutdown. It powers the CARs (Condenser Air Removal), the LPCI pump, and both Shutdown Cooling Pumps.

### DC bus
This powers the ventilation (has no ingame use atm) and the main lights.

### Emergency Bus
This powers the Low Power (LP) lights, and the actual controls for the panels. If the battery dies (hits 0%), these systems would be unable to work, giving 0 lighting and no control over operations, and as such, the server you're playing on will be shut down.
