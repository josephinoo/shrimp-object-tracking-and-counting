# Shrimp Object Tracking and Counting using YOLOv8
This repository contains code for an object tracking and counting system for shrimp using YOLOv8 implemented in PyTorch. The system is designed to be used with a video feed from a shrimp farm, and is capable of tracking individual shrimp and counting the number of shrimp present in the video.

### Authors
- Joseph Avila
- Xavier Toala

## Requirements
To use this system, you will need:

Python 3.6 or higher
PyTorch 1.7 or higher
OpenCV 4.5 or higher
YOLOv8 weights file
A video feed of a shrimp farm
To use the project, clone the repository and run the shrimp_tracker.py script. The script takes the path to a video file as input.

```bash
pip install torch opencv-python
```
You will also need to download the YOLOv8 weights file from the following link and place it in the weights/ directory:

- YOLOv8 Weights

## Usage
To use the system, you can run the following command:
```bash
python shrimp_tracker.py --video <path-to-video-file>
```

Replace <path-to-video-file> with the path to the video file you want to process. The output of the system will be a new video file with the tracked and counted shrimp. You can specify the output file name using the --output parameter. By default, the output file will be saved in the output/ directory with the name tracked_<input-file-name>.

You can also specify the confidence threshold for the detections using the --confidence parameter. The default value is 0.5.

```bash
python shrimp_tracker.py --video <path-to-video-file> --output <output-file-name> --confidence <confidence-threshold>
```

Credits
This code is heavily based on the following repositories:

- ultralytics/yolov5
- amdegroot/ssd.pytorch



## Contributing
Contributions to the project are welcome. If you find a bug or have an idea for a new feature, please open an issue on GitHub or submit a pull request.

## License
The project is licensed under the MIT License. See the LICENSE file for more information.
