# Roboguard

The Roboguard device consists of 2x PIR motion detection sensors located inside a weatherproof plastic enclosure.

The sensors have a 110 degree throw which covers an area of up to 20 to 25 metres.

It runs on 8x 1.5v D cell batteries and is completely wireless sending data over the 433.92 Mhz range (173mm antenna).

While running on batteries, it can last up to 3 years depending on the battery quality.

There are different sensitivity settings on the device.

All in all I have been using modals manufactured in 2015 on a farm with extremely positive results.

My only issue is the high price for one unit.

# Communication Layer

I was able to determine the signal typs sent from the Roboguard to the HQ device and have made a simple list below.

- Protocol
    - 433.92Mhz AM frequency
    - ASK (amplitude shift keying)
    - Manchester NRZ (non return to zero)

- Signals
    - alarm signal
    - learn/tamper share same signal
    - Heartbeat ping signal [1x every +-15min]

# Comments

My devices send pings every 15 minutes containing the heartbeat ping signal.

After 1 hour it will trigger the status light if the signal is bad or a device has not sent a ping for more than 15 minutes.

If the battery is low then a constant alarm signal is sent once the device has been triggered in this state.

While testing I was able to simulate a low battery trigger every 5 seconds from 4.5v downwards.

Remember even though it takes 12v (13v) from 8x 1.5v batteries the 50% margin is around 6v.

# Conclusion

Using the knowledge gained from my testing I was able to pair other devices using the 433.92Mhz frequency range on my farm to the Roboguard.

This was a huge win for me since I could now use the HQ as a stand alone wireless alarm system.

I now have multiple devices that are Roboguard HQ compatible.

Since Roboguard is extremely popular in South Africa I am sure others can do the same.

# links

- [Roboguard website](https://roboguard.co.za)

