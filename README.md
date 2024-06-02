# Video-Special-Effects

## Introduction
This project, implemented in C++ using the OpenCV library, focuses on video input manipulation to create various visual effects. The project involves recording live video, applying greyscale transformations, implementing filters like sepia tone and blur, and performing edge detection and face recognition in a video stream.

## Tasks
### Task 1: Image Display and Manipulation
Implemented a program (imgDisplay.cpp) to:

Enter a loop, checking for keypresses.
Quit on 'q'.
Save the image on 's'.
Rotate the image clockwise on 'r'.
Rotate the image anti-clockwise on 'l'.

### Task 2: Video Display
Implemented a program (vidDisplay.cpp) to:

Open a video channel, create a window, and display frames in a loop.
Quit on 'q'.
Save the video on 's'.

### Task 3: Greyscale Video Stream
Converted the live video stream to greyscale using OpenCV's cvtColor function. The conversion formula is:
𝑌 = 0.299⋅𝑅 + 0.587⋅𝐺 + 0.114⋅𝐵

### Task 4: Alternative Greyscale
Added an alternative greyscale effect focusing on the red channel. This method inverts the red channel values.

### Task 5: Sepia Filter
Applied a sepia filter to the video stream. The new blue value is calculated as:
0.272⋅𝑅 + 0.534⋅𝐺 + 0.131⋅𝐵

### Task 6: Blur Filter
Task 6(a)
Implemented a basic 5x5 blur filter from scratch.

Task 6(b)
Optimized the blur filter using separable 1x5 filters for better performance.

### Task 7: Sobel Filters
Implemented Sobel X and Y filters for edge detection in the video stream, triggered by pressing 'x' and 'y' respectively.

### Task 8: Gradient Magnitude
Calculated the gradient magnitude from the Sobel X and Y images, triggered by pressing 'm'.

### Task 9: Blur and Quantize
Blurred and quantized the video stream, reducing the intensity levels, triggered by pressing 'l'.

### Task 10: Face Detection
Linked faceDetect.cpp to vidDisplay.cpp to perform face detection when the 'f' key is pressed.

### Task 11: Custom Filters
Implemented three custom filters:

Embossing Filter: Adds depth and texture by emphasizing gradients.
Halo Filter: Adds sparkles around detected faces.
Adjust Brightness and Contrast: Adjusts the brightness and contrast of the video stream.
Extension: Vignette Filter
Added a vignette effect, creating a darkening effect towards the edges of the video stream.
Extension: Image Captions
Enabled adding captions to video frames, which can be saved with annotations by toggling caption mode with the 'j' key and saving with the 's' key.

