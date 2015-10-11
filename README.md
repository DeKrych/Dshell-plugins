# Dshell-plugins
This is an unofficial library of plugins written by Penn State students for [Dshell](https://github.com/USArmyResearchLab/Dshell), the U.S. Army Research Lab's network forensic analysis framework.

For general questions regarding Dshell, please see their [README.md](https://github.com/USArmyResearchLab/Dshell/blob/master/README.md)

## Prerequisites
* [Dshell](https://github.com/USArmyResearchLab/Dshell), U.S. ARL's Dshell
* Dshell's Prerequisites
  * Linux (developed on Ubuntu 12.04)
  * Python 2.7
  * [pygeoip](https://github.com/appliedsec/pygeoip), GNU Lesser GPL
    * [MaxMind GeoIP Legacy datasets](http://dev.maxmind.com/geoip/legacy/geolite/)
  * [PyCrypto](https://pypi.python.org/pypi/pycrypto), custom license
  * [dpkt](https://code.google.com/p/dpkt/), New BSD License
  * [IPy](https://github.com/haypo/python-ipy), BSD 2-Clause License
  * [pypcap](https://code.google.com/p/pypcap/), New BSD License

## Setup
After installing Dshell, these additional decoders can be downloaded and moved to &lt;install-location&gt;/decoders/misc/
* To ensure that these decoders are now available for use within Dshell:
  * `./dshell` which runs Dshell (You should see the Dshell> prompt)
  * `decode -l` lists the available decoders

## Basic Usage
* `decode -d <decoder>`
  * Displays information about the decoder, including command-line flags
* `decode -d <decoder> <pcap>`
  * Runs the desired decoder on the pcap or list of pcaps
