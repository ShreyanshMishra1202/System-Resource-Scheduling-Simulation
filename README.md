# System-Level Simulation of Priority-Based Resource Scheduling

## Project Overview
This project implements a system-level, time-driven simulation in which multiple independent agents compete for a single shared resource. The objective is to study scheduling behavior, system states, and feasibility under constrained availability conditions. The focus is on correct system modeling and decision logic rather than UI or domain-specific physical accuracy.

## System Model
The system consists of multiple agents, a single shared resource, a scheduler, and a discrete time progression mechanism. Agents become eligible for service based on a dynamic availability condition. When the resource is idle, the scheduler selects one eligible agent for execution.

## Scheduling Policy
The system uses **non-preemptive priority-based scheduling**. Scheduling decisions occur only when the resource is idle. Once an agent is selected, it retains the resource for a fixed execution window and runs to completion without interruption.

## System States
**Idle**
- The resource is free
- No agent is executing
- Scheduling decisions are allowed

**Busy**
- The resource is occupied
- Exactly one agent is executing
- No re-selection occurs

## System Assumptions
- Time progresses in discrete simulation steps  
- Only one agent can use the resource at any time  
- Execution duration is fixed and deterministic  
- Agent availability is abstracted using logical conditions  
- Scheduling is non-preemptive  

## System Invariants
- At most one agent executes at any time  
- Scheduling occurs only in the idle state  
- Execution always runs to completion  
- System state remains consistent across time steps  

## Design Focus (Phase-1)
Phase-1 focuses on correctness of system behavior, clear separation of decision and execution phases, and consistent state management. Performance analysis and fairness improvements are handled in later phases.

## Known Limitations
- Starvation is possible under static priority scheduling  
- The model is intended for feasibility and behavior analysis, not physical accuracy  

## Future Extensions
- Metrics collection and resource utilization analysis  
- Starvation mitigation using aging  
- Comparative evaluation of scheduling strategies  
