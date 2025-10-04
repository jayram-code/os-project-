# os-project-
 Interactive browser game teaching OS process scheduling concepts. Click to dispatch processes from Ready Queue to CPU while minimizing latency. Features combo system, difficulty ramping, and futuristic dark theme. Built with vanilla HTML/CSS/JavaScript.
#  OS Dispatcher Game - Interactive CPU Scheduler Simulator
<img width="1297" height="689" alt="image" src="https://github.com/user-attachments/assets/5adf5741-ea76-4806-b7dc-ab1ccdb82564" />


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

An immersive, futuristic browser game that teaches Operating System concepts through interactive gameplay. Experience what it's like to be an OS Dispatcher managing process scheduling in real-time!

[ Play Now](#installation) | [Learn More](#educational-objectives) | [Contribute](#contributing)

---

## Features

### Core Gameplay
- **Real-time Process Management**: Dispatch processes from Ready Queue to CPU
- **Dispatch Latency Tracking**: Measure and optimize your reaction time
- **Dynamic Scoring System**: Earn points for fast dispatches, lose points for delays
- **60-Second Challenge**: Test your skills in time-limited gameplay

### Advanced Mechanics
- **Combo Bonus System**: Chain 3+ fast dispatches (&lt;2s) for explosive bonus points
- **Visual Effects**: Stunning particle trails, glowing animations, and screen shake
- **Difficulty Ramping**: Process spawn rate increases from 3-6s to 1-4s intervals
- **Warning System**: "TOO SLOW!" alerts for >5s latency with visual feedback

### Futuristic Design
- **Dark Cyber Theme**: Neon colors and animated grid background
- **Smooth Animations**: Cubic-bezier transitions and particle effects
- **Responsive Layout**: Works seamlessly on desktop, tablet, and mobile
- **Color-Coded Priorities**: High (red), Normal (green), Low (orange) processes

---

## Educational Objectives

This game teaches fundamental Operating System concepts:

### **Process Scheduling**
- Understanding the **Ready Queue** where processes wait for CPU time
- Learning about **process states**: Ready → Running → Completed
- Visualizing **context switching** between processes

### **Dispatch Latency**
- Definition: Time delay between process arrival and CPU dispatch
- Real-world impact on system performance
- Trade-offs between latency and throughput

### **Dispatcher Role**
- The dispatcher is responsible for:
  - Switching context from one process to another
  - Switching to user mode
  - Jumping to the proper location in the user program
- Minimizing **dispatch latency** is critical for system responsiveness

### **Performance Metrics**
- Average latency calculation
- Score optimization strategies
- Understanding fast-path vs. slow-path dispatching

---

## How to Play

### **Objective**
Keep the average dispatch latency as low as possible while maximizing your score!

### **Controls**
1. Click **START GAME** to begin the 60-second challenge
2. **Click on processes** in the Ready Queue to dispatch them to CPU
3. Watch as processes execute and move to Completed area
4. Build combos by dispatching 3+ processes quickly (&lt;2s each)

### **Scoring Rules**

| Latency | Result | Points |
|---------|--------|--------|
| **< 2 seconds** |  FAST! | +40 to +50 points |
| **2-5 seconds** |  OK | +10 to +25 points |
| **> 5 seconds** |  TOO SLOW! | -20+ points (penalty) |
| **3+ Combo** |  COMBO BONUS! | +25 per combo level |

### **Performance Ranks**
-  **Legendary Dispatcher**: &lt;1.5s avg, 5+ max combo
-  **Exceptional**: &lt;2.0s avg, 3+ max combo
-  **Excellent**: &lt;2.5s avg
-  **Good**: &lt;3.5s avg
-  **Needs Improvement**: >3.5s avg

---

##  Installation

### **Option 1: Direct Download**
```bash
# Clone the repository
git clone https://github.com/yourusername/os-dispatcher-game.git

# Navigate to the project directory
cd os-dispatcher-game

# Open index.html in your browser
# (Double-click the file or use a local server)
```

### **Option 2: Live Server (Recommended)**
```bash
# Using Python
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Then open: http://localhost:8000
```

### **Option 3: Online Platforms**
- Upload to **GitHub Pages** for instant hosting
- Deploy to **Netlify** or **Vercel** with one click
- Use **CodeSandbox** or **Replit** for online editing

---

##  Technologies Used

- **HTML5**: Semantic structure and canvas elements
- **CSS3**: Advanced animations, gradients, and responsive design
- **Vanilla JavaScript**: Pure JS with OOP design patterns
- **No Dependencies**: Zero external libraries required!

---

##  Game Architecture

### **Class Structure**
```javascript
class OSDispatcherGame {
  - Process spawning system
  - Dispatch latency calculation
  - Combo tracking logic
  - Score management
  - Visual effects engine
  - Difficulty scaling algorithm
}
```

### **Process States**
```
[New Process] → [Ready Queue] → [CPU Execution] → [Completed]
     ↓              ↓                 ↓                ↓
  Created      Waiting for       Running on        Finished
              Dispatcher           CPU Core
```

---

##  Learning Resources

Want to learn more about OS concepts?

- [Operating System Concepts (Silberschatz)](https://www.os-book.com/)
- [MIT OpenCourseWare: Operating Systems](https://ocw.mit.edu/)
- [GeeksforGeeks: Process Scheduling](https://www.geeksforgeeks.org/cpu-scheduling-in-operating-systems/)
- [Process Scheduling Algorithms](https://en.wikipedia.org/wiki/Scheduling_(computing))

---

##  Contributing

Contributions are welcome! Here are some ideas:

### **Enhancement Ideas**
- [ ] Add multiple CPU cores (multiprocessor scheduling)
- [ ] Implement different scheduling algorithms (FCFS, SJF, Round Robin)
- [ ] Add process priority levels that affect scoring
- [ ] Create difficulty modes (Easy, Medium, Hard)
- [ ] Add sound effects and background music
- [ ] Implement leaderboard with local storage
- [ ] Add tutorial mode for beginners
- [ ] Create mobile touch controls optimization

### **How to Contribute**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

##  Code Style

This project follows clean code principles:
- ✅ Comprehensive comments explaining OS concepts
- ✅ Clear variable naming conventions
- ✅ Modular, reusable functions
- ✅ Object-oriented design patterns
- ✅ No external dependencies for easy understanding

---

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

---

##  Acknowledgments

- Inspired by Operating System course materials
- Design influenced by cyberpunk aesthetics
- Built for educational purposes to make OS concepts fun and interactive
- Thanks to all contributors and players!

---

##  Contact & Support

-  **Found a bug?** [Open an issue](https://github.com/yourusername/os-dispatcher-game/issues)
-  **Have an idea?** [Start a discussion](https://github.com/yourusername/os-dispatcher-game/discussions)
-  **Like the project?** Give it a star!

---

##  Quick Start Summary

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/os-dispatcher-game.git

# 2. Open index.html in your browser
cd os-dispatcher-game
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux

# 3. Start playing and learning!
```

---

<div align="center">

###  Made with  for Computer Science Students

**[⬆ Back to Top](#-os-dispatcher-game---interactive-cpu-scheduler-simulator)**

</div>
