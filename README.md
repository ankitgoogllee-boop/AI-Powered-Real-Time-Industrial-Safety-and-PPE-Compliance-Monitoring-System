# AI-Powered-Real-Time-Industrial-Safety-and-PPE-Compliance-Monitoring-System
# IndustrialVision AI

**IndustrialVision AI** is an AI-powered real-time industrial safety and PPE (Personal Protective Equipment) compliance monitoring system designed to improve workplace safety through Computer Vision and Deep Learning.

The system uses AI-based object detection to monitor workers and identify whether required personal protective equipment is being used correctly. It can analyze images and video streams in real time and detect safety-related objects such as helmets, safety vests, masks, and other PPE according to the classes included in the trained model.

The main goal of the project is to reduce dependence on manual safety monitoring and provide an automated visual monitoring solution that can assist safety personnel in identifying PPE non-compliance quickly.

## 🎯 Project Objective

The primary objective of IndustrialVision AI is to develop an intelligent safety monitoring system capable of:

* Monitoring industrial environments in real time.
* Detecting workers using Computer Vision.
* Identifying required PPE equipment.
* Detecting PPE compliance and non-compliance.
* Providing real-time detection results.
* Generating alerts for safety violations.
* Recording detection information for analysis.
* Supporting industrial safety teams with automated monitoring.

## 🧠 How the System Works

The system follows an AI-based Computer Vision pipeline:

```text
Camera / Video / Image
        ↓
Frame Capture
        ↓
Image Preprocessing
        ↓
AI Object Detection Model
        ↓
Worker & PPE Detection
        ↓
Compliance Analysis
        ↓
Safety Violation Detection
        ↓
Real-Time Alert
        ↓
Monitoring & Analytics
```

The system receives visual input from an image, video, or camera stream. Each frame is processed by the trained AI model. The model identifies workers and PPE-related objects and provides bounding boxes and confidence scores.

The detected objects are then analyzed to determine whether the required PPE is present. If a safety violation is identified, the system can generate an alert.

## 🛡️ PPE Compliance Monitoring

PPE compliance is an important component of the system.

Depending on the trained dataset, the model can identify PPE categories such as:

* Safety Helmet
* Safety Vest
* Face Mask
* Safety Gloves
* Safety Goggles
* Safety Shoes
* Person/Worker

The exact classes depend on the dataset used to train the model.

The system can identify situations such as:

```text
Worker Detected
       ↓
Required PPE Checked
       ↓
PPE Present?
   ↙️          ↘️
 YES           NO
 ↓              ↓
Compliant     Violation
                 ↓
               Alert
```

## 🚨 Real-Time Safety Alerts

When the system detects a predefined PPE violation, it can generate a safety alert.

Examples include:

* Worker without safety helmet
* Worker without safety vest
* Missing required PPE
* Unsafe worker condition
* Other detected safety violations

The alert mechanism can be extended to provide:

* On-screen alerts
* Sound alarms
* Email notifications
* SMS notifications
* Dashboard notifications
* Safety event logging

## 📹 Real-Time Monitoring

The system is designed with real-time monitoring as a key objective.

It can be extended to work with:

* Live camera feeds
* CCTV cameras
* Recorded videos
* Uploaded videos
* Images

The AI model processes video frames and displays detection results with bounding boxes and confidence scores.

## 🤖 AI and Deep Learning

IndustrialVision AI uses a YOLO-based object detection model for real-time detection.

The trained model is stored as:

```text
best.pt
```

The model provides information such as:

* Detected object/class
* Bounding box
* Confidence score
* Number of detected objects

The model can be further improved by training it with additional industrial safety images and properly annotated PPE datasets.

## ⚙️ Technologies Used

* **Python** — Main programming language
* **YOLO / Ultralytics** — Real-time object detection
* **PyTorch** — Deep Learning framework
* **OpenCV** — Image and video processing
* **Streamlit** — Interactive monitoring interface
* **NumPy** — Numerical processing
* **Pandas** — Data processing and analytics

## 📊 Monitoring and Analytics

Detection results can be used to generate safety analytics such as:

* Total workers detected
* PPE compliance count
* PPE violation count
* Detection confidence
* Safety violati
