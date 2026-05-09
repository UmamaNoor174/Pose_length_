**Pose Analytics: Body Landmark Distance Tracker** 📏🧘‍♂️

An advanced Computer Vision application that utilizes MediaPipe and OpenCV to detect human poses and calculate real-time Euclidean distances between specific body landmarks (like wrists, eyes, and mouth).

📌 **Project Overview**

This project goes beyond simple pose detection by implementing mathematical geometry to measure body proportions in real-time. By calculating the pixel distance between landmarks, it provides quantitative data that can be used for ergonomics, fitness form correction, or specialized behavior analysis.

✨ **Key Features**

1. Distance Measurement: Automatically calculates Euclidean distance between:
     Left and Right Wrists.
     Left and Right Eyes.
     Mouth width (Left to Right corners).

2. Real-Time Skeleton Overlay: Visualizes 33 skeletal landmarks with distinct color coding for joints and connections.

3. On-Screen HUD: Displays live pixel measurements directly on the video feed for immediate analysis.

4. Coordinate Scaling: Converts normalized landmark coordinates into actual pixel values based on the webcam resolution.

🛠️ **Technical Stack**

1. Language: Python 3.11
2. Core Libraries:
    OpenCV: Video stream processing and UI text rendering.
    MediaPipe: Real-time 3D pose landmark detection.
    Math: For geometric calculations (Euclidean distance).

3. Framework Compatibility: Can be integrated into Flask-based web dashboards.

**Setup and Installation**

1. Clone the Repository:
Bash
git clone https://github.com/UmamaNoor174/pose-analytics.git
cd pose-analytics
2. Install Dependencies:
Bash
pip install opencv-python mediapipe
3. Run the Project:
Bash
python pose_length.py

**How it Works**

1. Logic: 
The script uses the formula $d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$ to find the distance between any two body points.

2. Detection: 
Stand in front of the webcam; the system will automatically identify your wrists, eyes, and mouth.

3. Output: 
Live distances (in pixels) will appear in the top-left corner of the screen.

4. Exit: Press 'q' to stop the session.

**Academic Context**

This research is conducted within the Department of Information Technology. The logic used here is a core component of the Student Behaviour Monitoring System, helping to identify specific physical actions or postures during examinations through precise spatial analysis.

👤 **Developer**
Umama Noor
