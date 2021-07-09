
FIRASIM-[![Build Status](https://travis-ci.org/RoboCup-SSL/grSim.svg?branch=master)](https://travis-ci.org/RoboCup-SSL/grSim)[![CodeFactor](https://www.codefactor.io/repository/github/parsianroboticlab/grsim/badge/master)](https://www.codefactor.io/repository/github/parsianroboticlab/grsim/overview/master)
=======================


![FIRASIM on Ubuntu](docs/img/screenshot01.jpg?raw=true "grSim on Ubuntu")

- [Install instructions](INSTALL.md)
- [Authors](AUTHORS.md)
- [Changelog](CHANGELOG.md)
- License: [GNU General Public License (GPLv3)](LICENSE.md)

System Requirements
-----------------------

FIRASIM will likely run on a modern dual core PC with a decent graphics card. Typical configuration is:

- Dual Core CPU (2.0 Ghz+)
- 1GB of RAM
- 256MB nVidia or ATI graphics card

Note that it may run on lower end equipment though good performance is not guaranteed.


Software Requirements
---------------------

FIRASIM compiles on Linux (tested on Ubuntu variants only) and Mac OS. It depends on the following libraries:

- [CMake](https://cmake.org/) version 3.5+ 
- [OpenGL](https://www.opengl.org)
- [Qt5 Development Libraries](https://www.qt.io)
- [Open Dynamics Engine (ODE)](http://www.ode.org)
- [VarTypes Library](https://github.com/jpfeltracco/vartypes) forked from [Szi's Vartypes](https://github.com/szi/vartypes)
- [Google Protobuf](https://github.com/google/protobuf)
- [Boost development libraries](http://www.boost.org/) (needed by VarTypes)

Please consult the [install instructions](INSTALL.md) for more details.

Usage
-----

Receiving data from FIRASIM is similar to receiving data from [SSL-Vision](https://github.com/RoboCup-SSL/ssl-vision) using [Google Protobuf](https://github.com/google/protobuf) library.
Sending data to the simulator is also possible using Google Protobuf. Sample clients are included in [clients](./clients) folder. There are two clients available, *qt-based* and *Java-based*. The native client is compiled during the FIRASIM compilation. To compile the Java client, please consult the corresponding `README` file.


Qt [example project](https://github.com/robocin/ssl-client) to receive and send data to the simulator.

If you use this in your research, please cite the original paper:

```
@inproceedings{Monajjemi2011grSimR,
  title={grSim - RoboCup Small Size Robot Soccer Simulator},
  author={Valiallah Monajjemi and A. Koochakzadeh and S. S. Ghidary},
  booktitle={RoboCup},
  year={2011}
}
```

If you wish to cite this repo with it's modifications specifically, please cite:

```
@misc{firasim2019,
  author = {Rahimi, Mohammad Mahdi},
  title = {FIRASIM},
  year = {2019},
  publisher = {GitHub},
  note = {GitHub repository},
  howpublished = {\url{https://github.com/fira-simurosot/FIRASim/}}
}
```
