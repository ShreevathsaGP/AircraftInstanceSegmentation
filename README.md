# Aircraft Instance Segmentation

| Original Image | Segmentation Result |
|----------------|---------------------|
| ![input_image_1](https://github.com/user-attachments/assets/21b8dafa-4883-436e-9ff0-6f9a226670da) | ![output_image_1](https://github.com/user-attachments/assets/a88cc8b2-e29b-483c-9a45-c2d054d1ed73) |
| ![input_image_2](https://github.com/user-attachments/assets/9e2706c1-db03-4372-af5b-2cd47333fb5a) | ![output_image_2](https://github.com/user-attachments/assets/17e8055a-af15-4337-8149-c52fbe95a9e7) |
| ![input_image_0](https://github.com/user-attachments/assets/e27e84d5-6c3a-4002-9d15-0f18a9140d11) | ![output_image_0](https://github.com/user-attachments/assets/8c7697bc-07de-472c-9694-311ea5c711f9) |


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

The dataset used in this project is sourced from the [Open Images Dataset V7](https://storage.googleapis.com/openimages/web/index.html), specifically focusing on images containing aircraft.

## Results

Sample results of the segmentation model on aircraft images are shown in the table at the top. The segmentation results highlight the detected aircrafts and their segmented areas.

## Potential Improvements

1. **Enhanced Segmentation by Decoupling Object Detection and Segmentation**:

   - Use YOLO v8 for object detection.

   - Apply Meta's Segment Anything Model (SAM) to segment the individual bounding boxes obtained from YOLO v8.

   - This approach can provide more accurate segmentation results, albeit with increased computational complexity and slightly slower inference times.

3. **Build a frontend**:
   - Develop a web frontend that allows users to upload multiple images.

   - Perform segmentation automatically and display the results in a user-friendly manner.

   - Allow the frontend to accept user feedback and corrections on segmentation results.

   - Use the corrected segmentation as training data to improve the model's accuracy over time.

   - This makes the algorithm accessible without requiring users to write code or use Jupyter Notebooks.

## References

- [Tutorial: Image segmentation on custom dataset using YOLOv8](https://www.youtube.com/watch?v=aVKGjzAUHz0)
