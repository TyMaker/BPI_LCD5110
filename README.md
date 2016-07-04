# BPI_LCD5110

BPI Banana Pi 驱动Nokia 5110 LCD

Overview
--------
 * 兼容Banana Pi M1/M2P/M3 Raspberry Pi A/B+/2B/ZERO

 * Makt 天宇科技  更多详情见[我的博客](http://makt.top "http://Makt.top")  


User
----------
Download & Install WiringPi :

		### For BPI-M1 / M1Plus
		    git clone https://github.com/BPI-SINOVOIP/BPI-WiringPi.git -b BPI_M1_M1Plus
		    
		### For BPI-M2
		    git clone https://github.com/BPI-SINOVOIP/BPI-WiringPi.git -b BPI_M2
		    
		### For BPI-M3
		    git clone https://github.com/BPI-SINOVOIP/BPI-WiringPi.git -b BPI_M3    
		    
		## Installation
		    cd BPI-WiringPi
		    chmod +x ./build
		    sudo ./build

Download Code

        git clone https://github.com/TyMaker/BPI_LCD5110
        cd BPI_LCD5110/
        cc -o cpushow pcd8544_rpi.c PCD8544.c  -L/usr/local/lib -lwiringPi
        sudo ./cpushow
