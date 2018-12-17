![](https://i.imgur.com/eh1QMvS.jpg)

# ABSOLUTELY AMAZING THING: auTONomous Intelligent Car 

![wwwwowww](https://media.giphy.com/media/OK27wINdQS5YQ/giphy.gif)


I present to You, the autonomous car, almost entirely written in Python.

# Second Version*

![Second Version](https://lh3.googleusercontent.com/xZi2YtqGj9eyGwgN6Cv7f8IOTtTGhyF9R63gP46E6o_FYAIG0sE6KshoPQIdHI0yB0M_12FqhraWmgf5IVwChfGCR2R8_xB3VU9uThSF9Swo1kTQs50YQw0wuFENgqzi8uNtJzIkJLxglpeXTPdaTHxA_LHPb80bH_POSiPaGubV4qFAL0eRO4jUh0VOYhyAYfb7j2-ZfgoqDgAC3rcJ3TWbuNi-qLxAQKupFlW5ZhBKi_qju2IA98hOyAfwRD92LxWDya2be6XsyNzHlpJT-XeSdNu_LKqHBJZzExF3fIL10ag0dK9orViAvptESs7cL5s5owkRAvwpUKaaDm1F4QMnlOoFgy_4oQPYg4aeNTdIakgZdmuUQfz2G_dRnHjbeNHXEoDy4z5yWqFr_M2v0PPmH87NnbOYrEjge-KF7mY1HNYH8oGjzq5pnKOrO7UAB0LrGO7smxilqWQ2T3-dK-V-ppEujbIzZRjaw02xdh94a-Pj9x0Q0iKmAUXI370z01C_racZTcPeCKxjOabj1A8OgADNkjUt1_UHfw-kYKIC4roeObC4l-dr3D-8ymsQc9FuoLTXJAgi5Vhq193Wyel-LUcL44efAl4PglNH6oVdimggdyzmqH-57Al1r8WmkB7a9NM4V1o2uDVj38rdWyZFSQ=w1791-h1007-no)

(*First one totally not worth showing xD)

## Hardware MARK2:
- RC Range Rover Car [like this one](http://allegro.pl/range-rover-evoque-sterowany-rastar-1-24-full-r-c-i5741237813.html)
- [Raspberry Pi Zero](https://botland.com.pl/moduly-i-zestawy-raspberry-pi-zero/8330-raspberry-pi-zero-w-512mb-ram-1ghz-wifi-bt-41.html?search_query=raspberry+pi+zero&results=30) 
- [Pololu MinIMU-9 v5](https://botland.com.pl/czujniki-9dof-imu/5528-pololu-minimu-9-v5-9dof-akcelerometr-zyroskop-i-magnetometr-i2c.html)
- [Pi Camera](https://botland.com.pl/kamery-do-raspberry-pi-32b/5619-camera-hd-c-kamera-dla-raspberry-pi-zgodna-z-wersja-oryginalna.html?search_query=pi+kamera&results=236) with connecting tape
- [Pakiet Li-Pol Redox 900mAh 20C 3S 11,1V](https://botland.com.pl/akumulatory-li-pol-3s-111v-/8320-pakiet-li-pol-redox-900mah-20c-3s-111v.html)
- [L298 -](https://botland.com.pl/sterowniki-silnikow-moduly/3164-l298-dwukanalowy-sterownik-silnikow-modul.html)

Second version on video

[![Druga działająca wersja (wideo)](https://img.youtube.com/vi/XM7lNRdp8ow/0.jpg)](https://www.youtube.com/watch?v=XM7lNRdp8ow)
 

## How does it work:

The software is communicating with Raspberry Pi via WiFi network, using sockets. Sensors, camera, and steering - each one is implemented
as a separate service on socket.
You can steer it with keyboard on PC, and have an live feed from camera.
All of the sensors, stearing and video can be dumped to files on PC.
All written in Python.

## The Goal
To implement a SLAM capability, that would enable the car to map the environemnt and navigate.

## Achievements of the first version.
  - Working camera feeed
  - Working steering system
  - Working IMU
  - Partian SLAM implemented
  - Using only the feed from camera, it can map the environment to "birds eye view"
  
  **Attention! This is cool!** ORB-slam working on the camera deed:
  
  [![Second version (video)](https://img.youtube.com/vi/XR-vKycwOm8/0.jpg)](https://www.youtube.com/watch?v=XR-vKycwOm8)
  
  **C A R E F U L! This is cool as well** 2D map from the video feed:
  
  [![Second version (video)](https://img.youtube.com/vi/Wd5jEd4hx6U/0.jpg)](https://www.youtube.com/watch?v=Wd5jEd4hx6U)
  
  
  
# The third version


![Third version, less spectacular](https://lh3.googleusercontent.com/IuCSr21Cb3tGpGMnIhsa7TThIg2WQow34TMnW2t3mI2jwENIGsg7YI2H-PUxN7tL1rPp5GF8OytFAX5TnJt4F91LoR5jvWLSZfbNOt-bqljZWx_-JIScLlvS8kxXzLI2Gl5FW_V-4n8G2psZsI2k11mGIHGzmENbIgd1157-BmnFWVcFHjPWYQiKbv_6vLWFJmYBeK4ICtQrbBSLLpSVLlJoUGQLrAGPiltxqREM2potxoTvzC1uk4joj2DezeMMhbXHsouxb-veooV5JQUoD2KNKSOuwWNTJy7wCSLCP7bKnq5WOK7klRYwIx4nhzVjPGsIMBqVnM15oarJQVdWVM-cJr0SAhowkN2LHgan0iTv56c5mLPj6WO0Rhsg6H6f9YSMKIieSHfKuPdo44S4-Foa54bNrneKJ7gbCveb5hEwNuFyEbp-QbFYruM3aJ-113DGR29Fb0GkyQczrmi7Nr5teJlE_0DOf8V22BuAhgfWqvsuHxakuo4GFyOPKOLtgclmE0enZLRjDV5R5vBZ2DtZIwuDwUgBv_kpZTwIVqcrZFJ-hiMxG4rVD-6fxH_p4hclV3qyV7BUZyOnHyXiyLOh1Liglgfismk5ZBtzackYbYXSuWPvHRvD7tSXbFObZ4aH4Z-vawgQeaY8QT4tLKXImYnEGanmDq3ttEevNlh40Gf4aWk5v7IVdFno2qg9EiqIc1KLZSdT38J3fMY=w1433-h806-no)

Third version was created because of the problems with the steering (cheap remote controled cars have low quality gears inside). 
Also, in the previous version, any manipulation of the circuits, was difficult because of the casing. 
Also it was difficult to get good odometry readout. 

So i changed the body of the car as well as the wheels. 
Looks a bit worse, but is waaaaay more effective ;]

**Third version has working odometry system**

## What can be improved:

![](https://rlv.zcache.com/uncle_sam_i_want_you_poster-rad708dab64b04b6e8f41bb6beece2194_q1kv_8byvr_540.jpg)

If you would like to help, or have questions regarding the project, see ![here](https://github.com/mmajewsk/Tonic/issues).



# Setting up

- Follow the hardware guide (❌ Not created yet)
- Follow the device setup guide (❌ Not created yet)
- Create orb slam docker, using [this repo](https://github.com/mmajewsk/orb_slam_py2_docker/)  (✔️)
- Follow the software setup guide (❌ Not created yet)