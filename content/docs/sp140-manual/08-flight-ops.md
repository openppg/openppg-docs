---
title: "Flight Operations"
description: "Normal flight procedures for the SP140 v2.5"
summary: "Takeoff, climb, cruise, landing, and post-flight shutdown procedures"
date: 2026-01-13T00:00:00+00:00
lastmod: 2026-01-13T00:00:00+00:00
draft: false
weight: 180
toc: true
seo:
  title: "SP140 v2.5 Flight Operations"
  description: "Complete guide to safe flight operations including takeoff, flight, and landing procedures"
  canonical: ""
  noindex: false
---

## Normal Flight Profile

The SP140 electric paramotor operates on the same principle as any other gas paramotor, spinning the propeller to produce thrust, so it can be flown similarly to most other paramotors.

### Takeoff

While no warm-up is needed, it's still a good idea to spin up the propeller and ensure there are no impediments to a smooth takeoff. Pilots tend to be focused on the takeoff once the wing is overhead, so it's best to confirm everything will operate as expected.

**Pre-Takeoff:**
1. Complete all [Pre-Flight Checks](../07-pre-flight)
2. Arm the system
3. Test throttle response with brief pulses
4. Check hand controller display for any alerts
5. Verify wing is properly laid out

**Takeoff Sequence:**
1. Establish wing overhead
2. Apply smooth, progressive throttle
3. Build speed gradually
4. Maintain directional control
5. Transition to flight smoothly

{{< callout context="tip" title="Pro Tip" icon="outline/rocket" >}}
The electric motor provides instant power - no need for warm-up or engine tuning.
{{< /callout >}}

### Climb-Out

During climb-out and under full power, always ensure there's a safe landing area at any point in case of motor or wing problems. Also, check the hand controller's screen for system alerts before they reach a critical state. It's designed to give a heads-up well in advance to avoid surprises.

**Climb Considerations:**
- Monitor battery SOC
- Check motor temperature
- Scan for system alerts
- Maintain situational awareness
- Keep emergency landing spots in mind

### In Flight

When settled into cruise flight, always be aware of your surroundings, watch out for other aircraft, and monitor any developing weather. Also, check the hand controller's screen to monitor flight systems status and remaining energy.

**Flight Monitoring:**
- **Battery SOC**: Plan landing with 15-20% reserve
- **Temperatures**: Motor, Battery, ESC should be in normal range
- **Alerts**: Address warnings before they become critical
- **Weather**: Monitor conditions continuously
- **Traffic**: Maintain see-and-avoid vigilance

**Cruise Control:**
When cruise control is engaged:
- Maintain awareness of power setting
- Monitor battery consumption
- Be ready to override if needed
- Check [First Start-Up section](../05-startup) for cruise control operation

{{< callout context="note" title="Important" icon="outline/info-circle" >}}
Your hand controller will vibrate to notify you of any warnings or alerts, along with displaying the information on the screen.
{{< /callout >}}

### Flying Philosophy

**Always fly in the manner that if a motor out occurred you would always have a safe glide to a landing spot.**

This means:
- Never fly over terrain with no outs
- Maintain sufficient altitude over obstacles
- Keep landing options within glide range
- Brief passengers on emergency procedures

### Landing

Many pilots choose to disarm the throttle on landing to prevent accidental activation when on the ground; this is a personal preference.

**Landing Sequence:**
1. Plan your approach with adequate altitude
2. Set up for final approach
3. Reduce power progressively
4. Flare as normal for your wing
5. **Optional**: Disarm throttle to prevent accidental activation
6. Execute landing

**After Touchdown:**
1. Killwing or control as appropriate
2. Disarm if not already done
3. Turn off main power switch
4. Secure equipment

## Post-Landing Shutdown

After flight, turn off the main power switch located on the battery pack. Then, unplug the main power lead from the motor. Note the battery's SOC percentage.

**Shutdown Procedure:**
1. **Disarm** the system (if not already done)
2. **Power Off**: Turn off main power switch on battery
3. **Disconnect**: Unplug main power lead from motor
4. **Check SOC**: Note battery state of charge
5. **Secure Equipment**: Prepare for transport

### Battery Management After Flight

**If landing with SOC below 10%:**
- Charge battery back to around 50% SOC before storing the system for longer than a week
- See [After-Flight Care](../09-after-flight) for detailed storage guidelines

**General Guidelines:**
- SOC > 50%: Can store as-is for short term
- SOC 20-50%: Ideal for storage
- SOC < 20%: Charge to 50% for storage
- SOC < 10%: Charge promptly to prevent cell damage

## Emergency Procedures

### Motor Failure
1. Maintain aircraft control
2. Set up for emergency landing
3. Execute normal landing flare
4. Land in prepared area

### System Alerts During Flight
1. **Warning (Yellow)**:
   - Note the alert
   - Monitor system
   - Plan to land soon
   - Address issue on ground

2. **Critical (Red)**:
   - Prepare for motor cutout
   - Set up emergency landing
   - Land as soon as safely possible

### Battery Warnings
- **SOC < 15%**: Land within 5 minutes
- **SOC < 5%**: Land immediately
- **Cell Voltage Low**: Land immediately

## Flight Planning

### Pre-Flight
- Check weather and forecasts
- Brief flight plan
- Calculate required battery capacity
- Identify landing options
- Notify others of plans

### Range Planning
- **Conservative**: Plan for 60-70% of rated flight time
- **Account for**:
  - Wind conditions
  - Altitude changes
  - Temperature effects
  - Reserve power

### Post-Flight
- Log flight time and battery usage
- Note any issues or anomalies
- Update maintenance records
- Plan next flight

## Performance Optimization

### Maximizing Flight Time
- Use cruise control for efficiency
- Fly in calm conditions when possible
- Minimize full-power climbs
- Maintain optimal wing loading
- Keep battery at moderate temperature

### Power Management
- **Takeoff**: Full power as needed
- **Climb**: 70-80% power typical
- **Cruise**: 40-60% power
- **Landing**: Variable, as needed

## Next Steps

After landing and shutdown:
- Review [After-Flight Care](../09-after-flight)
- Complete maintenance items
- Log flight in OpenPPG app
- Store equipment properly

For system alerts encountered during flight, see [Alerts & Warnings](../06-alerts) for detailed explanations.
