# Name Entity Recognition using BERT


## DESCRIPTION OVERVIEW
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

Named EntitiesRecognition (NER) is a basic task of Natural Language Processing (NLP). The purpose is to identify named entities such as person names, place names, and organization names in the corpus. Due to the increasing number of these named entities, it is usually impossible to exhaustively list them in the dictionary, and their constituent methods have some regularities. Therefore, the recognition of these words is usually included in the task of morphological processing (such as Chinese segmentation). Independent processing, called named entity recognition. 

Named entity recognition technology is an indispensable part of many natural language processing technologies such as information extraction, information retrieval, machine translation, and question answering systems.

Named entities are the research subjects for named entity recognition. Generally, named entities include 3 categories (entity, time, and number) and 7 categories (person, place, institution, time, date, currency, and percentage). Judging whether a named entity is correctly identified includes two aspects: whether the boundary of the entity is correct; and whether the type of the entity is correctly labeled. 

The main types of errors include correct text, which may be of the wrong type; conversely, text boundaries are incorrect, and the main entity words and part-of-speech tokens it contains may be correct.


## TECHNOLOGY USE
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Here we will be using  Anaconda Python 3.6 , Pytorch 1.4 with GPU support CUDA 10 with CuDNN 10.



## INSTALLATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

**In Pycharm it’s easy** 

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using _conda_ with _python3.6_
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from **requirements.txt** file using the command _`pip install -r requirements.txt`_


**In Conda also it’s easy**

1. Create a new virtual environment using the command
    _`conda create -n your_env_name python=3.6`_
2. Navigate to the project directory.
3. Install the necessary packages from **requirements.txt** file using the command         
_`pip install -r requirements.txt`_

## WORKFLOW DIAGRAM
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211196857-a827fc45-b805-4460-9ced-9956ee82b918.png" width=60%/>
</p>


## IMPLEMENTATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

### 1. Project Directory
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211196881-2b4b1d3d-9140-4a24-9357-0241a6be71e5.png" width=60%/>
</p>

This above picture shows the folder structure of the project. Here data folder consists of data and out_base folder consists of the BERT models.

### 2. requirements.txt
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211196910-14797817-dbe7-40de-b813-1e3d809f2b7c.png" width=60%/>
</p>

requirements.txt file consists of all the packages that we need to run with project.

### 3. bert.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211196939-de61f7ea-81bf-40e6-9bc0-d146d4b2b8ff.png" width=60%/>
</p>

This is the most important file in this project which we will be using for training and prediction.

### 4. clientApp.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211196983-d5c58678-1f6c-4cb8-9fd0-1c8a540e78db.png" width=60%/>
</p>

This is the flask server file and the entry point of application.

## TESTING IN LOCAL/API
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

To do the test testing we need to run the **clientApp.py** and after that web server will start at **http://0.0.0.0:5000/**
<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211197059-241b0171-7d39-4fcd-946a-91a0791476fc.png" width=60%/>
</p>

Enter the Text and click on Predict button.

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211197088-cbf1fd97-2cbb-43da-8e72-e797f73b00fc.png" width=60%/>
</p>

Predictions will be shown in the result box. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211197116-fe7e66f0-4d10-4de4-8d61-9fe047e1bc80.png" width=60%/>
</p>


## CONCLUSION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Here we successfully performed Named Entity Recognition on the given dataset.

## COMPARISION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

More data or better larger dataset can be used to build a better model. We can also try out better pre trained model with fine tuning to increase the performance.

## Download Link & Reference
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
* [Drive](https://drive.google.com/drive/folders/1W34qcPjXOANpSE7tHGyZ-c1EV3ghAZuM?usp=sharing)
* **Time**- _12-March-22,1:40:44_

