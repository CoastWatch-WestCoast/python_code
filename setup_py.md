# satellite_course_python_code 

## Viewing the exercises
The python exercises are a series of Jupyter Notebooks that are hosted on a GitHub repository. You can view a single exercise to see if it is of interest by 
clicking the linked name of each exercise in the **Exercises** section below. A non-executable version of the exercise will open in a new browser window.   

<!--If you want an executable version of a single Notebook, you can save a Notebook to your computer using the save menu in your browser while viewing the file online. To get all of the Notebooks, you can go to the GitHub repository and download a zip file with all of the exercises included. To download the repo and run the Notebooks on your computer:
-->
## Running the exercises
### Setup and test your python environment: 

1. Make sure you have __python 3__ and __conda__ installed on your machine
2. Download this repository. 
    * Use the green __Code__ dropdown to select __Download Zip__ and unzip to a location on your computer
    * Or [use this zip file link](https://github.com/CoastWatch-WestCoast/python_code/archive/refs/heads/satellite_course_jan_2022.zip)
3. Use a terminal window to navigate to the unzipped folder 

The following commands:  
* Update conda
* Create a new conda environment named 'coastwatch' and load the required modules to it  
* Activate the environment  
* Runs a script that checks for any missing modules  
* Launches jupyter-lab for displaying the jupyter notebook tutorials  

```
conda update conda
conda env create -f environment.yml
conda activate coastwatch
python check_modules.py
jupyter-lab
```

## Exercises
The first three exercises demonstrate the CoastWatch R code tutorials as python code. They show you how to extract gridded data from ERDDAP inside a box or polygon, and along a track. Additional examples demonstrate practical applications of working with time-series of satellite data.  
1. **[Get Data Using a Rectangular Bounding Box](extract_box.ipynb)**  
Demonstrates how to extract environmental data from an ERDDAP server in an rectangular bounding box (polygon) over time.  
2. **[Get Data Along a Track](extract_track.ipynb)**  
Extract environmental data from an ERDDAP server along an x,y and time trajectory, e.g. an animal or cruise track.  
3. **[Get Data Using an Irregular Shape](extract_irregular_shape.ipynb)**  
Extract environmental data from an ERDDAP server in an irregular bounding box (polygon) over time, e.g. a marine protected area.  
4. **[Comparing time-series of different satellite datasets](compare_satellite_timeseries.ipynb)**  
Several satellite ocean color sensors have been launched since 1997 to provide a continuous record of global ocean color data. This exercise examines the variability of Chlorophyll-a values during time periods where the satellite measurements overlap.  
5. **[Creating a virtual buoy](virtual_buoy_timeseries.ipynb)**   
Create a virtual buoy from satellite data for locations where in-situ buoy data may not be available or has been discontinued.  
