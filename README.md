# Progressive & Bifocal segment height estimation using OpenCV

### Calculating progressive and bifocal segment height of eyeglass in cm using card on forehead

By : [Tanishq Selot](https://github.com/tanishq150802)

## Requirements
* Python 3.10
* Numpy
* dlib
* OpenCV

All the code is contained within **Segment_height_estimation.ipynb**. Image examples are attached.

### Steps

* The card on forehead is detected using HSV and Adaptive thresholding.
* Rifining the card dimensions using thresholding for more accurate results.
* Canny edge filter is used for eyeglass edge detection.
* 41st and 47th facial attributes amongst the 68 given by dlib relate to pupil edge.
* The segment height is calculated in terms of pixels using Euclidean distance.
* The width of a credit card is 8.56 cm.
* This data along with scaling formula is used to calculate the segment in cm.

### Example

Normal Image             |  Progressive Segment height |  Bifocal Segment height
:-------------------------:|:-------------------------: |:-------------------------:
![img](https://user-images.githubusercontent.com/81608921/226201290-4ec6bb73-d5eb-49dd-b175-d453a2783569.jpeg) |  ![line](https://user-images.githubusercontent.com/81608921/226201959-3adab96a-db65-49a3-81c2-385ba0030ef4.jpg) |  ![bifocal](https://user-images.githubusercontent.com/81608921/226202360-7e5f685a-f911-4a01-a5a8-db9d4fc9a8dd.jpg)
### References
* [68 facial attributes using dlib](https://medium.com/mlearning-ai/glasses-detection-opencv-dlib-bf4cd50856da)
* [Scaling formula](https://www.youtube.com/watch?v=ghU6T4h-C74)
