# Hand-Gesture-Volume-Control  

This project leverages computer vision and hand gesture recognition to control system audio volume in real-time. Using Python libraries such as **MediaPipe**, **OpenCV**, and **PyCaw**, it processes live video feed, detects hand gestures, and maps the distance between specific fingers to the system's volume level.  

---

## Features  

- **Real-time Hand Tracking**: Detects and tracks hand landmarks using MediaPipe.  
- **Gesture-based Volume Control**: Adjusts system audio by measuring the distance between the thumb and index finger.  
- **Interactive Feedback**: Displays finger landmarks, a dynamic volume bar, and volume percentage on the video feed.  
- **System Audio Integration**: Controls audio using PyCaw's interface with the operating system.  

---

## How It Works  

1. **Hand Landmark Detection**:  
   - MediaPipe detects hand landmarks in the webcam feed.  
   - Identifies the thumb tip (ID 4) and index finger tip (ID 8).  

2. **Distance Calculation**:  
   - Computes the distance between the thumb and index finger using the Euclidean formula.  
   - Maps this distance to the system's volume range (-63.5 dB to 0 dB).  

3. **Volume Adjustment**:  
   - Adjusts the system volume using PyCaw based on the calculated distance.  

4. **Visual Feedback**:  
   - Displays circles on the finger tips and a connecting line.  
   - Shows a dynamic volume bar and percentage on the screen.  

---

## Technologies Used  

- **Python**  
- **OpenCV**: For video processing and visualization.  
- **MediaPipe**: For hand tracking and landmark detection.  
- **PyCaw**: For system audio control.  
- **NumPy**: For numerical computations.  

---

## Installation  

1. Clone the repository:  
   ```bash
   git clone https://github.com/vikneshsr13/Hand-Gesture-Volume-Control.git
   cd Hand-Gesture-Volume-Control

##Usage

Run the script.
Show your hand in front of the webcam.
Adjust the distance between your thumb and index finger to control the volume.
Press the spacebar to exit.

##Future Enhancements

Support for multi-hand gestures to control other system functionalities (e.g., screen brightness, media playback).
Add gesture recognition for predefined actions like play/pause or mute.
Optimize performance for low-latency processing.
Cross-platform compatibility improvements.
