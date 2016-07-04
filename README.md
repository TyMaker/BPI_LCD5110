# BPI_LCD5110

BPI Banana Pi 驱动Nokia 5110 LCD

Overview
--------
 * 兼容Banana Pi M1/M2P/M3 Raspberry Pi A/B+/2B/ZERO

 * Makt 天宇科技  更多详情见[我的博客](http://makt.top "http://Makt.top")  



Connection
----------

	 LCD pins      Raspberry Pi / Banana Pi
	 LCD1 - GND    P06  - GND
	 LCD2 - VCC    P01 - 3.3V
	 LCD3 - CLK    P11 - GPIO0
	 LCD4 - Din    P12 - GPIO1
	 LCD5 - D/C    P13 - GPIO2
	 LCD6 - CS     P15 - GPIO3
	 LCD7 - RST    P16 - GPIO4
	 LCD8 - LED    P01 - 3.3V 


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
