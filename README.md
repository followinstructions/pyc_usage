# How to create pyc file

Using terminal,
````
import py_compile
py_compile.compile('filename.py')

````
# Using functions from pyc file

import filename of pyc as per normal.

# Example

# Use the following scripts

# 1. date_time.py ; Prints current date and time
````
import datetime
def date_time():
        now = datetime.datetime.now()
        print ("Current date and time : ")
        print(now.strftime("%Y-%m-%d %H:%M:%S"))
````

# 2. importing.py ; Script using **date_time() function** in Date_and_time script

````
from frame_count import date_time

date_time()
````
# In ubuntu terminal...
# Converting **py** file to **pyc** file

Using terminal ( NOT on pycharm)

>- run python
>- run the following codes
````
import py_compile
py_compile.compile('date_time.py')
````
A date_time.pyc file should be create in the same directory

Run importing.py **after** deleting the py file. The current date and time should be printed.
