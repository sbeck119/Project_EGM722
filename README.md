# Project_EGM722
# Analysis of Green Space Accessibility in Belfast
## Setup/installation
### Prerequisites
Before you begin, make sure you have the following: 

•	An operating system such as Linux, macOS, or Windows (these download instruction will mainly relate to Windows) 

•	Python 3.8 or newer. Python can be downloaded from python.org

### Clone the Repository
The Git Repository will need to be cloned (downloaded to your computer) in order to have access to the datafiles and python script for the project and make any modifications to the script. 

Users should open a Command Prompt and navigate to the directory where the project will be downloaded into using cd:

````cd c:\Users\Shane\projects```` 

Enter the following command to clone the repository:

````git clone https://github.com/sbeck119/Project_EGM722.git````

This command will create a folder called ‘Project_EGM722’ in your directory chosen above and contain all files for the project. 
Note: After cloning, users may want to move into the project directory to start working with the files using: ````cd Project_EGM722````

### Installation of pip and Conda
The project will need to have several dependencies installed to work, these include Python 3.9, GeoPandas, Cartopy, Notebook, Rasterio, Pyepsg, Folium and Matplotlib. 
You can install these project dependencies using either pip or Conda package managers.

Conda is a powerful package and environment manager that runs on Windows, macOS, and Linux. It allows users to create separate environments for different projects and these will contain individual files, packages, and dependencies (Conda 2024). Pip is the package installer for Python and can install packages from the Python Package Index, PyPI (Anaconda 2024).

To begin you’ll need to install Anaconda from here: https://docs.anaconda.com/free/anaconda/install/ 

Here are the steps to set up a Conda Environment:

From the start menu open the Anaconda Command Prompt. 

 *Note you should see (base) at the beginning of the prompt. If you don’t you may be in the normal Command Prompt.* 

Navigate to your cloned repository:

````cd c:\Users\Shane\projects\Project_EGM722 ````

Create a new Conda environment: 

````conda env create -f newproj_env.yml````

This will create a new environment using the dependencies provided in the *newproj_env.yml* that is included in the repository. This may take several minutes.

Alternatively, you can use pip to install the dependencies. 

First, you need to install pip on your Conda environment using Anaconda Navigator or the command line interface:

````conda install -c conda-forge pip````

With pip installed, make sure the correct environment is activated and the use the Anaconda Command Prompt:

````pip install <package>````
### Datasets
The project requires several datasets: 
- wards.shp
- greenspaces.shp
- greenways.shp
- bikestations.cvs
- belfast_outline.shp

The datasets should be within the *‘Datafiles’* folder of the Git Repository. If they are missing the datasets can be obtained from the following resources – 

#### Dataset Source

| Name | Source |
| --- | --- |
|NI Wards: wards.shp |	opendatani.gov.uk|
|Belfast Outline: belfast_outline.shp |	ArcGIS.com- https://www.arcgis.com/home/item.html?id=4908e73f189e4c569155fd5ce65802ca |
|Bike Stations: bike_stations.cvs	| Belfast City Council |
|Greenways: greenways.shp	| ArcGIS.com -https://www.arcgis.com/home/item.html?id=3cbb936848354cd4801721c333c978ef# |
|Greenspaces: greenspaces.shp	| Outdoor Recreation Northern Ireland (ORNI) |

*Note*: Ensure that each dataset is downloaded in a shapefile or GeoJSON format, which is compatible with the GeoPandas library used in this project.
### Running the Script
To run the project, ensure **Python** and **Jupyter Lab** are installed on your system along with necessary libraries such as GeoPandas and Folium. You can install these using pip, input the following into your Anaconda command prompt:

````pip install jupyter lab````

Open Jupyter Lab by navigating to the project directory *‘cd Project_EGM722’* in the command line and input:

````jupyter lab````

Open the notebook *‘Project_EGM722.ipynb’* from the Jupyter Lab interface. Ensure you save your progress frequently.
