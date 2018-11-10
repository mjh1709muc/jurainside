# Please upload you EEPROM dumps to this folder

But: Don't upload faulty dumps please! The first thing you should do before anything else is a backup of your EEPROM!

Create them with the EEPROM-Tool. 

File naming scheme: 
```
<MANUFACTURER>-<MODEL>_<APPLIANCE-NO>_<NEW/ORG>_<ELECTRONIC-VERSION>_<DUMPDATE-YYYYMMDD>.txt
```

```<NEW/ORG>``` - Choose

```NEW```: if the machine was never used.

```ORG```: when you didn't change anything directly in the EEPROM.

Example:
```
Jura-F90_ORG_20253_E90MASK6+_20181110.txt
```

They should have the following structure:
```
# <MANUFACTURER> <MODEL> / <NEW/ORG>
# Typ: <TYP>
# EAN: <EAN>
#
# User: <YOURNAME>
# Date: <DUMPDATE-YYYY-MM-DD>
#
# Electronic: <ELECTRONIC-VERSION>
# Serial No.: <SERIAL-NO>
# Appliance No.: <APPLIANCE-NO>
# Prod. Date: <PRODUCTION-DATE-DDMMYYY>
# Elec. Date: <ELECTRONIC-DATE-DDMMYYY>

<ADDR>  <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> 
<ADDR>  <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> <DATA> 
```

```<TYP>``` is on the label under the coffeemaker
```<EAN>``` is the EAN-code. You can use this page to find it https://www.kaffeevollautomaten.org/kaffeemaschinen/

Use key combinations to find ```<ELECTRONIC-VERSION>, <SERIAL-NO>, <APPLIANCE-NO>, <PRODUCTION-DATE-DDMMYYY>, <ELECTRONIC-DATE-DDMMYYY>```

https://github.com/mjh1709muc/JuraInside/wiki/Key-combinations

Sometimes the ```<APPLIANCE-NO>, <SERIAL-NO>``` are printed on a barcode label.


Example:

```
# Jura F90 / ORG
# Typ: 629
# EAN: 7610917131129
#
# User: mjh1709muc
# Date: 2018-11-10
#
# Electronic: E90 Mask6+
# Serial-Nr.: 102
# Appliance-Nr.: 20253
# Prod. Date: 9 92002
# Elec. Date: 9 82002

0000  22B5 00B2 1399 1CBE 019B 0014 0007 3762 
0008  0071 003C 1678 0010 0000 01D5 0001 0048 
```
