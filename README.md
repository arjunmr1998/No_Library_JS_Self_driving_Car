# Self-Driving Car Simulation in JavaScript

A self-driving car simulation built completely from scratch using vanilla JavaScript and HTML5 Canvas.

The project demonstrates how autonomous driving behavior can emerge through a simple neural network combined with evolutionary optimization. No machine learning libraries or frameworks were used.

## Demo

The simulation trains multiple cars in parallel and continuously evolves the neural network weights and biases. Over successive generations, the best-performing vehicle learns how to navigate traffic while avoiding collisions.

<img src="Single_car_autonomus.gif" width="500">
---

## Features

- Feedforward Neural Network implemented from scratch
- Genetic Algorithm based learning and mutation
- Ray-casting sensors for environment perception
- Collision detection using polygon intersections
- Traffic simulation with autonomous and non-autonomous vehicles
- Real-time neural network visualization
- Local storage support for saving the best-performing brain
- Pure JavaScript implementation (no external libraries)

---

## How It Works

### 1. Sensors

Each car uses multiple ray-casting sensors to detect:

- Road boundaries
- Other vehicles
- Distance to obstacles

The sensor readings become inputs to the neural network.

### 2. Neural Network

The neural network receives sensor data and predicts:

- Move Forward
- Turn Left
- Turn Right
- Reverse

### 3. Evolution

Instead of backpropagation, this project uses evolutionary learning:

1. Generate many cars
2. Select the best performer
3. Save its neural network
4. Create mutated copies
5. Repeat

Over time, driving behavior improves automatically.

---

## Technologies Used

- JavaScript (ES6)
- HTML5 Canvas
- CSS3

No external frameworks or machine learning libraries were used.

---

## Project Structure

```
├── index.html
├── style.css
├── main.js
├── car.js
├── control.js
├── road.js
├── sensor.js
├── network.js
├── visualizer.js
└── utils.js
```

---

## Learning Outcomes

This project helped me understand:

- Neural Networks
- Genetic Algorithms
- Autonomous Vehicle Fundamentals
- Collision Detection
- Sensor Modeling
- Simulation Development
- Browser Graphics using Canvas

---

## Acknowledgements

This project was inspired by the excellent tutorial series by Radu Mariescu-Istodor:

https://www.youtube.com/watch?v=Rs_rAxEsAvI

The implementation was written independently while following the concepts presented in the tutorial.


## Future Improvements

- Reinforcement Learning (Q-Learning / Deep RL)
- Improved Traffic Behavior
- Vehicle Dynamics Model
- Lane Changing Logic
- Obstacle Prediction
- Advanced Sensor Models

