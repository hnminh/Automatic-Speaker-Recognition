#  Speaker Identification Using GMMs
This is done for final project of Digital Signal Processing.  

I have modified this code to run on Linux. In Window, there will be some differences in paths and commands.

## Installation
### 1. Install Anacoda 64-bit Python 2.7 version
For Linux  
Go to the following link: Anaconda.com/downloads.
Copy the bash (.sh file) installer link.  

Open command line  
Use wget to download the bash installer
```
$ cd ~
$ mkdir tmp
$ cd tmp
$ wget <bash-link>
```

Run the bash script to install Anacoda
```
$ ls <bash file of Anacoda>
$ bash <bash file of Anacoda>  
```

Source the .bash-rc file to add Anacoda to your PATH
```
$ cd ~
$ source .bashrc
```

Verify the installation
```
$ python

Python 3.6.5 |Anaconda, Inc.| (default, Mar 29 2018, 18:21:58)
[GCC 7.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

### 2. Install packages
To install `python_speech_features` package
```
pip install python_speech_features
```
In case `pip` is not downloaded
```
apt install python-pip
```
## Dataset
Audios using for this project will be stored in *development_set*  `
### 1. Training Data
Dataset (file to be trained) need to be located in folder *dataset*.  
To generate list of (path) file to be trained
```
python train_list_generator.py
``` 
A file named *speaker_models* will be produced.  
Training model will be stored in *speaker_models* folder.

### 2. Testing Data
Testing data need to be located in folder *testing_data*.  
To generate list of (path) file to be tested
```
python test_list_generator.py
```
A file named *development_set_test.txt* will be produced.

## Reference
Source code: https://github.com/abhijeet3922/Speaker-identification-using-GMMs
