# Hourly_Recommendation_Q_Learning

This repository contains the Household_energy_consumption dataset and a Jupyter Notebook **(`Hourly_Recommendation_Q_Learning.ipynb`)** that demonstrates the use of **Q-Learning** for building a recommendation system. The goal of this project is to design an agent that learns optimal actions over time and provides **hourly recommendations** based on reinforcement learning principles.

---

## 📖 Project Overview

Reinforcement Learning (RL) provides a powerful framework for sequential decision-making. In this project, **Q-Learning**, a model-free RL algorithm, is applied to build a system that learns recommendation strategies through trial and error.

Key aspects of the project include:

* Defining the environment, states, and actions.
* Implementing Q-Learning update rules.
* Training the agent to maximize cumulative rewards.
* Generating **hourly recommendations** based on the learned Q-table.

---

## 🔬 Methodology

### 1. Environment Setup

* **States:** Represent user contexts or time-based slots (e.g., hours of the day).
* **Actions:** Recommendation options available to the system.
* **Rewards:** Numerical feedback for actions taken in each state.

### 2. Q-Learning Algorithm

* Initialize Q-table with zeros.
* Update Q-values using the Bellman equation:

      Q(s, a) ← Q(s, a) + α [ r + γ max_a' Q(s', a') – Q(s, a) ]

* Apply **ε-greedy policy** for balancing exploration and exploitation.

### 3. Training

* Run episodes where the agent interacts with the environment.
* Continuously update Q-values to converge toward optimal policy.

### 4. Recommendation Generation

* After training, the learned Q-table is used to produce **recommendations on an hourly basis**.

---

## 📊 Results

* The agent successfully learns **time-based recommendation patterns**.
* Performance improves as the number of episodes increases, showing the effectiveness of reinforcement learning for recommendation tasks.
