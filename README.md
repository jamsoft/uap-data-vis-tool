# UAP Data Visualisation Tool

## Getting started

Download the tool here:
https://github.com/jamsoft/uap-data-vis-tool/raw/main/downloads/JamSoft.UapTool.exe

## Loading Data

The tool isn't supplied with the JSON data file but will automatically download the latest version for you.

1. Launch the executable by double-clicking the .exe file you just downloaded (** see notes).
2. Click the Load Hatch Data button
3. The tool loads the hatch data file (hatch_udb.json) found next to the exe on disk, or it will download it for you.
4. Explore the data

The data has been painstakingly formatted, sourced and processed by Rich Geldreich as part of his UFO Data project which you can find [here](https://github.com/richgel999/ufo_data). Thanks Rich!

Currently this tool only supports the Hatch JSON data file which can be found [here](https://github.com/richgel999/ufo_data/blob/main/bin/hatch_udb.json).

** When launching the tool, you may get a Windows warning about an "unsafe" program saying "Windows protected your PC" this is just due to the tool not currently being signed by my developer certificate, just click "More Info", then the "Run anyway" button.

# Data Selection

### Dates
The tool at the moment shows some of the basic statistics and various time related data visualisations. The data can be selected based on date ranges using the `From` and `To` controls. Some predefined date ranges are also selectable in the combobx/drop down menu.

If for any country or description search string you use and the charts vanish, it's possible that the matching cases are outside the date range you have currently selected. Bash the `All Dates` button to ensure the entire database is included by dates.

### Description
You can use the Description text box to specify a word to filter the data based on the contents of the description field.

### Country

You can also filter the data based on individual countries using the country dropdown.

## Time Series

The Time series can also be specified in terms of the time slice size. Normal will plot as per the data, 30 minutes and 60 minutes (the default) groups cases into these time boxes to flatten out the trend line.

# Google Maps

Individual sightings can be viewed in Google Maps by double clicking on a data row in the Raw Data View.

# Supported Platforms

Currently the tool only supports 64-bit Windows, we have MacOS and Linux versions incoming once I've had enough time to test these builds.

# Issues & Feature Requests

If you encounter any issues using the tool or have any feature requests please do open an issue here on this repository.

# Screenshots
### Statistics
![alt text](/img/pies.png "Pies")
### Time
![alt text](/img/time.png "Time Series")
### Duration
![alt text](/img/time-duration.png "Duration Series")
### Raw Data View
![alt text](/img/raw-data.png "Raw Data View")

Happy UAP'ing!

# Roadmap

MORE DATA PLEASE!!

Looks like I've just sourced an absolute mountain of data, watch this space.

More default charts and different pivots for data comparisons, ideas most welcome.