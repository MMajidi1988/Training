# Multi-GPU Training on YOLO

This script is designed for the training of YOLO (You Only Look Once) models on multiple GPUs. It incorporates several utilities including Comet ML for experiment tracking, Ultralytics YOLO, and RTDETR for object detection, as well as utilities for logging and monitoring GPU and CPU usage.
Features

    Comet ML Integration: Seamlessly track your experiments with Comet ML.
    Multi-GPU Support: Automatically detects and utilizes available GPUs for training.
    Performance Logging: Logs training performance metrics and hardware usage.
    Dynamic Model Loading: Flexibly loads different YOLO model variants.

Prerequisites

    Python 3.6+
    PyTorch
    Comet ML
    Ultralytics YOLO and RTDETR
    GPUtil, psutil
    tqdm

Installation

    Clone the repository and navigate to the script's directory.
    Install the required dependencies:

    bash

    pip install torch comet_ml gputil psutil tqdm

    (Optional) Set up Comet ML by creating an account and obtaining an API key.

Usage

    Ensure you have the necessary models and hyperparameters.json file in the specified directory.
    Set the COMET_EVAL_LOG_CONFUSION_MATRIX environment variable if needed.
    Run the script:

    bash

    python [script_name].py

Configuration

    Model Paths: Edit the models_to_load dictionary in the script to specify the paths to your YOLO model files.
    Hyperparameters: Modify hyperparameters.json to adjust training parameters.

Logging

    Training logs are saved in training_log.log.
    Hardware usage (CPU and GPU) is logged during training.
    Training duration is also logged upon completion.

Contributing

Feel free to fork this repository and contribute by submitting a pull request.
