---
title: "8. After-Flight Care"
description: "Transport, battery storage, scheduled maintenance, charging, and firmware updates"
weight: 10
slug: "after-flight"
---

## 8.1 Transport

When transporting the motor and frame strap it securely in place from large movements. If traveling on bumpy roads, please store the battery upright or lay it flat on its side in its foam case. **Do not transport the battery upside down.**

## 8.2 Short- & Long-Term Storage

For long-term storage, store the entire paramotor in a cool, dry place. This helps prevent degradation of the fabrics in the harness and battery pack due to environmental factors. For optimal long-term storage (over one week), store the battery pack **at 10-25°C, with a state of charge (SOC) between 30-50%, and away from high humidity.**

Even with the main power switch off, the pack self-discharges about **1% per day** because the BMS stays active for monitoring and Bluetooth. For storage longer than a few weeks, use the **"Close BMS"** setting in the battery's Bluetooth app to minimize standby drain.

Operating in very cold environments (sub-0°C temperatures) is not a problem for the SP140. However, avoid storing the battery pack outside in those temperatures, as the battery pack's maximum energy output will be reduced if cooled to those temperatures. Normal cold weather flying, even at -20°C, is fine, as the internal heating of the cells during use will protect the battery pack. The performance decrease only occurs during long-term storage in cold environments.

## 8.3 Scheduled Maintenance

There's little maintenance needed, as there are no motor rebuilds, oil changes, carburetor tuning, and essentially no moving parts, unlike a gasoline motor. There are a few things to keep an eye on below:

| Interval                                    | Task                                                                                                                                                                                                                                                                                                                                           |
| :------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Every flight**                            | Inspect bolts, straps, and propeller for any marks or chips                                                                                                                                                                                                                                                                                    |
| **Every 3 weeks**                           | Check the battery pack's cell voltages on the hand controller screen (see [5.3 Telemetry Link data](../first-start/)) or with the [OpenPPG app](https://openppg.com/beta/). If any cell has dropped below 3.3 V, charge the pack back into the 30-50% storage range described in [8.2](#82-short---long-term-storage), roughly 3.8 V per cell. |
| **Every ~20 flights while the unit is new** | Re-check the swing-arm motor-mount lock nuts. These back off slightly when new and then settle — this is expected and not a safety concern. Threadlocker (Loctite orange or red) or a double-nut setup with a slightly longer bolt will stop it. Stop and inspect if you ever see large or growing play.                                       |

## 8.4 Charging

1. The included charger plugs into any standard household wall outlet — no special or dedicated circuit is needed. It draws about 10 A at ~100 V (roughly 1,000 W).
2. **Chargers are region-specific (110 V or 220 V) — they are not dual-voltage.** Plugging a 110 V charger into a 220 V outlet will damage it immediately. Always use the charger that matches your region's mains voltage.
3. A full recharge takes about **2-3 hours** for the 2.6 kWh battery and **4-5 hours** for the 4.8 kWh battery. The stock charger is fixed-output — charging speed is not adjustable.
4. For field charging away from mains power, use a **clean sine wave inverter generator** with at least ~1,500 W of capacity. Avoid cheap non-inverter generators — rough power can damage the charger.
5. If you land with the SOC below 10%, charge the battery back to around 50% before storing the system for longer than a week (see [7.2 Post-Landing Shutdown](../flight-operations/)).

## 8.5 Firmware Updates

The hand controller and the motor controller (ESC) each run their own firmware. Keeping them current fixes bugs and adds features, and the two need to be on compatible versions — a mismatch can hide telemetry such as battery voltage even though the motor still runs normally.

1. Updates are done through the online configurator at [config.openppg.com](https://config.openppg.com), connected over a USB-C **data** cable (charge-only cables will not work).
2. Use a Chromium-based browser — **Chrome or Edge. Safari is not supported.**
3. From firmware v8.0 onward the hand controller also supports over-the-air updates through the [OpenPPG app](https://openppg.com/beta/), with no cable required.
4. Your current firmware version is shown on the hand controller screen at startup.

The configurator site has the full step-by-step instructions, release notes, and the settings reference. If an update ever leaves the controller unresponsive, contact [info@openppg.com](mailto:info@openppg.com) — it is usually recoverable.
