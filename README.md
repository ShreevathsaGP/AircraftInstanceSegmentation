# Aircraft Instance Segmentation

| Original Image | Segmentation Result |
|----------------|---------------------|
| ![input_image_1](https://github.com/user-attachments/assets/21b8dafa-4883-436e-9ff0-6f9a226670da) | ![output_image_1](https://github.com/user-attachments/assets/a88cc8b2-e29b-483c-9a45-c2d054d1ed73) |
| ![input_image_0](https://github.com/user-attachments/assets/e27e84d5-6c3a-4002-9d15-0f18a9140d11) | ![output_image_0](https://github.com/user-attachments/assets/1c16b8fd-0cd1-4567-840b-5712f5c331ff) |

## Overview
This project performs instance segmentation of aircraft in images using OpenCV, YOLO v8 and TensorFlow. The goal is to detect and segment individual aircrafts within various images accurately.

## Technologies Used
- **OpenCV**: Image processing and manipulation.

- **YOLO v8**: Object detection and segmentation.

- **TensorFlow**: Training and optimization.

- **Ultralytics**: Access to YOLO v8 model.

## Installation

To set up the project on your local machine, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/aircraft-instance-segmentation.git
   
   cd aircraft-instance-segmentation
   ```

2. **Create and activate a virtual environment:**

   ```bash
   python3 -m venv venv
   
   source venv/bin/activate
   ```

3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Dataset

The dataset used in this project is sourced from the Open Images Dataset V7, specifically focusing on images containing aircraft.

## Results

Sample results of the segmentation model on aircraft images are shown in the table at the top. The segmentation results highlight the detected aircrafts and their segmented areas.

## Future Work

### Potential Improvements

1. **Enhanced Segmentation**:

   - Use YOLO v8 only for object detection.

   - Use Meta's Segment Anything Model (SAM) to segment the individual bounding boxes obtained through object detection

   - This approach would yield more accurate segmentation results but at the cost of increased computational complexity and slightly slower inference times.

2. **Building a frontend**:
	- Build a web frontend that allowed you to upload a number of images.

	- Segmentation is performed automatically and results are displayed in user-friendly manner.
	
	- The aim is to make the algorithm accessible without having to write code and or run Jupyter Notebooks.

## References

- [Tutorial: Image segmentation on custom dataset using YOLOv8]([https://example.com](https://www.youtube.com/watch?v=aVKGjzAUHz0))
