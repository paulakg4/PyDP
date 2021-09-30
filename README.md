# PyDP
PyDP is a Python class for interacting with the DonorPerfect API

This is a project I am just beginning to work on and does not currently include much functionality. I will push updates as they are made. 

Coding is a hobby for me and there will probably be better ways to do what I've done. Feel free to contribute.


Example Usage:

from PyDP import *

dp = PyDP()

fieldname = "first_name"

donorid = 1

dp.getFieldValue(fieldname, donorid)
