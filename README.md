# pentax-wifi-tether
Automatically downloads files from Pentax cameras via wifi and sorts them by date.

Useful when you work in studio and you want to see your pictures immediately, without removing your SD card.

![window](https://raw.githubusercontent.com/maruncz/pentax-wifi-tether/f72bdbf75eeb573afee6651c8abd5bdcae8507f9/window.png)

## Build Instructions

Download the opensource edition of Qt5 here https://www.qt.io/download and install Qt5.12.2 or newer and Qtcreator.

Open `tether.pro` file in Qtcreator and build

  or 

On the console:

    1) Install required Qt packages:
           sudo apt-get install qt5-default qt5-qmake libqt5multimedia5-plugins qtmultimedia5-dev
    
    2) Clone the repo:
          git clone https://github.com/maruncz/pentax-wifi-tether.git
       
    3) Change into checked out directory:
          cd pentax-wifi-tether
    
    4) Configure the project:
          qmake tether.pro CONFIG+=release
    
    5) Build it:
         make -j 2

    6) Run it:
        ./tether


Note: 
  This was tested on Ubuntu 20.04 and you will also need build-essentials etc.
  
