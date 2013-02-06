touch_event_record
==================

A simple script that accepts input via stdin (piped from adb shell getevent)
and does the appropriate conversions, printing out the corresponding
adb shell sendevent commands to replay your touch actions.

After completing your input, you can copy the output into a shell script
and add sleep statements as needed to introduce delays between touch
events in playback.  (A later version may automatically create these, but
for now you're on your own ;))

** NOTE: Requires the Android Debug Bridge (adb) utility to be installed.

Usage: adb shell getevent | touch_event_record.py


