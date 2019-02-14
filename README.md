# SpO2 Pi Python

This project is intended to run on a Raspberry Pi in order to read data from a
MAX30105 light sensor and calculate pulse oximetry and heart rate (and maybe more).

## Usage

Run `python2 main.py filename` from the RPi.
This will save raw Red, IR light data to `filename` file.

## Todo

- Need some method to convert the raw light data to SpO2 and HR. Right now I made
defined a function called `calculate_spo2_and_hr` in converter.py that gets
called when you run main.py, but it just returns dummy data.

- Need to implement the ability to send the SpO2 and HR measurements to the web
app. Currently, I have a placeholder in main.py called `send_spo2_and_hr(spo2, hr)`
for this purpose.
