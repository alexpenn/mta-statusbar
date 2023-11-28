# mtaStatusBar
rumps based status bar widget for MTA arrival times

Example:

<img width="219" alt="image" src="https://github.com/alexpenn/mta-statusbar/assets/2838351/16d3d62e-0d41-4fc6-a4ff-f729ad2362ee">

# requirements

This script relies on the following packages: rumps (Ridiculously Uncomplicated macOS Python Statusbar), Python language bindings for GTFS, protobuf3-to-dict, and dotenv to insert the API key provided by the MTA. If you use PIP, the following commands will do the trick:
```
pip install rumps
pip install --upgrade gtfs-realtime-bindings
pip install protobuf3_to_dict
pip install -U python-dotenv
```
Note that there seems to be a specific version requirement for protobuf. If running the code after the previous installations yields a TypeError, the following may fix the issue (see more info here):
```
pip install 'protobuf==3.20.1'
```
Access to the MTA live feeds requires signing up for an API key from the NYC MTA: http://datamine.mta.info/user/register

Put API key into the changeme.env file (after API_KEY=) and rename the file into an .env file within the root directory of the Python script.

# license

Uses the MIT license.
