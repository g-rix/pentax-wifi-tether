# pentax-wifi-tether

Using 'pentax-wifi-tether' connect to your Wi-Fi-capable PENTAX camera and download your date-sorted images.

![window](https://raw.githubusercontent.com/maruncz/pentax-wifi-tether/f72bdbf75eeb573afee6651c8abd5bdcae8507f9/window.png)

## Qtcreator Build Instructions

Download the opensource edition of Qt5 here https://www.qt.io/download and install Qt5.12.2 or newer and Qtcreator.

    Open `tether.pro` file in Qtcreator and build

## Console Build Instructions

    1) Install Qt package dependencies:
           sudo apt-get install qt5-default qt5-qmake libqt5multimedia5-plugins qtmultimedia5-dev
    
    2) Clone the repo:
          git clone https://github.com/maruncz/pentax-wifi-tether.git
       
    3) Change to that directory:
          cd pentax-wifi-tether
    
    4) Configure the project:
          qmake tether.pro CONFIG+=release
    
    5) Build:
         make -j 2
         
    6) Run:
        ./tether

## How
  1) Enable Wi-Fi on your laptop and camera.
  2) Connect your laptop to the camera's WiFi-AP. (See the camera's menus from credentials.)
  3) Start the tether application, followed by the 'Connect' button
  4) Press 'Start', when download has completed, press 'Stop'.

## Supported Pentax Cameras
  1) K70
  2) K3 III

## Notes
  Tested with Ubuntu 20.04 and a Pentax K3 III.
  Ubuntu build-essentials also needed.
  May also work for the Pentax KS-2, KP, K1 and K1 II.
