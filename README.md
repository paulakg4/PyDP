# PyDP
## PyDP is a Python class for interacting with the DonorPerfect API

This is a project I am just beginning to work on and does not currently include much functionality. I will push updates as they are made. 

Coding is a hobby for me and there will probably be better ways to do what I've done. This is also the first time I've worked with XML data. Feel free to contribute.


Example Usages:
### Create Instance
```
from PyDP import *
dp = PyDP()
```

### Get the value of a field
```
fieldname = "first_name"
donorid = 1
dp.getFieldValue(fieldname, donorid)

# Returns field value
```
### Create a contact entry
```
dp.createContact(donor_id=donorid, activity_code="LT", comment="Sent this person a letter")

# Returns the contact id if successful
```
