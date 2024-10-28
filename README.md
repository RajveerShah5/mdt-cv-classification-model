# YOLOv5 Object Detection

This repository contains scripts for running YOLOv5 benchmarks on all supported export formats, training the YOLOv5 model on custom datasets, and validating trained models. YOLOv5 is a state-of-the-art object detection model.

## Requirements
To run the scripts in this repository, you'll need the following dependencies:
- Python 3.6+
- PyTorch
- Other dependencies as listed in `requirements.txt`

## Command Line Arguments
--weights: Path to the model weights (default: yolov5s.pt)
--source: Path to input source (default: data/images)
--img-size: Inference size in pixels (default: 640)
--conf-thres: Confidence threshold (default: 0.25)
--iou-thres: NMS IoU threshold (default: 0.45)
--device: Device to run on (cuda device, i.e. 0 or 0,1,2,3 or cpu)
--view-img: Display results
--save-txt: Save results to *.txt
--save-csv: Save results to *.csv
--classes: Filter by class
For a full list of options, run python detect.py --help.

## Output
Detection results will be saved in the runs/detect directory by default. This includes:
Annotated images/videos
Text files with detection information (if --save-txt is used)
CSV files with detection information (if --save-csv is used)

## Contributing
Contributions to improve the code or add new features are welcome.

## Acknowledgments
This code is based on the Ultralytics YOLOv5 project. Please refer to their repository for more detailed information about the YOLOv5 architecture and training process.
