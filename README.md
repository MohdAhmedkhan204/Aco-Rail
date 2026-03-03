# Aco-Rail
ACO-ML PrecisionRail HSR
Ant Colony Optimization & ML for Accurate Train Positioning
Aim:
The primary aim of this project is to modernize the positioning and navigation systems of the Indian Railway (IR) network for High-Speed Rail (HSR) corridors. By leveraging Ant Colony Optimization (ACO) and Machine Learning, the system provides a fail-safe mechanism that maintains sub-meter accuracy even when traditional sensors encounter failures.
Objective:
   . Hybrid Trajectory Management: To build a system that seamlessly switches from Traditional GPS tracking to ACO-driven logic during signal loss or sensor failure.
   . Path Integrity: To treat the physical railway tracks as "Pheromone Constraints," ensuring the train never drifts from the digital twin of the iron rails.
   . Indian Railway Localization: To apply these advanced algorithms specifically to the complex geometry of Indian rail junctions and stations using real-world coordinate data from provided datasets.

   
Task:
   . Network Modeling: Utilize the train_network_project_30.csv dataset to construct a mathematical Graph where Stations represent Nodes and Tracks represent Edges.
   . Failure Simulation: Program a Trigger Event where the Traditional train loses its positioning accuracy, simulating a hardware breakdown, sensor error, or signal interference.
   . Autonomous Recovery: Design the ACO algorithm to activate upon failure, identifying the Pheromone Optimal Path to the next station to recover lost time and stabilize positioning.
   . Comparative Visualization: Build a Real-Time Dashboard to contrast the Delayed/Failed Traditional Path against the Optimized ACO Recovery Path.

   
Failure & Recovery Logic:
This project introduces a Smart-Switch architecture:
   . Scenario A (Traditional Failure): When a sensor failure occurs, the train follows a non-optimized, noisy path. This results in significant time loss and positioning drift (The Longer Path).
   . Scenario B (ACO Fix): Upon detecting the same failure, the system triggers the ACO ML Optimizer. It recalculates the velocity and trajectory based on track pheromones, finding the shortest time-path back to the destination (The Optimized Path).

   
Expected Result:
   . Time Efficiency: In failure scenarios, the ACO-enhanced train is expected to reach the destination 20-30% faster than the traditional fallback method.
   . Sub-Meter Precision: While the traditional failure path shows high variance and drift, the ACO-ML path converges onto the verified track geometry.
   . Optimal Delay Resolution: The system will demonstrate that ML-driven pathfinding is the most effective solution for minimizing the impact of unforeseen technical failures in high-speed rail environments.
