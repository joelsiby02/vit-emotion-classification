# vit-emotion-classification
Explore the power of model building with ViT (Vision Transformer) and build a professional-quality application for real-time emotion recognition. This repository includes the code for the real-time emotion recognition application and instructions for customizing the emotions and the model used.



# Real-time Emotion Recognition using ViT (Vision Transformer)

This project uses the ViT (Vision Transformer) model from the transformers library to perform real-time emotion recognition on a video stream captured by the device's camera.

## Getting Started

### Prerequisites

Before running this project, you'll need to install the following dependencies:

- pandas
- numpy
- torch
- torchvision
- opencv-python
- pillow
- transformers

You can install these dependencies using pip:

```
pip install pandas numpy torch torchvision opencv-python pillow transformers
```

### Running the Project

To run the project, simply run the `video_camera.py` file:

```
python video_camera.py
```

This will start the video stream from the device's camera and display the video frames with the predicted emotion in real-time.

### Customizing the Emotions

You can customize the emotions that the model recognizes by modifying the `emotions` list in the `video_camera.py` file:

```
emotions = ["Angry", "Disgust", "Fear", "Happy", "Neutral", "Sad", "Surprise"]
```

### Customizing the Model

You can customize the ViT model used by modifying the `model` variable in the `video_camera.py` file. For example, you can use a different pre-trained model or modify the number of labels:

```
model = ViTForImageClassification.from_pretrained('google/vit-base-patch16-224', num_labels=len(emotions), ignore_mismatched_sizes=True)
```

## Acknowledgments

This project was inspired by the ViT model and the transformers library. Special thanks to the developers of these projects for making this project possible.
