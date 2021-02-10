# Exploration in Arts (Capstone project for the EPFL Extension School)

Welcome to the repository for my capstone project in the program "Applied Data Science: Machine Learning" at the EPFL Extension School.

The goal of this project was to showcase the skills acquired along the program, in data analytics and machine learning. 
I applied these skills in the context of art collections, a subject I feel passionate about. Indeed, the Arts are an interesting mean of communication throughout history and from all corners of the world. 
Recent digitalization efforts from museums enable to create new exciting opportunities for exploration with data sciences.

## Data source
The data used in this project comes from the Metropolitan Museum of Art digital catalogue and online database. 
The museum provides a large list of its collection, covering various types of pieces. 
I retrieved the text data from their github repository: https://github.com/metmuseum/openaccess on 30 October 2020. 
In addition, I used their API, following the indications here: https://metmuseum.github.io/
In order to avoid any issues with legal rights, I only used the data for the art pieces labelled as 'Open Access' by the MET.
In this repository, I uploaded a list of the artworks' ID after cleaning, for easy access. 

## Jupyter notebooks
I have fragmented my work into three parts: data preparation, 1st machine learning task and 2nd machine learning task. 

For data preparation, there are two Jupyter notebooks :
- DataPrep_EDA-ChristelCHAPPUIS.ipynb --> the main notebook for data cleaning
- API_file_treatment.ipynb --> a side notebook to perform and treat requests done to the MET website. The motivation was to retrieve information about dimensions and the url for the image. For cleanliness, it was done separately. The output of this notebook is a text file that can then be read in the main data preparation notebook.

For the 1st machine learning task: 'Where is this art piece ?' (predict the department, classification task, imbalanced dataset) :
- ML1-ChristelCHAPPUIS.ipynb

For the 2nd machine learning task: 'What is this art piece ?' (predict the category, classification task, 600 images of coin/dress/earrings/painting/stone sculpture/sword) :
- ML2-ChristelCHAPPUIS.ipynb

### Note
The two machine learning tasks are completely independant. For the second task, the images are retrieved inside the notebook directly with a url request.
