From https://www.waveshare.com/wiki/SGP40_VOC_Sensor

Install BCM2835
   wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.60.tar.gz
   tar zxvf bcm2835-1.60.tar.gz 
   cd bcm2835-1.60/
   sudo ./configure
   sudo make
   sudo make check
   sudo make install
   
Install WiringPi
   sudo apt-get install wiringpi
   cd /tmp
   wget https://project-downloads.drogon.net/wiringpi-latest.deb
   sudo dpkg -i wiringpi-latest.deb
   gpio -v
   
Waveshare Demo Code
   sudo apt-get install p7zip-full
   wget https://www.waveshare.com/w/upload/6/62/SGP40_Voc_Sensor_code.7z
   7z x SGP40_Voc_Sensor_code.7z -r -o./SGP40_Voc_Sensor_code
   sudo chmod 777 -R  SGP40_Voc_Sensor_code
   
Run Waveshare Demo Code
   cd
   cd SGP40_Voc_Sensor_code/RPI
   sudo python SGP40.py