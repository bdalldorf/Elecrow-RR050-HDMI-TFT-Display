### Elecrow RR050 HDMI 5 Inch 800x480 TFT Display for Raspberry Pi B+/2B/3BE

[Product Website](https://www.elecrow.com/hdmi-5-inch-800x480-tft-display-for-raspberry-pi-b-p-1384.html)



#### Device
* Raspberry Pi 3 Model B+
* OS: Raspbian



#### [Config File](https://github.com/bdalldorf/Elecrow-RR050-HDMI-TFT-Display/blob/master/config.txt)
* Note: This disabled the keyboard and mouse to enable the touchscreen.
~~~
# Elecrow RR050 HDMI 5 Inch 800x480 TFT Display for Raspberry Pi B+/2B/3B
# --- added by elecrow-pitft-setup ---
hdmi_force_hotplug=1
max_usb_current=1
hdmi_drive=1
hdmi_group=2
hdmi_mode=1
hdmi_mode=87
hdmi_cvt 800 480 6 0 0 0
dtoverlay_ads7846,cs=1,penirq=25,penirq_pull=2,speed=50000,keep_vref_on=0,swapxy=0,pmax=255,xohms=150,xmin=200,xmax=3900,ymin=200,ymax=3900,display_rotate=0
# --- end elecrow-pitft-setup ---
~~~



#### Install Driver On Raspbian
~~~
Download the ZIP package and extract the files
https://github.com/goodtft/LCD-show

Go to the extracted directory and run the command:
sudo ./LCD5-show-master
~~~
