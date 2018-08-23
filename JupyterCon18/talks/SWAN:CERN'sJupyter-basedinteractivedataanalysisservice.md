# SWAN: CERN's Jupyter-based interactive data analysis service

## Diogo Castro (CERN)

1PB per second from detectors --> filtered and stored in EOS

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
