# NanoSDR

## Applications

### Introduction
Most of the applications installed are supporting SoapySDR.
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
gr-iio module (PlutoSDR) is also installed  

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
QSSTV has benn installed from repository, since sources are not available.
#### WS-JTX 2.2.0
Compiled from sources : 

#### LuaRadio 0.8
https://luaradio.io  

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
