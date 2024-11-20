# Chess-Robotic-Arm (Voice Recognition)
Here’s a detailed **README.md** file for your voice recognition repository:

---

# Voice Recognition Technology for Chess Robot

## Project Overview  
This voice recognition system empowers disabled players to interact with a chess robot by using natural voice commands. It bridges the gap between voice input and physical chess moves, enhancing accessibility and engagement. The purpose is to ensure every individual can enjoy chess effortlessly, creating a seamless experience. **By integrating advanced voice recognition with chess logic, the system translates player commands into physical movements on the board.**

---

## Key Features  
- **Natural Language Input:** Players can use simple phrases like "move knight to e5" to interact with the robot.  
- **Command Parsing:** Intelligent parsing of commands ensures accurate understanding of chess-related instructions.  
- **Validation with Chess Logic:** Ensures all moves are legal before execution.  
- **Robotic Arm Control:** Converts voice commands into movements for the robotic chess arm.  
- **Error Feedback:** Provides real-time feedback for invalid commands or illegal moves.  
- **Audio Response:** Uses text-to-speech to confirm moves and guide users during gameplay.

---

## Getting Started  
To begin with this project, you'll need specific hardware and software components. Follow the steps below to set up and start using the system seamlessly.

---

## Materials  
- **Microphone:** A high-quality mic to capture the player's voice commands clearly.  
- **Chess Robot Arm:** A robotic arm for executing chess moves physically.

---

## Prerequisites  
**Before diving into the setup, make sure you have the required hardware components mentioned above and software dependencies installed.**  

### Software Dependencies  
- **Python 3.8+**: The primary language for this project.  
- **Picovoice Leopard:** Voice-to-text processing tool.  
  ```bash
  pip install pvleopard
  ```  
  Converts speech input into text commands with high accuracy.  

- **gTTS (Google Text-to-Speech):** Generates audio responses.  
  ```bash
  pip install gtts
  ```  
  Converts text feedback into audio for better user interaction.  

- **Chess Library:** Implements chess rules and logic.  
  ```bash
  pip install chess
  ```  
  Ensures all moves are validated before execution.  

- **Serial Communication Library:** Interfaces with the robotic arm.  
  ```bash
  pip install pyserial
  ```  
  Handles communication between the chess robot and your system.  

- **OS Module:** Handles file management and audio playback. *(No installation required; it's a built-in Python module.)*

---

## Installation  

### Part 1: Download and Build Necessary Packages  
1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/YourUsername/VoiceRecognitionChess.git
   cd VoiceRecognitionChess
   ```  

2. **Install Required Libraries:**  
   Install all dependencies using the `requirements.txt` file:  
   ```bash
   pip install -r requirements.txt
   ```  

3. **Check Missing Packages:**  
   Ensure all libraries are installed. Use this command to verify:  
   ```bash
   pip freeze
   ```  

   If any package is missing, install it manually using `pip install <package-name>`.  

4. **Build Hardware Communication Setup:**  
   Ensure your robotic arm is connected via USB or Bluetooth and recognized by the system.  

### Part 2: Python Environment and Packages  
1. **Set Up a Python Virtual Environment:**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```  

2. **Install Required Python Packages:**  
   Re-run:  
   ```bash
   pip install -r requirements.txt
   ```  
   This ensures the environment contains all dependencies.

---

## Configuration of the Project  
Here are the main variables used in the project and their roles:  
- **`leopard`**: Initializes the Picovoice Leopard model for speech-to-text.  
- **`chess_board`**: Represents the current state of the chess game.  
- **`ser`**: Manages communication with the robotic arm.  
- **`frames`**: Stores recorded audio frames for processing.  
- **`piece` and `target`**: Extracted from the command to identify the chess piece and target square.  
- **`tts`**: Handles text-to-speech conversion.  
- **`command`**: The full voice command given by the user.

---

## Support  
Need help? You can reach out directly via the **Issues** tab of the Github page for support.

---
