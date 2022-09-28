# climate-ml-tutorial

* [Introduction](#introduction)
* [README](#readme)
* [CEDA_Data_Retrieval](#ceda_data_retrieval)

## Introduction

This repository is for the Met Office Data Science Community of practice and their partners. It contains information on:

* CEDA data retrieval 

* Exploring gridded data with iris 

* Exploring tabular data with pandas 

## README

These notebooks should be self contained and have all the information within them you will need. Each notebook has links to extra relevant resources such as code documentation if you'd like to learn more or need help. 

## CEDA_Data_Retrieval

### What is Ceda

The Centre for Environmental Data Analysis (CEDA) serves the environmental science community. They provide compute and data archives for the user. These notebooks run with data retrieved from the CEDA archive. The data used is publicly available and can be accessed once a free account has been made. 

### Guide to retrieve CEDA data

* Register with CEDA: <https://services.ceda.ac.uk/cedasite/register/info/>
* Open up a terminal on your machine
* Downloading a file with CURL: <https://help.ceda.ac.uk/article/4442-ceda-opendap-scripted-interactions#curl>
* Follow the instructions under Getting started
    * This will make a directory for certification with CEDA 
    * clone a github repository with relevant code
    * get trustroots and a Security Certificate 
    * Beware the security certificate lasts 3 days, after this the command will need to be run again 
* You can now run a curl command, we use the first NetCDF in the example, so that can be downloaded 

` curl --cert $PWD/creds.pem -L -c /dev/null http://dap.ceda.ac.uk/thredds/fileServer/badc/ukmo-hadobs/data/insitu/MOHC/HadOBS/HadUK-Grid/v1.0.0.0/1km/tas/ann/v20181126/tas_hadukgrid_uk_1km_ann_188901-188912.nc -o tas_hadukgrid_uk_1km_ann_188901-188912.nc `

* Beware that this file will be downloaded to your current directory, to specify the file location, add the full path. For example:

` curl --cert $PWD/creds.pem -L -c /dev/null http://dap.ceda.ac.uk/thredds/fileServer/badc/ukmo-hadobs/data/insitu/MOHC/HadOBS/HadUK-Grid/v1.0.0.0/1km/tas/ann/v20181126/tas_hadukgrid_uk_1km_ann_188901-188912.nc -o data/user/Ceda_data/tas_hadukgrid_uk_1km_ann_188901-188912.nc `

* all we need to do to download other files, is navigate to them in the CEDA archive, find the relevant link and replace in the command above
* For the other data file we need <https://data.ceda.ac.uk/badc/ukmo-hadobs/data/insitu/MOHC/HadOBS/HadUK-Grid/v1.0.3.0/12km/rainfall/day/v20210712>
    * Please explore the different file levels to see the different data types that can be accessed 
* The first file on the page is the one we need for our notebook
* Click the 3 cogs on the right
    * you should see a data url on this page
    * we don't need all of this url, just everything from badc onwards
    * you can see how the urls are similar to the example, just replace the example url with the current url

<img src="highlighted_curl.PNG" />

* replace the highlighted green with the url: badc/ukmo-hadobs/data/insitu/MOHC/HadOBS/HadUK-Grid/v1.0.3.0/12km/rainfall/day/v20210712/rainfall_hadukgrid_uk_12km_day_18910101-18910131.nc
* replace the highlighted blue with the filename: rainfall_hadukgrid_uk_12km_day_18910101-18910131.nc
    * note any filename can be used, but id recommand sticking to the current filenames 
        
        




