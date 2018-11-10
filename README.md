# ML_PneumDetect_2018
This is a final project repository for course 520.612: Machine Learning for Signal Processing at Johns Hopkins University. The project is based off of the kaggle competition. (Datasets are not included but can be found from kaggle with proper terms of agreement)

### Getting the Data
The data can be found through the kaggle competition: https://www.kaggle.com/c/rsna-pneumonia-detection-challenge/data. It can also be downloaded through the kaggle api: 

```shell
kaggle competitions download -c rsna-pneumonia-detection-challenge
```

Please download and unzip the files to a directory /data inside the root folder. The .gitignore is set to ignore the data due to both the terms of usage with kaggle and the size. 

### Libraries

* scikit-learn
* pandas
* numpy
* seaborn
* matplotlib
* scipy
* ipython
* jupyter (formerly ipython) notebook
* textblob
* re
* nltk
* csv
* io
* datetime
* os 
* sys
* pydicom

###

One way to get a majority of these libraries, especially pandas, scikit-learn and the other standard Machine learning ones is through the [Anaconda Python Distribution](https://www.anaconda.com/download/#macos)from Continuum Analytics. To install this, click on the link and follow the directions.  You will want to then use the package manager conda to install any missing packages.  When I tried this recently, I only had to run the following command to get all of the packages listed above:

```shell
$ conda install seaborn
```

A word of caution: if you install Anaconda, you will be asked if you want to put the Anaconda python interpreter in your path.  If you do this, you will use Anaconda by default instead of other Python versions that have been installed on your computer.  This can mess with existing software.  If you want to get around this, simply say "no" to adding the Anaconda interpreter to you path.  You can manually decide to use the anaconda interpreter by creating the following shell script (let's assume we put it at ~/use_anaconda.sh; of course you will also want to make sure the path is to your installed location of Anaconda).

```shell
#!/bin/bash
export PATH = /home/wtang/anaconda2/bin:$PATH
```

To use Anaconda you would simply type: 
```shell
$ source ~/use_anaconda.sh
```
Then you can startup a Python interpreter or 

```shell
jupyter notebook
```
to launch the notebooks

### Other libraries

```shell
pip install -U pydicom
````