# Control Rods
The control rods moderate the reaction. The higher the insertion, the slower the reaction gets, allowing you to adjust the power level.

The rods start out fully inserted with the average rod position at 0%.

### Control Lever:
Allows you to manually move the rods. Its speed can be adjusted with the “Rod Control Speed” switch.

### Auto Balancer:
Rods temperature imbalance happens because the fuel rods are fueled unequally. Automatically matches the temperatures between rods with instability as a side effect. It’s recommended to keep it on “Fast” until you’ve met demand (or until you see the temperature imbalance has been fixed), after which you can turn it off. _Attention: major temperature imbalance will cause a reactor trip, so pay attention to rod temperature monitor._

### SCRAM:
Rapidly inserts all of the rods, shutting down the reactor. This does not immediately cool down the reactor so shutdown cooling is required for a full shutdown.

### Control Mode:
Switches between controlling individual rods via the blue buttons or all of them at once. Keep it on “All” unless you need to manually fix a temperature imbalance.

### Rod Level:
Changes the cell layer that is displayed on the temperature monitor. Usually left on “A” (average temperature) as it’s the only useful metric.

## Monitors
These are the main way of inferring the current status of the reactor, so they’re important to keep track of at all times.

### Average Power Range Monitor (APRM):
Shows you the power level (in %) of the reactor while it’s running. Don’t let this get outside of 5-100% unless you know what you’re doing. On low powers, for example, when starting up the reactor, you should use the IPR monitor (see below) instead, because APRM isn't capable of accurately reading very low power values.

### Reactor Period:
Shows you the APRM change rate. It’s measured in how many seconds it’ll take for the APRM to triple (to be exact, to change by 2.72 times). Infinity ("Inf" on the display) means the power is stable while negative numbers mean it’s decreasing.

### Intermediate Power Range (IPR):
Used for monitoring the power level during startup. Changing the level adjusts its sensitivity and scale (range).

### Source Range Monitor (SRM):
Measures neutron flux on extremely low power levels during startup, but it’s not all that useful. "Saturated" means the core is saturated with neutrons and the reactor has reached criticality.
