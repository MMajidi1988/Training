Multi-GPU Training on YOLO README
This script facilitates training YOLO (You Only Look Once) models using multiple GPUs. It integrates Comet ML for experiment tracking, Ultralytics YOLO and RTDETR for object detection, and tools for logging and monitoring GPU and CPU usage.

Features
- Comet ML Integration for experiment tracking.
- Automatic detection and utilization of multiple GPUs for training.
- Performance metrics and hardware usage logging.
- Flexibility in loading different YOLO model variants.

Requirements
Python 3.6+
PyTorch
Comet ML
Ultralytics YOLO and RTDETR
GPUtil, psutil, tqdm

Install these libraries using pip:

pip install torch comet_ml gputil psutil tqdm

Setup
Set the `COMET_EVAL_LOG_CONFUSION_MATRIX` environment variable as needed.
Configure your model paths and hyperparameters in `models_to_load` and `hyperparameters.json`, respectively.

Usage
Ensure models and `hyperparameters.json` are in the specified directory.
Run the script in your Python environment:

python [your_script_name].py

Logging
Training logs are recorded in `training_log.log`.
CPU and GPU usage are monitored and logged.
Training completion time is logged.

Contributions
Contributions are welcome. Please fork this repository and submit a pull request with your changes.

License
This project is licensed under the MIT License.

Disclaimer
This script is provided "as is", without warranty of any kind. Use at your own risk.

Happy Coding! 🚀🤖
