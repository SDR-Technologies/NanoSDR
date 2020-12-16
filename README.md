# NanoSDR

## Download link
Download image corresponding to your Jetson-Nano. 
Take care to use adequate image since hardware is not the same for Nano-2GB and nano 4GB models.


## Default user
Default user is `ubuntu` , default password : `ubuntu`  
First boot is longer than usual since the Nano needs to recreate SSH keys, and expand filesystem partition to maximum available size.  
Once session is openend feel free to change locale settings and keyboard mapping.  
Pre-installed languages/keyboards : english-US, french, german, spanish.  

## Installed applications

### Introduction
Most of installed applications are supporting SoapySDR.
However only RTLSDR and PlutoSDR support have been deeply tested.  
Feel free to install SoapySDR module corresponding to your device if not yet installed.


#### SoapySDR
Current version installed on NanoSDR is v0.8  
Supported modules are : BladeRF, plutoSDR, RTLSDR, SDRPlay, SoapyRemote

```
######################################################
##     Soapy SDR -- the SDR abstraction library     ##
######################################################

Lib Version: v0.8.0-g926c86d9
API Version: v0.8.0
ABI Version: v0.8
Install root: /usr/local
Search path:  /usr/local/lib/SoapySDR/modules0.8
Module found: /usr/local/lib/SoapySDR/modules0.8/libPlutoSDRSupport.so (0.2.0-6e2ae74)
Module found: /usr/local/lib/SoapySDR/modules0.8/libbladeRFSupport.so  (0.4.1-1c1e8aa)
Module found: /usr/local/lib/SoapySDR/modules0.8/libremoteSupport.so   (0.6.0-c09b2f1)
Module found: /usr/local/lib/SoapySDR/modules0.8/librtlsdrSupport.so   (0.3.1-bec4f05)
Module found: /usr/local/lib/SoapySDR/modules0.8/libsdrPlaySupport.so  (0.3.0-8c4e330)
Available factories... bladerf, plutosdr, remote, rtlsdr, sdrplay
```

#### GNUradio 3.8.2
This version was installed from PPA sources  
gr-iio module (PlutoSDR support) is also installed.  

#### osmocom & gr-osmocom 
- built-in source types: osmosdr rtl uhd plutosdr miri rfspace soapy redpitaya spyserver    

Specific compilation with plutoSDR and SpyserverClient  
https://github.com/dk2ro/gr-osmosdr-pluto-spyserver


#### GQRX
This is the latest version compiled from sources : https://github.com/csete/gqrx
 
#### SigDigger
https://github.com/BatchDrake/SigDigger

#### Inspectrum
https://github.com/miek/inspectrum

#### URH
https://github.com/jopohl/urh

#### QSSTV  
QSSTV has been installed from Ubuntu repository, since sources are not available.

#### WS-JTX 2.2.2
Compiled from sources available here: https://physics.princeton.edu/pulsar/k1jt/wsjtx-2.2.2.tgz

#### LuaRadio 0.8
LuaRadio can be used to rapidly prototype software radios, modulation/demodulation utilities, and signal processing experiments. It can also be embedded into existing radio applications to serve as a user scriptable engine for signal processing.
LuaRadio is very similar to GNUradion using blocks, sources, sinks, except it use scripts.  
Very nice examples are provided on the website for RTLSDR device, can be adapted to other devices through SoapySDR.
Website : https://luaradio.io  

#### RTLSDR_Airband
https://github.com/szpajder/RTLSDR-Airband/

Compiled with specific options : `PLATFORM= armv8-generic make NFM=1 PULSE=1 WITH_RTLSDR=1 WITH_SOAPYSDR=1` 

#### FFMPEG (GPU acceleration)
https://github.com/jocover/jetson-ffmpeg  
This is a full version of FFMPEG including all formats available.
Since it's relies on hardware for acceleration, you have to run it as `sudo` user.

#### rtl_433 (soapy support)
https://github.com/merbanan/rtl_433
#### rx_tools (soapy)
https://github.com/rxseger/rx_tools
#### tx_sdr
Tool for transmitting data to SDRs, based on rtl_sdr from librtlsdr, and rx_sdr from rx_tools, using the SoapySDR vendor-neutral SDR support library, intended to support a wide range of TX-capable devices.  
https://github.com/triq-org/tx_tools

This tool has not been tested due to lack of time ...
#### dump1090 (/usr/bin/readsb)
https://github.com/Mictronics/readsb  
Note : original executable "dump1090" as been renamed by the author. Use `readsb` command instead.




## Thank you !  
First, thanks to the authors of those nice SDR applications !  

Thank you for giving your time testing the nanoSDR image and providing suggestions and ideas:
- F4GKR 
- F5OEO  
- F5OZP 
- LamaBleu


