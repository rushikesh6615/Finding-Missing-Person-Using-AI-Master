🔹 1. Introduction
Every year, thousands of people go missing, and traditional search operations often rely on manual, slow, and error-prone processes. With the rise of Artificial Intelligence (AI) and facial recognition technologies, it's now possible to automate and accelerate the search for missing individuals.
This project proposes an AI-based facial recognition system that can match photos of found individuals against a central database of missing person records, offering a faster, more reliable solution to aid families, police departments, and NGOs.

🔹 2. Objective
Detect and recognize faces using AI and computer vision.

Compare real-time or uploaded images with a database of missing individuals.

Provide intelligent matching results to assist in identification.

Offer a user-friendly interface for uploading, searching, and managing case records.

🔹 3. Key Features
📸 Upload an image of a person (found or missing).

🤖 Run AI model to extract facial embeddings.

🔍 Match the face with an existing dataset of missing individuals.

🧾 Add, update, and manage personal details in the missing persons database.

🎥 (Optional) Real-time face detection from webcam or CCTV footage.

🔹 4. Technologies Used
🔸 Frontend
HTML5, CSS3, JavaScript

Bootstrap / React (optional UI layer)

🔸 Backend
Python with Flask or Django

OpenCV for image preprocessing

face_recognition or dlib for face encoding

TensorFlow/Keras for deep learning models

🔸 Database
SQLite / MongoDB (to store person data and embeddings)

🔸 Libraries & Tools
NumPy, Pandas, OpenCV, face_recognition, Flask, TensorFlow/Keras

🔹 5. System Workflow
Image Input
User uploads a photo (JPEG, PNG) of a person they are trying to identify.

Face Detection & Encoding
The AI model detects the face, extracts 128D facial embeddings (using dlib or deep CNN).

Matching
Compares the encoding with existing entries in the database using Euclidean distance threshold.

Result Display
Shows matched profile (if found), or option to add the face as a new missing person.

Live Mode (Optional)
Captures faces in real-time using a webcam and checks against the database.

🔹 6. Dataset
Contains images of known missing individuals (manually collected or from public databases).

Each entry includes:

Name, Age, Gender

Last Seen Location

Date Missing

Associated Face Image

Facial embeddings are stored separately for quick comparison.

🔹 7. Algorithms Used
✅ Face Detection
Using HOG + SVM or CNN face detector from dlib.

✅ Facial Embedding Extraction
CNN-based face encoders convert faces into 128-dimensional vectors.

✅ Matching Algorithm
Uses Euclidean Distance to measure similarity between facial embeddings.

A threshold (e.g., 0.6) determines whether a match is acceptable.

🔹 8. Evaluation Metrics
Accuracy: % of correctly matched individuals.

Precision/Recall: Measures false positives and false negatives.

Time Efficiency: Time taken to detect, encode, and match faces.

Robustness: Works under different lighting, pose, and image quality conditions.

🔹 9. Limitations
Accuracy depends on image quality and angle.

Faces with aging, disguises, or partial occlusion might not match well.

Requires sufficient number of training samples for improved accuracy.

🔹 10. Future Enhancements
Integrate face aging prediction models to match old images with current ones.

Add location-based filters using GPS tagging.

Support multi-face detection in real-time video feeds.

Build a mobile application for field use by law enforcement.

🔹 11. Conclusion
This project demonstrates the transformative potential of AI in social applications. By automating facial recognition for missing persons, we not only reduce the manual burden but also significantly improve the chances of timely identification.
With further enhancements and wider dataset access, this system can evolve into a powerful nationwide or even global tool for humanitarian efforts.

🔹 12. References
dlib: https://github.com/davisking/dlib

face_recognition: https://github.com/ageitgey/face_recognition

OpenCV Documentation: https://docs.opencv.org/

Real-Time Face Recognition Research: https://arxiv.org/abs/1905.08789
