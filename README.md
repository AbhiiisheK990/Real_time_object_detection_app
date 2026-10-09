# Real-Time Object Detection App

A real-time object detection Android application built using **Flutter** and **TensorFlow Lite** with the **SSD MobileNet** model. The app detects objects using the device camera, provides spoken announcements for detected objects, and performs inference directly on the device without requiring an internet connection.

## Features

- **Real-Time Object Detection:** Detects and identifies objects from the live camera feed.
- **Flutter-Based UI:** Provides a mobile interface for real-time object recognition.
- **TensorFlow Lite Integration:** Runs a lightweight machine learning model optimized for mobile devices.
- **SSD MobileNet Model:** Uses a pre-trained object detection model for identifying common objects.
- **Optimized Mobile Inference:** Achieves approximately 40 FPS on a Snapdragon 450 device under the tested conditions.
- **Text-to-Speech Accessibility:** Announces detected objects using spoken audio feedback.
- **Cooldown Filtering:** Reduces repetitive voice announcements for continuously detected objects.
- **Offline Processing:** Performs object detection on-device without requiring cloud services.

## Tech Stack

- **Framework:** Flutter
- **Programming Language:** Dart
- **Machine Learning:** TensorFlow Lite
- **Object Detection Model:** SSD MobileNet
- **Accessibility:** Text-to-Speech (TTS)
- **Platform:** Android

## How It Works

1. The device camera captures live video frames.
2. Frames are processed using the TensorFlow Lite SSD MobileNet model.
3. The model identifies objects and generates detection results.
4. Detected object labels are displayed in the application.
5. Text-to-speech announces detected objects, with cooldown filtering to avoid repetitive announcements.
6. All inference takes place locally on the device, enabling offline operation.

## Performance

The application achieved approximately **40 FPS on a device powered by the Snapdragon 450 processor** during testing.

Actual performance may vary depending on the device hardware, input resolution, model configuration, and inference settings.

## Getting Started

### Prerequisites

Install the following tools:

- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Android Studio](https://developer.android.com/studio) or Android SDK tools
- [Git](https://git-scm.com/downloads)
- A physical Android device or compatible emulator

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/AbhiiisheK990/Real_time_object_detection_app.git
```

**2. Navigate to the project directory**

```bash
cd Real_time_object_detection_app
```

**3. Install dependencies**

```bash
flutter pub get
```

**4. Connect an Android device**

Enable USB debugging on your device and connect it to your computer, or launch an Android emulator.

**5. Run the application**

```bash
flutter run
```

Grant camera and any required audio-related permissions when prompted.

## Model Information

The application uses SSD MobileNet with TensorFlow Lite for object detection on mobile devices.

The model file and its associated label file must be configured correctly in the project. Refer to the model paths and asset declarations in `pubspec.yaml` and the application's source code.

## Accessibility

The app includes text-to-speech functionality to announce recognized objects. Cooldown filtering helps limit repeated announcements when the same object remains in the camera frame.

This feature is intended to make object recognition more accessible, but the application should not be considered a replacement for dedicated assistive technology or safety equipment.

## Future Improvements

- Improve detection accuracy and inference performance.
- Add configurable voice announcement settings.
- Support additional object detection models.
- Improve handling of overlapping and frequently changing detections.
- Expand accessibility and usability features.
- Evaluate performance across a wider range of Android devices.

## Contributing

Contributions, suggestions, and bug reports are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a pull request describing your improvements.

## License

Add a license to this repository if you intend to allow others to use, modify, and distribute the project. Until a license is specified, the repository's reuse permissions remain subject to applicable copyright law.

## Author

**Abhishek Hiremath**

GitHub: [@AbhiiisheK990](https://github.com/AbhiiisheK990)
