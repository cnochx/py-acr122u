# PY-ACR122U

<img src="http://downloads.acs.com.hk/product-website-image/acr38-image.jpg" width="150" height="150">

This is a python library for the ACR122U NFC reader

## Installation
- git clone from https://github.com/cnochx/py-acr122u
- cd py-acr122u
- pip install -r requirements.txt # -> to install the Dependencies
- this build replace the windows Driver, for that it's not necessary to install the windows driver

## Usage for Reading

+ To get the uid and the reader info neet the below code.
+ call the ´read.py´ in the **Terminal** with `python read.py`

```python
from src import nfc

reader = nfc.Reader()
reader.print_data(reader.get_uid())
reader.info()
```

## Usage for writing

+ in Example/write_and_read are some ideas for writing, but not checked yet.

## Further information

+ the ``src/nfc.py`` creates an ACR122U object
+ based on given information from acs.com 
+ doc available here: http://downloads.acs.com.hk/drivers/en/API-ACR122U-2.02.pdf
