# SWAN: CERN's Jupyter-based interactive data analysis service

## Diogo Castro (CERN)

1PB per second from detectors --> filtered and stored in [EOS](http://information-technology.web.cern.ch/services/eos-service)

first jupyter c++ kernel came from root C++


SWAN
* analysis in a web browser
* no local installation or configuration needed
* integration with resources comes on the back end
* 3 pillars
  * Software - CernVM file system
  * Infrastructure - docker jupyter
  * Storage - CERNBox, EOS
    * EOS - disk storage system
    * Software - CVMFS - read only software software distribution on world wide grid, lazy fetching
* project creation and sharing framework
* it's got spark

* WLCG - worldwide LHC computing Grid (storage and processing power)

[web](http://swan.web.cern.ch/)

200 daily users

* coming up
  * move to jupyter lab
  * base new architecture on kubernetes
  * get into GPUs to facilite hep usage of ML
  
* links
  * http://cern.ch/swan
  * https://github.com/swan-cern
  * https://cern.ch/sciencebox
