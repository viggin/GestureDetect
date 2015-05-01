![recognition UI](recog_UI.jpg)

This project is aiming at detecting gestures and training user-defined gesture templates. The “gesture” here means a position OR a motion of the joints of body.

The function is provided in a package for **Unity3D** platform. It reads skeleton data from MS **Kinect** or similar motion capture devices. To acquire skeleton data, we uses **OpenNI** 1.5.4 because it is an open source library. You can change it to OpenNI 2.x or MS Kinect SDK. 

The algorithm of the program is a simple **template matching** one. It splits a gesture into several key postures. When these postures are detected successively, then the gesture event is triggered.

When training gesture templates, we use Unity3D to display a 3D avatar. If you do not want to use Unity3D, you can make use of the **c#** scripts in “GestureScripts” folder.