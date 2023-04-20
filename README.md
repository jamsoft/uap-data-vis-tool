# UAP Data Visualisation Tool `v1.4.0`

## Introduction

What is this?

A desktop application to import, standardise and visualise various UAP data sources. Importing both the UPDB and Hatch data sources will put `318,477` individual sighting events into a searchable database and visualisation tool.

# Getting started

## Download for Windows

[Windows x64](https://github.com/jamsoft/uap-data-vis-tool/raw/main/downloads/JamSoft.UapTool.exe)
> When launching the tool, you may get a Windows warning about an "unsafe" program saying "Windows protected your PC" this is just due to the tool not currently being signed by my developer certificate, just click "More Info", then the "Run anyway" button.
## Download for Linux

[Linux x64](https://github.com/jamsoft/uap-data-vis-tool/raw/main/downloads/JamSoft.UapTool)
> Once downloaded you may have to set it as executable in order to launch, right-click -> properties -> permissions -> Execute
## Initially Loading Data

The tool isn't supplied with the Hatch JSON data file or the UPDB data file but it will automatically download the latest versions for you and import the data.

1. Launch the executable by double-clicking the .exe file you just downloaded.
2. Click one of the `Load xxxx` buttons
3. The tool will the run the various processes to load the data. 
   1. if the file is not already there on disk, it will download it for you.
4. Explore the data

The Larry Hatch JSON data file is [here](https://github.com/richgel999/ufo_data/blob/main/bin/hatch_udb.json) if you want to download it manually.

The UPDB data file is [here](https://huggingface.co/datasets/findjammer/updb/tree/main) if you want to download it manually.

> If you wish to reset the import process or start from scratch, simply delete the database file (uapdb.ufo) and restart an import process.

# Data Selections

### Dates
The tool at the moment shows some of the basic statistics and various time related data visualisations. The data can be selected based on date ranges using the `From` and `To` controls. Some predefined date ranges are also selectable in the drop down menu.

If for any country or description search string you specify results in empty charts it's possible that any matching cases are outside the date range you have currently selected. To auto expand the date range simply click the `All Dates` button to ensure the entire database is included by date.

> **WARNING**: Selections spanning the entire dataset if you have imported the UPDB can take some time to process as it calculates statistics.

### Description
You can use the Description text box to specify a word to filter the data on. The filter is applied to the contents of the description field. You can also use the toggle switch to invert the selection and exclude sighting events containing the specified term.

### Country

You can also filter the data based on individual countries using the country dropdown.

Once you have your filter set-up, click the `Apply Filter` button to filter the database and calculate the statistics.

# Basic Statistics Series
The basic statistics view shows pie charts of each of the main characteristics of the selected data, such as Country, Time of Day etc.

![Pies](/img/pies.png "Pies")

# Time Series

The Time series breaks down the sighting by time of day. The series can also be configured in terms of the time slice size. Normal will plot in 15 minute slices, 30 minutes and 60 minutes (the default) groups cases into these time boxes to flatten out the trend line.

![Time Series](/img/time.png "Time Series")

# Time vs Duration
A breakdown of the average event duration plotted against the time of day.
![Duration Series](/img/time-duration.png "Duration Series")

# Keywords
These charts aggregate together certain collections of terms often quoted in relation to anomalous sightings. For instance, the `Trained Observers` series would include terms like `pilot`, `police`, `astronomer` or `air traffic controller` among others. Another example would be the shape series `Cylinder`, this aggregates together terms like `cigar`, `torpedo` and `tube`.

![Keywords Series](/img/keywords.png "Keywords Series")

# Raw Data View

The raw data view allows you to view each complete event entry for the given set of active filters. The data can be sorted in ascending and descending order by clicking on the column headers. You can also sort on multiple columns by holding `SHIFT` and clicking on the column headers.

![Raw Data View](/img/raw-data.png "Raw Data View")

### Google Maps

Individual sightings can be viewed in Google Maps by double clicking on a data row in the `Raw Data` view.

### Sighting Links

Individual sighting links can be viewed in your default browser by holding `CTRL` and double clicking on links column in the `Raw Data` view.

# Supported Platforms

Currently the tool only supports 64-bit Windows & Linux, we have MacOS version incoming once I've had enough time to test the build.

# Issues & Feature Requests

If you encounter any issues using the tool or have any feature requests please do open an issue here on this repository.

Happy UAP'ing!

# Roadmap
    
MORE DATA PLEASE!! Let us know if you want any data source added to the tool in the future.

More default charts and different pivots for data comparisons, ideas most welcome.

# Credits

The data has been painstakingly formatted, sourced and processed by Rich Geldreich as part of his UFO Data project which you can find [here](https://github.com/richgel999/ufo_data). Thanks Rich!

[UPDB data set](https://updb.app/)

![UFO](/img/ufo.png "Ufo Logo")