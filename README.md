# noisestress

#Monitoring Noise in Decibels 

The app uses the microphone from user app and calculates the decibels accordingly. Using the amount of decibels calculated the app shows whether the noise is measurable or not.

The app starts with a minimum threshold decibels and it keep on recording the decibels in real time. The app firstly calls the mainActivity which starts the SoundMeter java class, which subscribes the decibel calculation and real time decibel value collection.
The app collects the decibels ,stores it in buffer and then transfer it to cloud.
The android application uses a gradle mechanism using which it connects to the IBM Watson IOT cloud using the apache edgent application and then stores the buffer on the cloud.


The application is run as per the following steps:
1) Clone and download both the repository given in following links:
  a) https://github.com/momo1901/sound-meter-poc-edgent.git
  b) https://github.com/momo1901/NoiseMonitor.git

2) In the edgent code, update the code with your IBM Watson IOT device setting and then load and run the program as the steps given over in that repository(The link have been uploaded).

3) Running or compiling the application next, would eventually call the gradle files and make the application running and hence the data could be able to be loaded on cloud.

I would also like to thank specially @LithiumSR for mainly creating and working on the edgent module, which helped me and my team to successfully complete this project on time.


The Reference links:
1) Sound Meter Edgent Code(https://github.com/momo1901/sound-meter-poc-edgent.git)
2) Apache (https://maven.apache.org/what-is-maven.html Edgent (http://edgent.apache.org/)
3) Java Maven (https://maven.apache.org/what-is-maven.html)
4) LithiumSR (https://github.com/LithiumSR)
