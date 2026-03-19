# ClockMate: The Over-The-Board Chess Digitizer

ClockMate isn't just another chess clock. It's an iOS app that tracks your remaining time to the millisecond while converting your over-the-board moves into a digital PGN file. No more scrambling to write down moves on a paper scorecard while your clock is ticking.

![Swift](https://img.shields.io/badge/Swift-5.x-FA7343?style=flat&logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-16.0+-000000?style=flat&logo=apple&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-UI-007AFF?style=flat)

---

## What It Does

*   **Real-Time PGN Generation:** Tracks every move and compiles a standard PGN file you can use in any chess engine. Great for looking at your blunders later.
*   **Millisecond Time Accuracy:** Custom state machine logic makes sure the clock is dead accurate.
*   **Clean Move Input UI:** Designed to be fast and distraction-free, even during a frantic bullet game.
*   **Full Game State Tracking:** Keeps a running history of the board state so it always knows whose turn it is.

## Under the Hood

*   **State Management:** Handling rapid user inputs while keeping a perfect chronometer required clean concurrency work. The timing engine runs independently from the UI thread.
*   **PGN Parsing:** Transforms abstract move inputs into standardized PGN notation that any chess engine can read.
*   **SwiftUI Performance:** Built entirely in SwiftUI, holding 60fps even when you're frantically tapping the clock.

---

## Getting Started

### What You Need
*   Xcode 14.0 or newer
*   iOS 16.0+ device or simulator

### Setup
1.  Clone this repo:
    ```bash
    git clone https://github.com/amayIIp/ClockMate.git
    ```
2.  Open `ClockMate.xcodeproj` in Xcode.
3.  Pick your target device and hit `Cmd + R`.

---

## What's Next

*   **Computer Vision:** Eventually I want to point a camera at the board and have the app figure out the moves automatically.
*   **Cloud Sync:** Push finished games directly to Lichess or Chess.com for post-game analysis.

---

## License

This project is for educational purposes. Feel free to use the code, just don't use it to cheat.
