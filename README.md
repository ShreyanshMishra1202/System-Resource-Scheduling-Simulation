<div align="center">

# 🚀 System Resource Scheduling Simulation

### *A Comprehensive Priority-Based Resource Scheduling Simulator*

[![GitHub Stars](https://img.shields.io/github/stars/ShreyanshMishra1202/System-Resource-Scheduling-Simulation?style=for-the-badge&logo=github)](https://github.com/ShreyanshMishra1202/System-Resource-Scheduling-Simulation/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/ShreyanshMishra1202/System-Resource-Scheduling-Simulation?style=for-the-badge&logo=github)](https://github.com/ShreyanshMishra1202/System-Resource-Scheduling-Simulation/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/ShreyanshMishra1202/System-Resource-Scheduling-Simulation?style=for-the-badge&logo=github)](https://github.com/ShreyanshMishra1202/System-Resource-Scheduling-Simulation/issues)
[![License](https://img.shields.io/github/license/ShreyanshMishra1202/System-Resource-Scheduling-Simulation?style=for-the-badge)](LICENSE)

---

</div>

## 📋 Overview

**System Resource Scheduling Simulation** is a sophisticated, time-driven simulation framework designed to model and analyze how multiple independent agents compete for shared resources. This project provides deep insights into scheduling behavior, system state transitions, and resource feasibility under constrained conditions.

🎯 **Key Focus**: Accurate system modeling and intelligent decision logic, prioritizing correctness over UI aesthetics or domain-specific physical accuracy.

---

## 🏗️ Architecture & System Model

The simulation architecture comprises four core components working in harmony:

| Component | Description |
|-----------|-------------|
| 🤖 **Multiple Agents** | Independent entities competing for resources |
| 💎 **Shared Resource** | Single critical resource accessed by agents |
| ⚙️ **Intelligent Scheduler** | Decision-making engine for resource allocation |
| ⏱️ **Time Progression** | Discrete time-step simulation mechanism |

**Workflow**: Agents become eligible for service based on dynamic availability conditions. When the resource is idle, the scheduler intelligently selects one eligible agent for execution.

---

## 🎯 Scheduling Policy

Our system implements **Non-Preemptive Priority-Based Scheduling** for optimal resource allocation:

```
┌─────────────────────────────────────────────────────┐
│  Scheduling occurs ONLY when resource is idle       │
│  Selected agent runs to completion (no interruption)│
│  Fixed execution window ensures predictability      │
└─────────────────────────────────────────────────────┘
```

✨ **Key Characteristics**:
- 🔒 Non-preemptive execution
- 📊 Priority-based selection
- ⏰ Fixed-time execution windows
- ✅ Run-to-completion guarantee

---

## 🔄 System States

The system operates in two distinct states with clear transitions:

### 🟢 Idle State
```
┌─────────────────────┐
│ ✓ Resource is free  │
│ ✓ No agent running  │
│ ✓ Scheduling active │
└─────────────────────┘
```

### 🔴 Busy State
```
┌──────────────────────┐
│ ✓ Resource occupied  │
│ ✓ One agent running  │
│ ✓ No re-selection    │
└──────────────────────┘
```

---

## 📐 System Assumptions

Our simulation is built on the following foundational principles:

| Assumption | Description |
|------------|-------------|
| ⏱️ **Discrete Time** | Time progresses in discrete simulation steps |
| 🔐 **Exclusive Access** | Only one agent can use the resource at any time |
| 📏 **Fixed Duration** | Execution duration is fixed and deterministic |
| 🎲 **Logical Availability** | Agent availability is abstracted using logical conditions |
| 🚫 **No Preemption** | Scheduling is strictly non-preemptive |  

---

## 🛡️ System Invariants

These invariants guarantee system correctness and consistency:

```
✓ At most one agent executes at any time
✓ Scheduling occurs only in the idle state
✓ Execution always runs to completion
✓ System state remains consistent across time steps
```  

---

## 🎨 Design Philosophy (Phase-1)

<div align="center">

### *Correctness First, Optimization Later*

</div>

**Phase-1 Priorities**:
- ✅ **Correctness**: Accurate system behavior and state management
- 🔍 **Clear Separation**: Distinct decision and execution phases
- 🔄 **Consistency**: Robust state management across time steps
- 📊 **Foundation**: Solid base for future enhancements

> **Note**: Performance analysis and fairness improvements are planned for subsequent phases.

---

## ⚠️ Known Limitations

| Limitation | Description | Status |
|------------|-------------|---------|
| 🔄 **Starvation Risk** | Static priority scheduling may cause starvation | Future mitigation planned |
| 🎯 **Behavioral Focus** | Model optimized for behavior analysis, not physical accuracy | By design |  

---

## 🚀 Future Extensions

Exciting features planned for upcoming releases:

### Phase 2 & Beyond
```
📊 Metrics Collection
   └─ Resource utilization analysis
   └─ Performance benchmarking
   └─ System efficiency tracking

🔧 Starvation Mitigation
   └─ Age-based priority adjustment
   └─ Fairness algorithms
   └─ Dynamic priority modification

📈 Comparative Analysis
   └─ Multiple scheduling strategies
   └─ Performance comparisons
   └─ Trade-off analysis
```

---

## 🤝 Contributing

Contributions are welcome! Whether it's bug reports, feature requests, or code contributions, we appreciate your help in making this project better.

1. 🍴 Fork the repository
2. 🔨 Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🎉 Open a Pull Request

---

## 📜 License

This project is open source and available under the appropriate license. See the `LICENSE` file for more details.

---

## 👨‍💻 Author

**Shreyansh Mishra**

- GitHub: [@ShreyanshMishra1202](https://github.com/ShreyanshMishra1202)

---

<div align="center">

### ⭐ Star this repository if you find it useful!

**Made with ❤️ and ☕**

</div>  
