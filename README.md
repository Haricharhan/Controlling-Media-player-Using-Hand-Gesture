
# Hand Gesture Recognition for Keyboard Control

This project leverages **OpenCV**, **MediaPipe**, and **PyAutoGUI** to recognize hand gestures and translate them into keyboard inputs. By counting the number of fingers held up, the program can trigger different keypress events, making it possible to control applications or games without a keyboard.

## Features

- **Gesture Recognition:** The program detects the number of fingers held up using MediaPipe's hand landmarks.
- **Keyboard Control:** Each gesture corresponds to a different keypress (e.g., one finger = right arrow key, two fingers = left arrow key, etc.).
- **Real-time Processing:** The program processes video input from the webcam in real-time, allowing immediate response to hand gestures.

## How It Works

1. **Hand Detection:** The program uses MediaPipe to detect and track hand landmarks.
2. **Finger Counting:** A custom function calculates the number of fingers extended based on landmark positions.
3. **Key Pressing:** Depending on the number of fingers detected, a specific key press is simulated using PyAutoGUI.

### Key Mappings:

- **1 Finger:** Right arrow key
- **2 Fingers:** Left arrow key
- **3 Fingers:** Up arrow key
- **4 Fingers:** Down arrow key
- **5 Fingers:** Space key

## Installation

To run this project, you'll need to have Python installed along with the following libraries:

```bash
pip install opencv-python mediapipe pyautogui
```

## Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/hand-gesture-keyboard-control.git
```

2. Navigate to the project directory:

```bash
cd hand-gesture-keyboard-control
```

3. Run the program:

```bash
python main.py
```

4. Use your webcam to display different hand gestures and see the corresponding key presses in action.

## Example Images

Here are some screenshots showing the application in action:

![1_clagIwqV2gdz-UoAcpOKAg (1)](https://github.com/user-attachments/assets/7899fccb-ff3d-429c-b783-08572cc42bf2)

 *Figure 1: The program detects points in the hand..*

![hand](https://github.com/user-attachments/assets/b2a82f4d-3e5b-4811-82ec-1a1821befe2e)

*Figure 2:  Specific names for Points .*

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Contributions are always welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
