Softflowd semi-statefully tracks traffic flows. Upon expiry of a flow, its statistics are accumulated and reports them to a designated collector host using the standard NetFlow protocol. 

See here for more details: https://code.google.com/archive/p/softflowd/

#### Installation (Red Hat Enterprise Linux / Derivatives)
Libs:
```
yum install libtool automake autoconf python-devel
libpcap-devel
```
Softflowd:
```
wget http://softflowd.googlecode.com/files/softflowd-0.9.9.tar.gz
tar -zxvf softflowd-0.9.9.tar.gz
cd softflowd-0.9.9
./configure
make
make install
```
Validate:
```
softflowd -h
```
#### License / Contributors
Copyright 2016 Damien Miller
 + License (3-Clause BSD) https://opensource.org/licenses/BSD-3-Clause
 + Project: https://code.google.com/archive/p/softflowd/
