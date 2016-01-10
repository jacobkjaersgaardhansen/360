# View live 360 video stream on a smartphone
The aim of this project is to be able to watch a <b>live</b> 360 video stream on a smartphone. The project is inspired by the <b>recorded</b> 360 videos that lately have shown up on Facebook and Youtube (like http://youtu.be/7gjR60TSn8Q) and the general virtual reality hype (even though we ignore the "virtual" part in this project). Such videos give the viewer an immersive experience of being there himself by utilizing the built-in gyroscope and accelerometer (that most new smartphones have) to change the direction of view just by moving the smartphone in the space around him. This turns the smartphone into something that feels like a window into another world.

We want to achieve the same kind of "being-there" experience with live video. We acknowledge that real 3D 360 view takes a lot of computation power, but we have seen that 2D 360 live conference calls are possible in real time with commercial available equipment like the device seen on the table in center of this picture http://rack.1.mshcdn.com/media/ZgkyMDE0LzAyLzA0LzFlL3BvbHljb21yb29tLjE5MjE4LmpwZwpwCXRodW1iCTk1MHg1MzQjCmUJanBn/99230cc9/c2a/polycom-room-system.jpg. Therefore, we believe that a lightweight 2D solution is possible. 

We want to put a live video stream from such a device into a webpage and "navigate" around the stream by using dynamically cropping of the stream. I.e. say at every 50 ms the device orientation is measured locally and the video stream is cropped accordingly. The entire video stream is loaded to the smartphone contiunueolsy, but only part of it is shown. Thereby the viewer gets the desired experience of having a device in his hands that acts like a window through which he can experience another location in realtime.


To setup:

1. Install openCV (e.g. http://milq.github.io/install-opencv-ubuntu-debian/ or http://docs.opencv.org/master/d5/de5/tutorial_py_setup_in_windows.html)
2. Flask (http://blog.miguelgrinberg.com/post/video-streaming-with-flask)
3. Setup your local network (or use localtunnel.me) to browse the page from your phone
