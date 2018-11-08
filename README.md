# HealthKit_data_convert
Convert a HealthKit XML file – containing health and fitness data from iOS (iPhone) and watchOS (Apple Watch) devices – to a CSV file. Plot the data with [nabelekt/HealthKit_data_plot](https://github.com/nabelekt/HealthKit_data_plot)

While there are other scripts, websites, and apps (http://quantifiedself.com/qs-access-app/) to accomplish the same task, I found each one that I tried lacking in some way.

This project makes use of Python version 3. The version of Python installed by default in macOS, as of macOS 10.14 (Mojave), is Python 2.7.10. Instructions for installing Python 3 on macOS can be found at https://docs.python-guide.org/starting/install3/osx/. Python installers for Windows can be found at https://www.python.org/downloads/windows/.

### Usage

The first step is to obtain your HealthKit data from your iPhone. To do this:
1. Launch the Health app.

2. Tap the icon in the top right corner:

      ![alt text](https://imgur.com/dSqC8sv.png)

3. Tap "Export Health Data":

      ![alt text](https://imgur.com/M6Xg5UA.png)

Then, with Python 3 or later installed, at the command line do:

`python HealthKit_data_convert.py [input_file] [output_file]`

For example:

`python HealthKit_data_convert.py ../Health_Data/example_input1.xml ../Health_Data/output.csv`
