# Real-time-Road-Conditioning-Model
Real-time Road Conditioning Model
A real-time deep learning-based system for detecting road anomalies such as potholes, cracks, and debris using YOLOv8. The system is designed to enhance road safety, improve maintenance planning, and integrate with smart traffic systems.

📌 Features
Real-time detection of potholes and cracks.

Powered by YOLOv8 for fast and accurate object detection.

Uses OpenCV for video feed processing.

Model training with hyperparameter tuning for optimal accuracy.

Can be integrated with road safety applications and autonomous vehicles.

Tested on multiple datasets with varying road conditions.

🗂 Dataset Sources
Kaggle: Road Surface Type Classification

Mendeley Data

GitHub - Road Damage Detector

Roboflow Dataset for Pothole Detection

⚙️ Installation & Usage
Prerequisites
Python 3.8+

ultralytics

torch

opencv-python

numpy

pandas

matplotlib

seaborn

bash
Copy
Edit
pip install ultralytics opencv-python torch numpy pandas matplotlib seaborn
Running the Model
Clone the repository and navigate to the project folder.

Train or use pre-trained YOLOv8 weights.

Run the real-time detection:

bash
Copy
Edit
python detect.py --weights yolov8_custom.pt --source 0
For video file input:

bash
Copy
Edit
python detect.py --weights yolov8_custom.pt --source input_video.mp4
🖼️ Methodology
Data Preparation

Collected diverse road images and annotated using LabelImg in YOLO format.

Model Training

Custom YOLOv8 training on the prepared dataset.

Fine-tuned with hyperparameter adjustments for optimal Mean Average Precision (mAP).

Real-time Inference

Capturing frames via OpenCV.

Real-time visualization of bounding boxes on road damage detections.

Data logging for future analysis.

📊 Results
Mean Average Precision (mAP@0.5:0.95): Achieved >0.5 on test datasets.

Real-time detection capability with minimal latency.

Limitation: Slightly reduced accuracy under extreme weather (e.g., heavy rain/fog).

🔮 Future Scope
Enhance robustness under varied environmental conditions.

Expand detection to other anomalies (e.g., waterlogging, surface deformations).

Integration with GPS for geo-tagging road defects.

Development of an interactive dashboard for visualization and reporting.

🧑‍💻 Authors
Poorna Singh

Namrata Todkar

Samradny Ware

Guided by Dr. Sameer Sayyad
Symbiosis Institute of Technology (SIT), Pune
Academic Year 2022-26

📚 References
YOLOv8 Documentation

DebuggerCafe: Frame Differencing with OpenCV

Multiple research publications listed in the project report.


