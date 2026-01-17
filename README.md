FaceRecognition-Android
<p align="left"> High-performance Android SDK for real-time face recognition and face liveness detection, delivering up to <b>99.9% accuracy</b> with industry-leading speed and security. </p>
✨ Key Features

Real-time face recognition with latency below 200 ms

Advanced liveness detection to prevent photo and video spoofing attacks

Lightweight SDK with APK size under 35 MB

Fully compliant with ISO/IEC 30107-1 biometric standards

On-device processing only — no cloud transmission or data leakage

🏆 Industry Recognition
 
 
Overview

This repository showcases face recognition and face liveness detection technologies developed by KBY-AI, optimized specifically for native Android applications.

The SDK integrates both recognition and liveness capabilities into a single, efficient mobile solution designed for high-security biometric applications.

◾ FaceSDK (Mobile) Capabilities
Feature Category	Basic	Standard	Premium
Face Detection	✔	✔	✔
Face Liveness Detection	✔	✔	✔
Pose Estimation	✔	✔	✔
Face Recognition	✖	✔	✔
68-Point Face Landmarks	✖	✖	✔
Face Quality Assessment	✖	✖	✔
Face Occlusion Detection	✖	✖	✔
Eye Closure Detection	✖	✖	✔
Age & Gender Estimation	✖	✖	✔
◾ FaceSDK (Mobile) Product List
No.	Repository	SDK Type
1	Face Liveness Detection – Android	Basic
2	Face Liveness Detection – iOS	Basic
➡️	Face Recognition + Liveness – Android	Standard
4	Face Recognition + Liveness – iOS	Standard
5	Face Recognition + Liveness – Flutter	Standard
6	Face Recognition + Liveness – Ionic-Cordova	Standard
7	Face Recognition + Liveness – React Native	Standard
8	Face Attribute – Android	Premium
9	Face Attribute – iOS	Premium
10	Face Attribute – Flutter	Premium

For Face SDK (Server) solutions, visit: https://github.com/kby-ai/Product

📲 Try the Demo App
Google Play

Download the official demo application from Google Play to experience real-time face recognition and liveness detection.

🎥 Performance Demonstration
 
📸 Screenshots

(Screenshots retained as provided)
  
  

🔧 SDK APIs
Face Detection & Liveness
FaceSDK.faceDetection(bitmap, param)


Returns a list of FaceBox objects containing:

Face bounding box

Liveness score

Facial angles (yaw, roll, pitch)

Template Extraction
byte[] template = FaceSDK.templateExtraction(bitmap, faceBox)


Generates a biometric template used for identity verification.

Similarity Calculation
float similarity = FaceSDK.similarityCalculation(template1, template2)


Returns a similarity score between two face templates.

YUV to Bitmap Conversion
Bitmap bitmap = FaceSDK.yuv2Bitmap(nv21, width, height, mode)


Converts camera YUV frames into Bitmap format.
The mode parameter depends on camera orientation.
