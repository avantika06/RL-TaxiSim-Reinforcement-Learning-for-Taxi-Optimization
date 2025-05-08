  

# RL-TaxiSim: Reinforcement Learning for Taxi Optimization  

## **Overview**  
RL-TaxiSim is a reinforcement learning project that explores various RL algorithms to optimize taxi navigation in a simulated city grid. Using OpenAI Gym's **Taxi-v3** environment, the project implements **Q-Learning, SARSA, and Deep Q-Networks (DQN)** to train an intelligent agent that efficiently picks up and drops off passengers while maximizing rewards.  

## **Motivation**  
Real-world taxi operations involve **dynamic decision-making, efficiency optimization, and route planning**. This project aims to:  
- Experiment with different reinforcement learning strategies.  
- Compare performance metrics like convergence speed and reward accumulation.  
- Identify the best RL algorithm for optimizing navigation tasks in structured grid environments.  

## **Features**  
✔️ **Implemented RL Algorithms:** Q-Learning, SARSA, and Deep Q-Networks (DQN).  
✔️ **State & Action Space:** 500 discrete states, 6 possible actions (move, pick-up, drop-off).  
✔️ **Reward System:** +20 for successful drop-offs, -1 per step to encourage efficiency, -10 for illegal actions.  
✔️ **Performance Evaluation:** Algorithm comparison based on learning speed and reward optimization.  

## **Technologies Used**  
- **Python** (NumPy, Matplotlib)  
- **OpenAI Gym (Gymnasium)** for Taxi-v3 simulation  
- **TensorFlow/Keras** for Deep Q-Network (DQN) implementation  
- **Reinforcement Learning Techniques:**  
  - **Q-Learning:** Off-policy learning with Q-table updates  
  - **SARSA:** On-policy learning with safer exploration  
  - **Deep Q-Network (DQN):** Neural network-based function approximation  

## **Installation & Setup**  
### **1. Install Dependencies**  
```bash
pip install numpy matplotlib gymnasium tensorflow
```
### **2. Run Training**  
```bash
python train.py  # Trains Q-Learning, SARSA, and DQN models
```
### **3. Run Evaluation**  
```bash
python evaluate.py  # Tests trained models on new episodes
```

## **Results & Analysis**  
- **DQN outperformed** both Q-Learning and SARSA, achieving faster convergence (~2000 episodes).  
- **SARSA was more stable** but learned slower (~2500 episodes).  
- **Q-Learning required the most episodes (~3000) to stabilize**, due to its aggressive exploration strategy.  

## **Future Enhancements**  
🔹 **Implement Double DQN & Dueling DQN** for improved convergence.  
🔹 **Introduce multi-agent learning** for simulating multiple taxis in a shared environment.  
🔹 **Extend to real-world taxi routing problems** using GPS and traffic data.  

