# Digital Image Processing Assignment

This assignment implements a collection of fundamental **Digital Image Processing** tasks using **Python in Google Colab**. The implementations use common Python image-processing libraries such as **OpenCV, PIL, NumPy, and Matplotlib**.

## Google Colab Notebook

All implementations, experiments, visualizations, and results are available in the following Google Colab notebook:

**Colab Notebook:**
https://colab.research.google.com/drive/1mFMoRCCUJ8jQ1o_oIK5xs7QGbSxnPbNV?usp=sharing

---

## Implemented Tasks

### 1. Reading, Displaying, and Inspecting a Digital Image

* Read and display both grayscale and color images.
* Determine image width and height.
* Identify the number of color channels.
* Display the image data type.
* Compare the properties of grayscale and color images.

### 2. Converting a Color Image to Grayscale

* Load an RGB/color image.
* Convert the color image into grayscale.
* Display the original and grayscale images side by side.
* Compare the number of channels and data size before and after conversion.

### 3. Classifying an Unknown Image

* Accept an image as input.
* Automatically classify it as:

  * Binary image
  * Grayscale image
  * Full-color image
* Provide the reasoning behind the classification based on image channels and pixel values.

### 4. Surveying Imaging Modalities

Five different imaging modalities are demonstrated:

* X-ray imaging
* Satellite/remote-sensing imaging
* Microscopy imaging
* Ultrasound imaging
* Infrared imaging

Each image is displayed with its modality and a real-world application.

### 5. Thresholding a Grayscale Image into Binary

* Read an 8-bit grayscale image.
* Apply different threshold values.
* Convert pixels above or equal to the threshold to white (255).
* Convert pixels below the threshold to black (0).
* Compare the results for multiple threshold values.

### 6. Observing the Checkerboard Effect — Spatial Resolution

* Reduce a grayscale image to:

  * 128 × 128
  * 64 × 64
  * 32 × 32
  * 16 × 16
* Keep the intensity resolution fixed at 8 bits.
* Display and compare the resulting images.
* Observe the blocky/checkerboard effect caused by reduced spatial resolution.

### 7. Observing False Contouring — Intensity Resolution

* Reduce an image from 256 gray levels to:

  * 128
  * 64
  * 32
  * 16
  * 8
  * 4
  * 2
* Keep the spatial resolution unchanged.
* Observe the appearance of false contours or banding in smoothly shaded regions.

### 8. Comparing Image Interpolation Methods

A small image is enlarged using three interpolation methods:

* Nearest-neighbor interpolation
* Bilinear interpolation
* Bicubic interpolation

The enlarged images are displayed side by side to compare blockiness and smoothness.

### 9. Computing and Interpreting an Image Histogram

* Calculate the histogram of a grayscale image.
* Plot the number of pixels for each intensity level from 0 to 255.
* Test the program using:

  * Dark image
  * Bright image
  * Low-contrast image
* Compare the histogram with the visual appearance of each image.

### 10. Finding Pixel Neighbors

A function is implemented to determine:

* 4-neighbors, N₄(p)
* Diagonal neighbors, Nᴅ(p)
* 8-neighbors, N₈(p)

The function is tested for:

* A middle pixel
* An edge pixel
* A corner pixel

Border conditions are handled so that nonexistent neighbors are excluded.

### 11. Computing Distance Measures Between Pixels

The following distance measures are calculated between two pixel coordinates:

* Euclidean distance
* City-block distance (D₄)
* Chessboard distance (D₈)

The results are verified using manually calculated test cases.

### 12. Image Arithmetic and Change Detection

Pixel-by-pixel image arithmetic operations are implemented:

* Addition
* Subtraction
* Multiplication
* Division

Image subtraction is also used for **change detection** between two nearly identical images to highlight regions that have changed.

### 13. Noise Reduction by Image Averaging

* Generate 20 noisy copies of a clean image using random Gaussian noise.
* Average the noisy images pixel by pixel.
* Display an individual noisy image and the final averaged image.
* Demonstrate how averaging reduces random noise.

### 14. Set and Logical Operations on Binary Images

Two binary images containing simple shapes are created and the following operations are performed:

* AND
* OR
* NOT
* XOR

The resulting images are displayed and interpreted based on the original shapes.

### 15. Basic Geometric Transformations

The following transformations are applied individually to an input image:

* Translation
* Rotation
* Scaling

The original and transformed images are displayed together. Empty/black regions created during transformations are also observed.

---

## Technologies and Libraries

The assignment is implemented using **Python** in **Google Colab** with libraries including:

* NumPy
* OpenCV
* PIL/Pillow
* Matplotlib

## Conclusion

This assignment demonstrates several fundamental concepts of digital image processing, including image representation, spatial and intensity resolution, thresholding, histograms, interpolation, neighborhood relationships, distance measures, image arithmetic, noise reduction, logical operations, and geometric transformations.

All source code, outputs, visualizations, and experiments are available in the Google Colab notebook linked above.
