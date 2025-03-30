# STM-AI: Development of a Web-Based Trained Image Classification for Real-Time Image Recognition 💻

## Overview

This project demonstrates the integration of advanced AI models with resource-constrained embedded systems, specifically using the STM32H747I-DISCO microcontroller board for real-time image recognition. The system leverages Google's Teachable Machine for model training and STM32Cube.AI Developer Cloud for optimization, showcasing the potential of deploying sophisticated AI applications on low-power hardware.

## Table of Contents 

- [Project Objectives](#project-objectives)
- [Features](#features)
- [Hardware Components](#hardware-components)
- [Software Tools](#software-tools)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Challenges](#challenges)
- [Future Work](#future-work)
- [Contributors](#contributors)
- [License](#license)

## Project Objectives🎯

1. **Optimization Techniques**: Develop and implement optimization strategies for image classification models to be deployed on resource-constrained STM32 microcontrollers.
2. **Real-Time Inference**: Deploy optimized models onto STM32 microcontrollers ensuring real-time inference capabilities with adequate accuracy and frame rates.

## Features⚡

- Real-time image recognition using STM32H747I-DISCO board.
- User-friendly model training via Teachable Machine.
- Model optimization for STM32 architecture using STM32Cube.AI Developer Cloud.

## Hardware Components🛠

### 1. STM32H747I-DISCO Board
- Dual-core architecture with strong performance.
- Comprehensive peripherals including USB OTG HS, Ethernet, SAI Audio DAC, etc.

### 2. B-CAMS-OMV Camera Module
- Extension connectors compatible with multiple camera modules.
- Based on the OV5640 image sensor offering a 5-Mpixel resolution.

## Software Tools🧰

### 1. Teachable Machine
- Intuitive web-based tool for training machine learning models without extensive coding knowledge.

### 2. STM32Cube AI Developer Cloud
- Free online service for developing AI on ST devices, supporting tools for creation, optimization, and benchmarking.

### 3. STM32CubeIDE
- Integrated development environment for STM32 microcontrollers and microprocessors with debug tools, code creation, compilation, and peripheral configuration.

## Installation📲

### Prerequisites

- STM32H747I-DISCO board
- B-CAMS-OMV camera module
- Computer with internet access

### Steps

1. **Train the Model**:
   - Use [Teachable Machine](https://teachablemachine.withgoogle.com/) to train your image classification model.
   - Export the TensorFlow Lite model.

2. **Optimize the Model**:
   - Upload the exported model to [STM32Cube AI Developer Cloud](https://www.st.com/en/embedded-software/x-cube-ai.html).
   - Optimize and download the C code tailored for the STM32H747I-DISCO board.

3. **Integrate and Deploy**:
   - Open the downloaded C code in STM32CubeIDE.
   - Configure project settings, build, compile, and flash the firmware onto the STM32H747I-DISCO board.

## Usage💡

1. Connect the B-CAMS-OMV camera module to the STM32H747I-DISCO board using a flexible flat cable (FFC).
2. Power up the STM32H747I-DISCO board.
3. Place objects in front of the camera within the optimal range for image recognition.
4. Observe the output on the display or through connected interfaces.

## Results🔬

- Successfully demonstrated real-time image recognition on STM32H747I-DISCO board.
- Achieved notable accuracy in recognizing various objects including Arduino UNO, ESP32 cam, ESP8266, and Wi-Fi expansion board with STM32.

## Challenges🏳

- **Frame Rate Performance**: Limited to 1.7 frames per second (fps), impacting responsiveness.
- **Camera Focus**: Lack of auto-focus capability in the B-CAMS-OMV camera module affected image quality and classification accuracy.

## Future Work✅

- Enhance frame rate performance through advanced optimization techniques.
- Upgrade to a camera module with auto-focus capabilities.
- Expand the training dataset to improve robustness and generalizability.
- Explore different neural network architectures optimized for embedded systems.
- Improve user interface and experience by developing a comprehensive dashboard.

## Contributors👨🏻‍💻

- [Fakhrul Fauzi (me)](https://github.com/p1sangmas)
- Saiful Azree
- Haziq Hanafi

## License🪪

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by opening issues or submitting pull requests. For any questions, please contact the contributors listed above.
