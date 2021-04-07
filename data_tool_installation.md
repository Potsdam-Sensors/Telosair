# Mongodata Installation Guide :star:


![Image of Telosair](https://github.com/Potsdam-Sensors/Telosair/blob/main/img/telosair.png)


## :star2: Dwonload and install git for Windows
please Download and install git https://git-scm.com/download/win

## :star2: Download and install Anaconda 
Please Downlaod and install Anaconda  https://www.anaconda.com/products/individual 



## :star2:  After instalation complete, open the anaconda prompt
- in windows search bar type in anaconda prompt can help you find it 

### :dizzy:  Pip install pymongo
   * After you open the anaconda prompt , type in below command:

```python
pip install pymongo
```

### :dizzy:  Pip install plotly
   * After the pervious installation done , type in below command:

```python
pip install plotly
```

### :dizzy:  Install MongodataTool
   * After the pervious installation done , type in below command to build new directory:

```python
mkdir github
```

* then type in below command to move in to the directot you build:

```python
cd github
```

* Now clone the script from Telosair githubpage by type in:

```python
git clone https://github.com/Potsdam-Sensors/Mongo_data.git
```

:exclamation: **Note** : this require username and password (contact kuerbanjiang@telosair.com for username and password)

* After you cloned the script, move in to the directory:

```python
cd Mongo_data
```

* Last step is install the script:

```python
python setup.py install
```

### :dizzy:  Open the jupyter Notebook then start analyse your data

* On Windows, you can run Jupyter via the shortcut Anaconda adds to your start menu(windows search bar), which will open a new tab in your default web browser
 



