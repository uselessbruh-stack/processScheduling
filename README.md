# ⏱️ CPU Scheduling Simulator

An interactive educational dashboard to visualize and understand CPU scheduling algorithms with animated Gantt charts and real-time metrics. Perfect for learning operating systems concepts!

![React](https://img.shields.io/badge/React-19.0-61DAFB?logo=react)
![Vite](https://img.shields.io/badge/Vite-6.2-646CFF?logo=vite)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.1-38B2AC?logo=tailwindcss)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## ✨ Features

### 📊 Supported Algorithms
- **FCFS** (First Come, First Served) – Processes execute in arrival order
- **SJF** (Shortest Job First) – Non-preemptive, shortest job first
- **SRTF** (Shortest Remaining Time First) – Preemptive, always run shortest remaining job
- **Priority Scheduling** – Execute based on process priority
- **Round Robin** – Time-quantum based fair scheduling
- **Multilevel Queue** – Multiple queues with different priorities

### 🎯 Application Features
- **Animated Gantt Charts** – Visual timeline of process execution with smooth animations
- **Real-time Metrics** – Calculate and display:
  - Average Waiting Time
  - Average Turnaround Time
  - CPU Utilization
  - Context Switches
- **Step-by-Step Execution** – Execute scheduling one step at a time for better understanding
- **Custom Process Input** – Add processes with custom arrival time, burst time, and priority
- **Random Generation** – Generate random process sets for testing
- **Responsive Design** – Works seamlessly on desktop and tablet devices
- **Interactive UI** – Intuitive controls and real-time feedback
- **Dark Mode Support** – Eye-friendly theme options

---

## 🚀 Quick Start

### Prerequisites
- Node.js 16+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/process-scheduling.git
cd processScheduling

# Install dependencies
npm install
```

### Development

```bash
# Start development server
npm run dev

# App will be available at http://localhost:5173
```

### Build

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

---

## 📁 Project Structure

```
processScheduling/
├── src/
│   ├── components/           # React components
│   │   ├── ProcessInput.jsx
│   │   ├── GanttChart.jsx
│   │   ├── Metrics.jsx
│   │   └── AlgorithmSelector.jsx
│   ├── algorithms/           # Scheduling algorithm implementations
│   │   ├── fcfs.js
│   │   ├── sjf.js
│   │   ├── srtf.js
│   │   ├── priority.js
│   │   ├── roundRobin.js
│   │   └── multiLevelQueue.js
│   ├── hooks/                # Custom React hooks
│   ├── styles/               # Tailwind CSS configuration
│   ├── App.jsx               # Main application component
│   └── main.jsx              # Entry point
├── public/                   # Static assets
├── dist/                     # Production build (generated)
├── package.json              # Dependencies & scripts
├── vite.config.js            # Vite configuration
├── tailwind.config.js        # Tailwind CSS configuration
├── README.md                 # This file
├── LICENSE                   # MIT License
└── .gitignore                # Git ignore rules
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **React 19** | UI library & state management |
| **Vite 6.2** | Ultra-fast build tool |
| **Tailwind CSS 4.1** | Utility-first CSS framework |
| **Framer Motion 11.18** | Smooth animations for Gantt charts |
| **npm** | Package manager |

---

## 📖 How to Use

### 1. **Select Algorithm**
   - Choose from the dropdown menu (FCFS, SJF, SRTF, etc.)

### 2. **Add Processes**
   - Manually enter processes with:
     - **Process ID** (P1, P2, etc.)
     - **Arrival Time** (when process arrives in queue)
     - **Burst Time** (CPU time needed)
     - **Priority** (for priority scheduling)
   - Or use **Random Generate** button

### 3. **Execute Simulation**
   - Click **Start** to run the entire simulation
   - Or click **Step** to execute one step at a time

### 4. **View Results**
   - **Gantt Chart** – Visual timeline of execution
   - **Metrics Panel** – Waiting time, turnaround time, etc.
   - **Process Table** – Details of each process

### 5. **Export/Reset**
   - Reset simulation to try different parameters
   - Export results (optional feature)

---

## 📊 Scheduling Metrics Explained

| Metric | Definition |
|--------|-----------|
| **Waiting Time** | Time process spends waiting in queue |
| **Turnaround Time** | Total time from arrival to completion |
| **Average Waiting Time** | Mean of all processes' waiting times |
| **Average Turnaround Time** | Mean of all processes' turnaround times |
| **CPU Utilization** | Percentage of time CPU is busy |
| **Context Switches** | Number of times CPU switches between processes |

---

## 🎓 Educational Value

This simulator helps students and professionals understand:
- ✅ How different scheduling algorithms work
- ✅ Trade-offs between algorithms (fairness vs efficiency)
- ✅ Impact of scheduling on system performance
- ✅ Real-world CPU scheduling decisions
- ✅ Operating system fundamentals

---

## 💡 Features to Implement

- [ ] Multiple queue scheduling visualization
- [ ] I/O operations simulation
- [ ] Priority inversion handling
- [ ] Export simulation as report/PDF
- [ ] Performance comparison between algorithms
- [ ] Custom algorithm builder
- [ ] Preset workload templates

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 📧 Support

For issues, questions, or suggestions, please open an [issue on GitHub](https://github.com/your-username/process-scheduling/issues).

---

## 🔗 Resources

- [Operating Systems Concepts](https://www.amazon.com/Operating-System-Concepts-Abraham-Silberschatz/dp/1119456339/)
- [CPU Scheduling Algorithms](https://en.wikipedia.org/wiki/Scheduling_(computing))
- [React Documentation](https://react.dev)
- [Vite Documentation](https://vitejs.dev)

---

**Built with ❤️ for OS enthusiasts and students**

## Setup

**Prerequisites:** [Node.js](https://nodejs.org/) (v18 or later)

```bash
# 1. Install dependencies
npm install

# 2. Start dev server
npm run dev
```

Open `http://localhost:5173` in your browser.

## Usage

1. Select a scheduling algorithm from the dropdown menu
2. Add processes either:
   - Manually by entering Arrival Time and Burst Time
   - Click **🎲 Random** to generate random processes
3. Click **▶ Start** to run the simulation
4. Use **Step Mode** for step-by-step execution to understand the algorithm
5. View the Gantt chart and metrics in real-time

## Building for Production

```bash
npm run build
```

The optimized build will be output to the `dist` folder.

## Learning Objectives

This simulator helps understand:
- How different CPU scheduling algorithms work
- The impact of scheduling on system performance
- Metrics like average waiting time and turnaround time
- Trade-offs between different scheduling strategies

## License

This project is licensed under the MIT License - see the LICENSE file for details.
