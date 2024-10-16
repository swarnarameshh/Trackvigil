# TrackVigil: Railway Track Maintenance and Inspection using YOLOv5 🚆🔍

# Trackvigil
Developed TrackVigil, an AI-powered railway track inspection system using YOLO v5 to detect 7 critical anomalies like bolt missing, track misalignment, and rail cracks. Leveraged transfer learning and achieved promising detection precision to enhance safety and efficiency in track maintenance.

# Project Overview
This project focuses on building an automated railway track anomaly detection system using YOLOv5. It aims to detect seven critical types of faults or anomalies that could pose significant risks if left unaddressed.

Railway inspections are traditionally performed manually, making them time-consuming, expensive, and often subject to human error. This project leverages deep learning and object detection to enhance the speed, accuracy, and safety of railway inspections.

# Anomalies Detected
The model is trained to detect the following seven anomalies:
- Bolthole Crack: Cracks around bolt holes, potentially leading to bolt failure or track misalignment.
- Bolt Missing: Absence of bolts, compromising the integrity of the rail fastening system.
- Rail Corrugation: Wavy patterns on the rail surface, leading to noise, vibration, and potential long-term damage.
- Fastener Missing: Missing fasteners, which can weaken the rail's connection to sleepers and increase the risk of derailment.
- Track Misalignment: Irregularities in track alignment that could lead to dangerous operational conditions.
- Rail Crack: Cracks in the rail itself, posing a major threat to the structural integrity of the railway.
- Vegetation Encroachment: Overgrown vegetation that can obstruct the track and hinder the safety of railway operations.
- 
# Why YOLOv5?
YOLOv5 (You Only Look Once version 5) is a state-of-the-art object detection model designed for high performance in both speed and accuracy. Here’s why YOLOv5 was chosen for this project:
Backbone: YOLOv5 uses CSPDarkNet, a backbone known for excellent feature extraction and multi-scale object detection, making it ideal for detecting both small and large anomalies.
Speed: YOLOv5 offers a fast inference speed, which is crucial for real-time or near-real-time railway inspection applications.
Accuracy: The model performs well even with a small dataset, thanks to its advanced feature extraction and deep learning architecture.

# Dataset Collection
The dataset used for this project was collected from various sources like Google and Kaggle, and it consists of 120 training images and 35 validation images. The dataset includes labeled images that correspond to the seven different anomalies detected by the model.


# Transfer Learning Approach
To improve model performance on our custom dataset, transfer learning was utilized:
The model was fine-tuned from a YOLOv5 model pre-trained on the MS COCO dataset.
Sublime Text was used to modify the .yaml configuration file, setting up the dataset paths and defining the seven classes of anomalies.

# Evaluation Metrics
Our model performed exceptionally well for certain fault types and showed overall positive trends:
- High Confidence Precision: Achieving 71% precision at high confidence levels for anomalies like vegetation encroachment.
- Bolt Missing: Detected with 86% accuracy, ensuring critical safety issues are flagged promptly.
- Background Detection: A perfect score of 1.00 in identifying non-anomalous sections, reducing false positives.

# Conclusion
This project marks a significant step toward automating railway track inspections using deep learning. The model’s ability to detect critical anomalies like missing bolts, track misalignment, and rail cracks can help prevent accidents, reduce downtime, and enhance maintenance efficiency.
