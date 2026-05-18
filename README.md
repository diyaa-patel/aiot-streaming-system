# AIoT Streaming System

A PyTorch-based AIoT simulation that evaluates real-time MNIST classification under edge computing constraints. The project compares model size, inference speed, queue scheduling, edge/cloud offloading, latency, deadline misses, dropped samples, and Age of Information.

## Overview

This project simulates an AIoT system where sensor data continuously arrives and must be processed before it becomes stale. The system uses MNIST digit classification as the inference task and evaluates how different model sizes and scheduling policies affect real-time performance.

## Features

- MNIST-based sensor data generation
- Configurable sample arrival rates
- FIFO and LIFO queue scheduling
- Admission control for queue overflow
- Tiny, compressed, and full CNN model variants
- Simulated edge and cloud inference
- 50ms network latency emulation
- Dynamic edge/cloud offloading
- Accuracy, latency, deadline miss, drop rate, and Age of Information tracking
- Experiments under normal load, overload, LIFO, and high-rate scenarios

## Technologies Used

- Python
- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook
- Edge AI
- AIoT Simulation

## Results Summary

- The Tiny model handled normal load efficiently with high accuracy and no deadline misses.
- The Full model achieved high accuracy but overloaded under high arrival rates.
- LIFO scheduling reduced Age of Information compared to FIFO by prioritizing newer samples.
- The compressed model provided a strong balance between speed and accuracy for high-rate streaming.

## Report

[Project Report](COMP4436_Project_Report_PATEL_Diya.pdf)

## What I Learned

This project helped me understand real-time AI system trade-offs, including accuracy versus inference speed, freshness versus fairness, edge versus cloud inference, and how queue scheduling affects latency and data freshness.
