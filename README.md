# DataDotWorld_Export_SPSS_Modeler

This extension allows you to export datasets from SPSS Modeler onto [Data.World](https://data.world/).

## Requirements

This extension requires the following
* IBM SPSS Modeler v18.1.1 or later
* IBM SPSS Modeler "Integration Plug-In for R"
* R v3.3.3

## Installation Instructions

This extension can be downloaded from the [Extension Hub](https://ibmpredictiveanalytics.github.io/)

## R packages used

This plugin will install the following R packages : 

* [Data.World](https://CRAN.R-project.org/package=data.world)
* [dwapi](https://CRAN.R-project.org/package=dwapi)
* [Properties](https://CRAN.R-project.org/package=properties)
* [stringr](https://CRAN.R-project.org/package=stringr)
* [httr](https://CRAN.R-project.org/package=httr)


## Other Requirements

This extension requires a Data.World Authentication Token. This token can be obtained from [here](https://data.world/settings/advanced)

## Steps

1. Download the extension from the Extension Hub

2. Click on the File Menu -> New Stream to create a new SPSS Modeler stream.

3. From the "Sources" node palette, drag drop "Var. File" onto the new stream. Select the attached test.csv file as input.<br>
![Image 1](/Resources/SPSS_Image_1.png)

4. From the "Output" node palette, drag drop "datadotworldexport" onto the new stream. This is the Data.World export node that will need to be configured. The following information has to be provided:<br>
    a. Data.World [authentication token](https://data.world/settings/advanced). This needs to be entered only the first time the extension is used.<br>
    b. Title - Sample dataset<br>
    c. Description - Sample dataset<br>
    d. Visibility - PUBLIC<br>
    e. Field chooser, select the columns (col1, col2, col3) to be exported to Data.World.<br>
    f. License String - Public Domain<br>
![Image 2](/Resources/SPSS_Image_2.png)    

5. Select the "Var. File" node, click on F2 and connect it to the "datadotworldexport" node.<br>
![Image 3](/Resources/SPSS_Image_3.png)

6. Execute the stream by clicking on the green play button<br>
![Image 4](/Resources/SPSS_Image_4.png)    
    
 ## Authors
 
* Deepak Rangarao
* Amod Upadhye

## Contact Information
For any issues while using this extension, please raise an issue on GitHub or send us an <a href="mailto:h6u9j3n4w2n7k6i7@ibm-analytics.slack.com">Email</a>
