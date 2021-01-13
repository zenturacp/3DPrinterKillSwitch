# Basic features

Here is a brief description of the main features in first version of the kit

## Sensors

There will be 4 sensors input total
- Hotend sensor
- Heated bed sensor
- Champer / AUX (Can be used for 2 hotends as well)
- Smoke detector

## Control / Display / Navigation

It will be a very simple interface with only 2 buttons

- Menu button
  - Switch between menus
- Set button
  - Cycle through options

### Display pages

When you press the menu button it will cycle through pages - if you press nothing in 20 seconds it will go back to page 0

1. Dashboard
   * Shows current readings plus max value to initiate Kill
2. Set Hotend Max Temp
   * Pressing the set button skips through options from 100 degrees to 300 degrees in 10 increments and a disabled state
3. Set Bed Max Temp
   * Pressing the set button skips through options from 50 degrees to 200 degrees in 10 increments and a disabled state
4. Set Chamber Max Temp
   * Pressing the set button skips through options from 20 degrees to 60 degrees in 1 increments and a disabled state
5. Set Smoke detector threshold (Optional - maybe this page vil just enable / disable)
6. Timer
   * Setting how long after threshold is reached the kill switch will activated in increments of 10,20,30,40,50,1 min, 2 min, 3 min, 4 min, 5 min, 10 min

### Save settings

When chaning settings and you leave a page its stored in EEPROM on the MCU

### Reset Settings / Factory Reset

Press and hold both buttons on startup will clear all values

