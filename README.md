# 🖐️ Rock-Paper-Scissors using Hand Gesture Recognition

### 🎮 A Real-Time AI-Based Game using OpenCV & MediaPipe

---

## 📌 Project Overview
**RPS_game.py** is a real-time **Rock-Paper-Scissors game** that uses **hand gesture recognition** to let you play against your computer.  
Your webcam captures your hand movement, **MediaPipe** detects the gesture (Rock, Paper, or Scissors), and the computer makes a random move.  
The result is displayed live on the screen with updated scores after every round.

---

## 🧠 Key Features
- 🖐️ Real-time hand gesture detection using **MediaPipe Hands**
- 🎥 Live video feed handled through **OpenCV**
- 🤖 Computer randomly generates its own move
- 📊 Dynamic round-based scoring system
- ⏳ Built-in countdown before every round
- 💬 Displays player and computer gestures visually

---

## 🏗️ Technologies Used
| Library | Purpose |
|----------|----------|
| **Python 3.8+** | Programming language |
| **OpenCV (cv2)** | Video capture, image processing, and frame display |
| **MediaPipe** | Hand landmark detection and tracking |
| **Random** | Generates computer’s random choice |
| **Time** | Manages countdown and round timing |

---

## ⚙️ Installation and Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/arxeman/RPS_game.git
cd RPS_game
```

### 2️⃣ Install Dependencies
Make sure Python 3.8 or higher is installed, then run:
```bash
pip install opencv-python mediapipe
```

### 3️⃣ Run the Program
```bash
python RPS_game.py
```

---

## 🕹️ How to Play
1. Run the program — your webcam window will open.  
2. Enter how many rounds you want to play.  
3. A **countdown (3...2...1)** will appear before each round.  
4. Show one of these gestures in front of the camera:

| Gesture | Description |
|----------|-------------|
| ✊ **Rock** | All fingers closed |
| 🖐️ **Paper** | All fingers open |
| ✌️ **Scissors** | Only index and middle fingers open |

5. The computer chooses randomly between rock, paper, or scissors.  
6. The round result (Win/Lose/Tie) and both choices are displayed on screen.  
7. After all rounds, the **final score** and **overall winner** appear in the terminal.

---

## 🧩 Code Structure
| File | Description |
|------|-------------|
| **RPS_game.py** | Main Python file containing the entire game logic |
| **README.md** | Documentation and usage guide |

### 🔍 Core Functions
| Function | Description |
|-----------|-------------|
| `determine_gesture(hand_landmarks)` | Detects and returns player’s gesture |
| `get_computer_choice()` | Randomly picks computer’s move |
| `get_winner(player_choice, computer_choice)` | Determines round winner |
| `show_countdown(cap, seconds)` | Displays countdown before each round |

---

## 🧠 Logic Overview
- Captures frames from webcam using **OpenCV**  
- Uses **MediaPipe Hands** to detect 21 hand landmarks  
- Analyzes the relative positions of finger tips and joints  
- Classifies gestures as:
  - All fingers down → **Rock**
  - All fingers up → **Paper**
  - Only index & middle up → **Scissors**
- Compares the player’s gesture with the computer’s random choice  
- Updates the score and shows results in real-time  

---

## 🖼️ Sample Output

### 💻 Console:
```
Enter number of rounds: 3

Final Scores:
Player: 2
Computer: 1
You win the game!
```

### 📷 Webcam Window:
- Displays hand landmarks and gesture outline  
- Shows current round, scores, and both gestures  
- Displays “Result: Player/Computer/Tie” dynamically  

---

## 🚀 Future Enhancements
- Add **multiplayer support**  
- Integrate **sound effects** and a graphical interface (GUI)  
- Enhance detection accuracy using **deep learning**  
- Develop **mobile app version** with camera-based gesture tracking  

---

## 🎓 Learning Outcomes
- Learned real-time image processing using **OpenCV**
- Understood **gesture recognition** through **MediaPipe**
- Implemented **logic-based game flow** in Python
- Gained insight into **AI-based human-computer interaction**

---

## 🧾 License
This project is open-source and free for educational or personal use.  
Feel free to fork, modify, and share with proper credit.

---

## 👨‍💻 Author
**Name:** Aryeman Verma  
**GitHub:** [@arxeman](https://github.com/arxeman)  
**Course:** B.E. Computer Science and Engineering  
**University:** Chandigarh University  
**Year:** 2025  

---

⭐ *If you like this project, don’t forget to star the repository!* ⭐
