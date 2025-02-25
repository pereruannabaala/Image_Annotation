# Open In Colab: OpenCV Drawing Basics
This project demonstrates fundamental OpenCV drawing operations in Python, including downloading assets, reading images, and drawing basic shapes such as lines, circles, rectangles, and text annotations.

## Requirements
To run this project, ensure you have the following dependencies installed:
- Python 3.x
- OpenCV (cv2)
- NumPy (numpy)
- Matplotlib (matplotlib)

## Running the Notebook in Google Colab
1. Open the Colab notebook by clicking the "Open in Colab" button.
2. Run all cells to download assets and execute the OpenCV drawing functions.

## Descriptions
The script performs the following actions:
1. Imports necessary libraries:
- ``os``: For operating system related functionalities.
- ``cv2``: OpenCV for image processing.
- ``matplotlib``: For plotting images.
- ``numpy``: For numerical operations.
- ``zipfile``: To extract zip archives.
- ``urllib.request``: To download files from URLs
2. Downloads and extracts assets:
- A function ``download_and_unzip`` is defined to download a zip file from a given URL and extract its contents.
- The script downloads a zip file containing an image ("Apollo_11_Launch.jpg") from a Dropbox URL and extracts it into the current directory.
3. Loads and displays the image:
- The image "Apollo_11_Launch.jpg" is loaded using ``cv2.imread``.
- The image is displayed using ``matplotlib.pyplot.imshow``. Note that OpenCV uses BGR color format, so the image is converted to RGB using ``[:, :, ::-1]`` before displaying.
4. Draws a line:
- A copy of the original image is created.
- ``cv2.line`` is used to draw a yellow line on the image.
- The modified image is displayed.
5. Draws a circle:
- A copy of the original image is created.
- ``cv2.circle`` is used to draw a red circle on the image.
- The modified image is displayed.
6. Draws a rectangle:
- A copy of the original image is created.
- ``cv2.rectangle`` is used to draw a magenta rectangle on the image.
- The modified image is displayed.
7. Adds text:
- A copy of the original image is created.
- ``cv2.putText`` is used to add text to the image.
- The modified image is displayed.

## Code Explanation
- ``cv2.line(img, pt1, pt2, color[, thickness[, lineType[, shift]]])``: Draws a line between two points.
- ``cv2.circle(img, center, radius, color[, thickness[, lineType[, shift]]])``: Draws a circle.
- ``cv2.rectangle(img, pt1, pt2, color[, thickness[, lineType[, shift]]])``: Draws a rectangle.
- ``cv2.putText(img, text, org, fontFace, fontScale, color[, thickness[, lineType[, bottomLeftOrigin]]])``: Adds text to an image.
- ``plt.imshow(image[:, :, ::-1])``: Displays an image using Matplotlib, converting it from BGR to RGB.

## Conclusion
This project demonstrates how to download image assets and perform basic drawing operations using OpenCV. Modify the coordinates, colors, and text to explore different effects.

Happy coding!
