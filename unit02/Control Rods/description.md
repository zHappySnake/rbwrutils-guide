# Control Rods
The control rods moderate the reaction. The higher the insertion, the less active the reaction becomes, allowing you to adjust the power level.

The rods start out fully inserted with the average rod position at 0%.

### Control Lever:
Allows you to manually move the rods. It’s speed can be adjusted with the “Rod Control Speed” switch.

### Auto Balancer:
Automatically matches the temperatures between rods with instability as a side effect. It’s recommended to keep it on “Fast” until you’ve met demand, after which you can turn it off.

### Scram:
Rapidly inserts the rods and shuts down the reactor. This does not immediately cool down the reactor so shutdown cooling is required for a full shutdown.

### Control Mode:
Switches between controlling individual rods via the blue buttons or all of them at once. Keep it on “All” unless you need to manually fix a temperature imbalance.

### Rod Level:
Changes the cell layer that is shown on the temperature monitor. Usually left on “A” (average) as it’s the only useful metric.

## Monitors
These are the main way of inferring the current status of the reactor, so they’re important to keep track of at all times.

### Average Power Range Monitor (APRM):
Shows you the power level of the reactor while it’s running. Don’t let this get outside of 5-100% unless you know what you’re doing.

### Reactor Period:
Shows you the change in APRM. It’s measured in how many seconds it’ll take for the APRM to triple. Infinity means it’s stable while negative numbers mean it’s decreasing.

### Intermediate Power Range (IPR):
Used for monitoring the power level during startup. Changing the level adjusts it’s sensitivity.

### Source Range Monitor (SRM):
Measures extremely low power levels during startup, but it’s not all that useful.
