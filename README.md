# DYMO-CUPS-Drivers
### About
The driver contained here is a fork of the drivers available for download
from DYMO's website, which doesn't seem show a download link at this time.

This driver is minimally modified to allow for compiling, and execution on a modern linux system.

### Build and install
```bash
./configure
make && sudo make install
```

### Command line examples

- Print very long text on a tape:
```bash
lpr -o landscape -o PageSize=24_mm__1___Label__Auto_ docs/test.txt
```

- Set printing options for the LabelWriter driver:
```bash
lpr -o PageSize=30252_Address -o PrintQuality=Graphics -o PrintDensity=Light docs/test.txt
```

- Set printing options for the LabelManager driver:
```bash
lpr -o PageSize=Address_Label -o CutOptions=ChainMarks -o LabelAlignment=Right -o TapeColor=1
```


