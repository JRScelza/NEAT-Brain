# Welcome to NEAT-Brain!

FRANCIS (**F**ast g**RA**ph **N**etwork metabolomi**C**s analysis**)** is a graph network-based bioinformatics pipeline for the exploration and analysis of liquid chromatography-mass spectrometry (LC/MS) based metabolomics data either from untargeted or targeted assays and with or without related knowledge bases. The software emphasizes modern and interactive graph network-based visualizations and also includes rudimentary statistical tools for pre- and post- processing methods


# Project Structure

/src
These are all of the tooling modules. For this project the files are provided in Jupyter notebook form in Python+3.1

	#Spectral signal visualization
	lcms_spectre_exploration.ipynb

	#Metadata exploration
	sample_data_exploration.ipynb

	#Graph network creation
	graph_network.ipynb

	#Statistical packages for analysis of compounds
	statistical_analysis_functions.ipynb

/data
These are all of the sample data files required for running the programs


	#The spectral data for the 8000 compounds
	compound_data.csv

	#Compund metadata and pathway relations
	compound_descriptions.csv

	#Sample demographic data from participants
	study_metadata.csv

## Run Jupyter Notebooks
The only interaction to run the programs are to define you root path:

	#Bring in the data
	PATH = '{PATH}/data/'
	data = pd.read_csv(PATH + "compound_descriptions.csv")

Make sure that you specify your own local ROOT. The data pathway is predefined and the individual notebooks also define the data file, no need to change. 


## Data Source

Journal
Scientific Reports 
URL
https://www.nature.com/articles/s41598-020-72914-7
Authors
Inoncent Agueusop, 
Petra B. Musholt, 
Beate Klaus, 
Kendra Hightower & 
Aimo Kannt
Citation
Agueusop, I., Musholt, P.B., Klaus, B. et al. Short-term variability of the human serum metabolome d...