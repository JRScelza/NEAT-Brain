# Welcome to NEAT-Brain!

https://github.com/JRScelza/NEAT-Brain/tree/main/data

NEAT-Brain (Nash Equilibrium Analysis Tool for Brain Metabolism) is an interactive dashboard for the exploration of brain metabolism based on game theory. This software utilizes a modified Bayesian Nash Equilibrium algorithm to model the biochemical resource competition in brain metabolism and the suboptimal payoffs associated with neurodegenerative disease with an emphasis on Alzheimer’s. Alzheimer’s disease (AD) is an age-associated, multifactorial neurodegenerative disorder that is the incurable. 

![alt text](https://github.com/JRScelza/NEAT-Brain/blob/main/brain_metabolism.png?raw=true)

# Project Structure

/src
These are all of the tooling modules. For this project the files are provided in Jupyter notebook form in Python+3.1

	
	# NEAT-Brain Game Theory Simulator.ipynb
	This is the main notebook. It walks throught the statistical analysis and the Nash Equilibrium simulation.

	# constants.ipynb
	This notebook is a STATIC set of the biochemical reaction constants.

	# data_generator.ipynb
	This is a simple script file that can create the data set used in the simulation

	# ODE_functions_timeseries.ipynb
	This notebook houses all of the functions from the Cloutier et Al. paper that are the differential equations for the dynamic modeling of the reaction curves. 

	# timeseries_visualization.ipynb
	This is a simple notebook for visualizaing any of the individual curves.

/data
These are all of the sample data files required for running the programs


	# cloutier_2009_data_w_params.csv
	The pre-processed data. This includes non-functional parameters from the model that are not used in the simulator.

	# cloutier_2009_data.csv
	The post-processed data. This is the core dataset uses by the simulator

# Run Jupyter Notebooks
## Local Python Installation


The easiest and most compact way to install Python is to use Miniconda (https://conda.io/en/latest/miniconda.html) distribution. While most people recommend Anaconda, which includes a large collection of Python libraries, I would rather start with barebone installation of Python, and install those packages that are really required. With Miniconda, initial distribution is only around 50 Mb, while Anaconda is close to 500 Mb in size.

After installing Miniconda, you would need to install Jupyter:

```
conda install -c conda-forge notebook
```

or

```
pip install notebook
```

After the installation, navigate to the folder where your notebooks are located, and start Jupyter server:

```
jupyter notebook
```

After this, browser window will open, and you are good to go.

----


The GitHub also includes information on Python libraries that are required to run the code. This is stored in the requirements.txt file. 

```
pip install -r requirements.txt 
```

### Finally, you can navigate to the main simulator file to run NEAT-Brain!
 <br>

NEAT-Brain Game Theory Simulator.ipynb

The notebook includes its own walkthrough. 

## Data Source

An integrative dynamic model of brain energy metabolism using in vivo neurochemical measurements, Mathieu Cloutier, Fiachra B. Bolger, John P. Lowry and Peter Wellstead, 2009, Journal of Computational Neuroscience, 27, 391-414. PubMed ID: 19396534

https://models.cellml.org/exposure/6e249a04f5c751e42ba41504d84e6e49
