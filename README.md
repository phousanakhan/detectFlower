# WhatFlower
Created an IOS application using Swift that can identify and provide a brief description of a plant. 
Integrate a caffe model that was trained on Oxford 102 flower dataset to detect the plant species. 
Employed a networking system between the application and MediaWiki API. 


### Requirements
1. Xcode 11.5 or higher
2. IOS 13.X.X or higher


[Classifier.zip](https://drive.google.com/file/d/1QGDMgSj-UCX0E_tH0E2LHvizhNGTN1Du/view?usp=sharing)

### Installing - Part 1: Creating Virtual Environment (Needed to install coremltools)
```
cd
mkdir Environemnts
virtualenv --python=/usr/python3.7 python37
source python37/bin/activate
pip install -U coremltools
```

### Installing - Part 2: Creating .mlmodel file from .caffemodel
1. Download "Classifier.zip"
2. Place convert_script.py into the unzipped file
3. Making sure that you're in the virtual environment, do the following:
```
python3 convert_script.py
```
4. Drag and drop .mlmodel file into Xcode

## Contribution
Angela Yu


## Demo
![](flower.gif)
