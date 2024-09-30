<div align="center">
  
[1]: https://github.com/Akshat1661
[2]: https://www.linkedin.com/in/akshat-desai-10bba1235/


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]

</div>


# <div align="center">Yolov8 Object Detection on Garbage Images</div>

## Table of Contents
1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Training the Model](#training-the-model)
4. [Testing the Model](#testing-the-model)
5. [Results](#results)
6. [Conclusion](#conclusion)
7. [References](#references)


Overview:
The goal of this project is to perform object detection on garbage images using YOLOv8, a state-of-the-art deep learning model. The input data for this project is the "Warp Waste Recycling Plant Dataset" from Kaggle, which contains over 10,000 images of various types of garbage items, including plastic bottles, cardboard boxes, and aluminum cans. The dataset also includes annotations for each image, identifying the location and type of each garbage item.

Object detection on garbage images has important applications in the field of waste management, as it can help automate the process of sorting and recycling different types of garbage items. Traditional methods of garbage sorting are often slow, labor-intensive, and prone to errors, leading to incorrect sorting and contamination of recyclable materials. By using object detection techniques like YOLOv8, we can potentially improve the accuracy and efficiency of garbage sorting and reduce the environmental impact of waste.

In this project, YOLOv8 was performed on resized images of 640x640 pixels.

This project demonstrates the application of YOLOv8 in a real-world problem and provides insights into how deep learning can be used to improve waste management and promote environmental sustainability.

## Dataset:

The dataset used for this project is sourced from Kaggle and includes:
- **Number of images**: Over 10,000
- **Classes**: 28 types of garbage items, including:
    - Various types of bottles (e.g., blue, green, transparent, yogurt, milk, oil)
    - Cans
    - Juice and milk cartons
    - Detergent containers (color, transparent, box)
    - Glass bottles (transparent, dark, green)


The dataset is split into training and validation sets:

Training data: 
```
/content/drive/MyDrive/Garbage_Detection/data/train/images/
```
Validation data: 
```
/content/drive/MyDrive/Garbage_Detection/data/val/images/
```
## Installation:
To run this project, follow these steps:

```
# Clone the repository
git clone https://github.com/your-username/garbage-detection-yolov8.git
cd garbage-detection-yolov8

# Install dependencies
pip install -r requirements.txt
```
Download the dataset from Kaggle and place it in the appropriate directories (/data/train/images/ and /data/val/images/).

## Training the Model
1. **Ensure your environment is set up with all the dependencies.**

2. **Run the following command to start training:**

    ```bash
    !yolo train model=yolov8n.pt data=dataset.yaml epochs=100 imgsz=640
    ```

    The model will be trained on resized images (640x640 pixels), with a focus on identifying the 28 classes of garbage items defined in the `dataset.yaml` file.

3. The model will be trained on resized images (640x640 pixels), with a focus on identifying the 28 classes of garbage items defined in the dataset.yaml file.

## Validation:
After the training process, validate the performance of the model using the validation dataset:
```
!yolo val model=runs/train/exp/weights/best.pt data=dataset.yaml
```
This will output the performance metrics of the model on unseen data, including precision, recall, and mean Average Precision (mAP).

## Testing
You can test the model on new images or unseen data using the following command:
```
!yolo detect model=runs/train/exp/weights/best.pt source=/path/to/your/test/images
```
Make sure to modify the source path to point to your test images.

## Results:

![Robo_25-Mar_15-47-34](https://github.com/user-attachments/assets/a6212128-0a26-4b57-acf3-fc3e67edae73)


## Contributing:
Contributions are welcome! If you'd like to improve the project or add new features, feel free to fork the repository and submit a pull request. Ensure your code follows the project's coding guidelines.

## License:
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact:
Feel free to reach out for any questions or collaborations:
<div align="center">
  
[1]: https://github.com/Akshat1661
[2]: https://www.linkedin.com/in/akshat-desai-10bba1235/


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]

</div>

akshat.desai.754@gmail.com


