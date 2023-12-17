# Face Recognition Alert System

## Overview

This Face Recognition Alert System, implemented in Python using OpenCV, NumPy, and face_recognition library, provides real-time face recognition. It detects known faces and sends alerts for unknown faces, utilizing Firebase Cloud Messaging (FCM) for notifications.

## Features

- **Face Recognition:** Utilizes the face_recognition library to recognize known faces.
- **Real-time Alerts:** Sends real-time alerts for unknown faces detected in the webcam feed.
- **Firebase Cloud Messaging:** Sends push notifications using FCM for both known and unknown face events.
- **Dynamic Arrival Tracking:** Tracks the arrival of known faces, sending arrival alerts.

## Setup Instructions

1. Install the required libraries:
    ```bash
    pip install opencv-python numpy face_recognition requests
    ```

2. Update the `path` variable in the code to the directory where images for face recognition are stored.

3. Set up Firebase Cloud Messaging (FCM):
    - Replace `serverToken` with your FCM server token.
    - Replace `deviceToken` with the FCM device token for the recipient.

4. Run the script:
    ```bash
    python <script_filename>.py
    ```

## Usage

- The system continuously captures the webcam feed and alerts for unknown faces.
- Upon detecting an unknown face, a push notification is sent to the specified device.
- The user can provide feedback by confirming whether they know the detected person.

## Note

- The system supports dynamic addition of known faces through user input during runtime.

Feel free to explore and customize the code to fit your specific use case!
