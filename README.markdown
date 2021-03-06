Alpine Data Labs Demos
======================

The following workflows attempt to explain how Alpine works through concrete examples.  They are based on relatively small public datasets.  The analytic flow and the data have been bundled together for convenience however there may be newer versions of the datasets available on the web.

Installation
------------


__Importing Workflows__

* Download the zip from github or git clone the directory of interest
* Under Workflows tab click on _Import_ button
* Select the directory of the workflow and pick the .afm file (repeat as necessary)
* Check the workflow you want to import and click on _Import_ or _Import and Open_

__Importing Data__

* Create a data source pointing to your [Hadoop cluster] (https://alpine.atlassian.net/wiki/display/DOC/Hadoop+Connection+Prerequisites "Hadoop cluster configuration")
* Browse to an HDFS location where you would like to copy the data files
* Under the data tab click on the _Import_ icon
* Select the data file using your browser's file navigation screen (each demo has a data subdirectory that houses the necessary files)
* Modify the properties of the dataset operator within each workflow to point the "Hadoop File Name" to the correct location

Demos
-----

[__Airline On-Time Statistics__] (/alpinedatalabs/demos/tree/master/airline_ontime_stats)

Predict flight arrival delays based on seasonality, departure delays and geography.

_Data:_ 2008 available in current repo, 1987-2008 available from [ASA] (http://stat-computing.org/dataexpo/2009/the-data.html) 

_Size:_ 7M rows for 2008, 120M for full data set, runs in ~1 hour

[__Census results by state__] (/alpinedatalabs/demos/tree/master/us_census)

Simple summary statistics, charts, correlations, and a linear regression on home ownership by demographics.

_Size:_ dozens of rows, runs in ~1 minute


[__Election 92__] (/alpinedatalabs/demos/tree/master/election92)

Election results by county.
Various charts and correlations for demographic factors and election results, regression on turnout by demographics, decision tree on outcome by demographics.

_Size:_ thousands of rows, runs in ~1 minute

[__FAA Service Difficulty Reports__] (/alpinedatalabs/demos/tree/master/faa)

Predict unscheduled landings based on flight stage (takeoff, approach, landing, cruising, etc), region and aircraft manufacturer.  
This workflow is based on Venky Rao's [post] (http://themainstreamseer.blogspot.com/2013/01/data-mining-and-airline-safety.html).

 __Data:__ 2012 included; full data available from [FAA] (http://av-info.faa.gov/dd_sublevel.asp?Folder=\\SDRS)
 
_Size:_ ~1 million observations, runs in ~1 minute


[__Presidential Donations__] (/alpinedatalabs/demos/tree/master/us_presidential_donations)

Donations by individual.
Comparison of the distribution of contributions at various donation levels

_Size:_ millions of rows, runs in ~5 minutes


[__US Census__] (/alpinedatalabs/demos/tree/master/us_census_full)

1% sample of census data. Frequency chart and correlations, decision tree on marital status by demographics, regression on income by demographics, clusters based on demographics.

_Size:_ millions of rows, runs in ~10 minutes

[__Forest Cover__] (/alpinedatalabs/demos/tree/master/forest_cover)

Ecological data for US forests (classic test dataset).
Box plots on elevation, clustering on environmental factors, regression and decision tree to predict type of forest based on environmental factors.

_Size:_ half a million rows, runs in ~30 minutes


 
