---
path: "/ksptot_on_linux"
date: "2019-01-19"
title: "KSP Trajectory Optimization Tool on Linux"
project: "kerbal space program"
---

## Installing

Tested on Ubuntu 18.04.1 LTS.

1.  Download MATLAB Runtime R2017b for Linux from
    http://ssd.mathworks.com/supportfiles/downloads/R2017b/deployment_files/R2017b/installers/glnxa64/MCR_R2017b_glnxa64_installer.zip.
    The rest of these instructions will assume that it was downloaded to `~/Downloads`.
2.  `mkdir -p ~/MCR`
3.  `cd ~/MCR`
4.  `unzip ~/Downloads/MCR_R2017b_glnxa64_installer.zip`
5.  `sudo ./install`
6.  `sudo ln -s /usr/local/MATLAB/MATLAB_Runtime/v93 /usr/local/MATLAB/R2017b`
7.  `cd ..`
8.  `rm -rf MCR`
9.  `rm ~/Downloads/MCR_R2017b_glnxa64_installer`
10. Download KSPTOT. (See below for URLs, or check the forum for the latest release.)
11. `mkdir -p ~/KSPTOT`
12. `cd ~/KSPTOT`
13. `unzip ~/Downloads/(name of zip file)`
14. `chmod +x run_KSPTrajectoryOptimizationTool.sh KSPTrajectoryOptimizationTool`

## Running

1.  `cd ~/KSPTOT`
2.  `./run_KSPTrajectoryOptimizationTool.sh /usr/local/MATLAB/R2017b`

## Notes

All available versions of MATLAB Runtime can be found at https://www.mathworks.com/products/compiler/matlab-runtime.html.
Each release of KSP TOT depends on a single specific version of MATLAB Runtime, which should be listed in the README file for it.

URLs for KSPTOT:

* v1.6.1 for Linux: https://drive.google.com/file/d/1prOSwfGroTJ_MNjp1FAvj8qDuWZpRXgk/view?usp=sharing
* v1.6.2 pre-release 3: https://drive.google.com/file/d/1pvjlFK0r19wM9MzwwKT_i_R6us1tDhws/view?usp=sharing (includes both Windows and Linux)
* v1.6.2 pre-release 4: https://drive.google.com/file/d/1pxIHzTH3vVpKfIgRgjE1GrM_8tF8Mzou/view?usp=sharing (includes both Windows and Linux)
