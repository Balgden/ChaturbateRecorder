# ChaturbateRecorder

This is script to automate the recording of public webcam shows from chaturbate.com. 


I have only tested this on debian(7+8) and Mac OS X (10.10.4), but it should run on other OSs

## Requirements

Requires python3.5 or newer. You can grab python3.5.2 from https://www.python.org/downloads/release/python-352/

to install required modules, run:
```
python3.5 -m pip install livesteramer bs4
```


edit lines 7 and 9 of ChaturbateRecorder.py to set the path for the directory to save the videos to, and to set the location of the "wanted.txt" file.
Line 11 of ChaturbateRecorder.py specifies which genders it woull check for models to record. The available genders are all listed in line 10. It is already set to check female and couples cams. You can add or remove genders, just make sure it remains a list of strings. This means it should start with "[" and end with "]" with each gender in double or single quotes and separated with commas ie: 
```
['female', 'male', couples']
```
or a single gender: 
```
['couples']
```

Add models to the "wanted.txt" file (only one model per line). The model should match the models name in their chatrooms URL (https://chaturbate.com/{modelname}/). 
