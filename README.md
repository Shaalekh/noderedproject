# AI-Animatronics Integration with Node-RED

## Overview
This project integrates AI with animatronics using Node-RED. It enables real-time control of servo motors, speech synthesis, and AI-driven automation for lifelike robotic movements and interactions, including an AI-controlled eye mechanism.

## Features
- **AI-driven control**: Uses AI models for intelligent decision-making.
- **Speech synthesis & recognition**: Enables voice interaction.
- **Servo motor control**: Animates robotic components.
- **MQTT communication**: Facilitates seamless data transfer.
- **Node-RED integration**: Provides a visual programming environment for easy customization.

## Hardware Requirements
- **Microcontroller** (Arduino, ESP32, or similar)
- **Servo Motors** (SG90, MG995, etc.)
- **PCA9685 Servo Driver** (if using multiple servos)
- **Power Supply** (5V 5A for servos)
- **Microphone & Speaker** (for speech interaction)
- **OLED Display** (optional, for visual feedback)

## Software Requirements
- **Node-RED** (latest version)
- **MQTT Broker** (e.g., Mosquitto)
- **Python 3.12** (for AI processing)
- **Google Gemini API / Dialogflow** (for AI-based responses)
- **Vosk** (for voice recognition)

## Installation & Setup
1. **Install Node-RED**
   ```sh
   npm install -g --unsafe-perm node-red
   ```
2. **Set up MQTT Broker**
   ```sh
   sudo apt install mosquitto mosquitto-clients
   ```
3. **Install Required Node-RED Nodes**
   ```sh
   cd ~/.node-red
   npm install node-red-dashboard node-red-contrib-mqtt node-red-contrib-google-action-dialogflow-http
   ```
4. **Set Up AI Services**
   - Configure Google Gemini API or Dialogflow
   - Set up Azure Speech-to-Text
5. **Deploy Flow in Node-RED**
   - Import the provided `flow.json` into Node-RED
   - Connect your hardware and start the Node-RED server
   ```sh
   node-red
   ```

## Usage
- **Voice Commands**: Speak commands to control servos and trigger AI responses.
- **Automated Animations**: Define motion sequences based on AI inputs.
- **Remote Control**: Use an MQTT client to send movement commands.

## Future Enhancements
- **Facial Recognition** for personalized interactions.
- **Gesture Control** using camera-based tracking.
- **Enhanced Speech Processing** with custom voice models.

## Contributions
Feel free to fork this repository and submit pull requests for improvements.

## License
This project is licensed under the MIT License.

---
### Author: [Your Name]  
### Contact: [Your Email / GitHub Profile]

