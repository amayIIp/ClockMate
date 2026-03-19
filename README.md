# ♟️ ClockMate: The Over-The-Board Chess Digitizer

ClockMate isn't just another iOS chess clock—it's a bridge between physical (over-the-board) chess and the digital world. Built with **SwiftUI**, it tracks your remaining time to the millisecond while simultaneously converting your physical moves into a digital **PGN (Portable Game Notation)** file. Basically, no more frantically scribbling down moves on a scorecard while you're in severe time trouble.

![Swift](https://img.shields.io/badge/Swift-5.x-FA7343?style=flat&logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-16.0+-000000?style=flat&logo=apple&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-UI-007AFF?style=flat)

---

## ✨ Features That Actually Matter

- **Real-Time PGN Generation** — Tracks every move entered and compiles a standard PGN file. Perfect for analyzing your blunders later with Stockfish.
- **Sub-Millisecond Time Management** — Complex state-machine logic ensures the clock is brutally accurate.
- **Move Input Interface** — A clean, distraction-free UI designed to register moves fast during blitz or bullet scrambles.
- **Game State Tracking** — Keeps a continuous history of the board state so it always knows whose turn it is and what the timing controls are.

## 🏗️ Technical Highlights

- **State Management**: Handling rapid, async user inputs while maintaining a perfect chronometer required rigorous state management. It uses Swift's modern concurrency to decouple the UI thread from the timing engine.
- **Data Parsing & Generation**: Transforming abstract move inputs into standardized, universally recognizable PGN structures.
- **Responsive UI/UX**: Built entirely in **SwiftUI**, maintaining 60FPS animations even when you're furiously slapping the clock in a time scramble.

---

## 🚀 Getting Started

### Prerequisites
- Xcode 14.0 or newer
- iOS 16.0+ device or simulator

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/amayIIp/ClockMate.git
   ```
2. Open `ClockMate.xcodeproj` in Xcode.
3. Select your target device/simulator and hit `Cmd + R` to build and run.

---

## 🔮 Future Roadmap (When time permits)

- **Computer Vision Integration:** Why even tap a screen? Just point the camera at the board and let ML figure out the moves.
- **Direct Cloud Sync:** Instantly sync games to Lichess or Chess.com for post-game analysis.

---

## 📄 License

This project is for educational purposes. Feel free to use the code, just promise me you won't use it to cheat.
