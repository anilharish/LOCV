-------------------------------------Updates from the main code------------------------------------
--------------------------------------------ANIL HARISH--------------------------------------------

1. Replaced "CV_LOAD_IMAGE_COLOR" with "cv::IMREAD_COLOR" for OpenCV 3.0 or higher.
2. OpenCV runtime error: "libopencv_core.so.4.0: cannot open shared object file: No such file or directory" in Ubuntu 18.04 LTS can be solved by:

   (i) $ sudo find / -name "libopencv_core.so.4.0*"
   (ii) It displays the directory the file is stored under in my case the result was: usr/local/lib/libopencv_core.so.4.0
   (iii) Create a file called opencv.conf in /etc/ld.so.conf.d/opencv.conf and edit the contents of the file by writing the path obtained previously.
   (iv) In my case: usr/local/lib to my opencv.conf file
   (v) Re-run the executable again.

------------------------------------TO COMPILE THE PROGRAM-----------------------------------------

3. Using G++ compiler: g++ -std=c++11 removeRedEyed.cpp -o removeRedEyes `pkg-config --libs --cflags opencv`
4. Run ./removeRedEyes
5. To change the name of the .jpg file used chage the name in Read Image section of the Code in Line 33 of the program.
