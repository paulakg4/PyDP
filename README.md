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
### Get codes (solicitation, gl, etc)
```
getCodes = dp.getCodes("SOLICIT_CODE")
[print(x) for x in getCodes]
```
### Update a donor (default DP fields only)
```
update_donor = dp.updateDonor(donor_id=34980, narrative="Has a lot of money")
```
### Update a donor udf code
```
update_udf = dp.updateDonorUDF(donor_id=34980, field_name="custom_fieldname", data_type="C", char_value="Some text to put in your custom field")
```
