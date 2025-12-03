# Reinforcement Learning — Lab 2  
### Stochastic Shortest Path (Wireless Routing Environment)

This project implements and analyzes a **Stochastic Shortest Path (SSP)** problem modeled as a **grid-based wireless routing network**.  
The goal is to understand how fixed policies behave under stochastic transitions, how to evaluate them using both **linear policy evaluation** and **Monte Carlo methods**, and how to compute the **optimal value function** and **optimal policy** using **Value Iteration**.

---

## **Overview of Tasks**

### **Task 1 — Identify the MDP**
- Explore stochastic transition probabilities for different state–action pairs.
- Visualize transitions (e.g., from state (2,2) taking action ‘U’).
- Interpret the meaning of slip probabilities and “stay in place” transitions.

### **Task 2 — Evaluate Fixed Policies (Linear System)**
- Policy 1: Always go Right (`R`)
- Policy 2: Always go Down (`D`)
- Solve the Bellman equations using a linear system to compute the value function.
- Visualize heatmaps of value functions.

### **Task 3 — Monte Carlo Evaluation & Trajectories**
- Simulate episodes under fixed policies.
- Compute:
  - average return  
  - mean number of steps  
  - success rate  
- Compare Monte Carlo estimates with theoretical values from Task 2.
- Visualize trajectories and animations.

### **Task 4 — Value Iteration (Optimal Policy)**
- Compute the optimal value function \(V^*\)
- Derive the optimal policy via one-step lookahead
- Visualize the optimal policy and value heatmap
- Compare \(V^*(0,0)\) to fixed-policy values

---



##  **Key Concepts Demonstrated**

### **MDP Formulation**
- 5×5 grid
- Actions: {U, D, L, R}
- Stochastic dynamics with:
  - intended move probability
  - slip left/right
  - stay-in-place
- Reward: -1 per step, 0 at goal

### **Policy Evaluation**
- Solved linear system for deterministic policies
- Clear comparison between "Always Right" and "Always Down"

### **Monte Carlo Policy Evaluation**
- Empirical estimation of value by averaging returns
- Observed convergence to theoretical values

### **Value Iteration**
- Applied Bellman optimality updates
- Extracted optimal policy from \(V^*\)
- Demonstrated drastic improvement vs fixed policies

---

##  **Example Visualizations**

| Always Right | Always Down | Optimal Policy |
|--------------|-------------|----------------|
| ![](images/always_go_right_heatmap) | ![](images/always_go_down_heatmap.png) | ![](images/optimal_value_heatmap.png) |


---

##  Notes
This project was completed as part of the **Reinforcement Learning** course.  
It demonstrates understanding of MDPs, dynamic programming, Monte Carlo methods, and optimal control.
