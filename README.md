# Facility Location Optimization using Gurobi

## Key Features

- ✔ Mixed Integer Linear Programming (MILP)
- ✔ Facility Location Optimization
- ✔ Binary Facility Selection
- ✔ Transportation Network Optimization
- ✔ Sensitivity Analysis
- ✔ Network Visualization
- ✔ Python + Gurobi Implementation

## Overview

This project presents a Mixed Integer Linear Programming (MILP) model for a multi-echelon facility location problem. The objective is to determine the optimal product flow from factories to warehouses and from warehouses to customers while minimizing total logistics cost.

The model is implemented in Python using Gurobi and includes sensitivity analysis and network visualization.

---

## Problem Statement

A company operates:

- 3 factories
- 5 warehouses
- 10 customer locations

The objective is to minimize:

- Factory-to-warehouse transportation cost
- Warehouse-to-customer transportation cost
- Warehouse fixed operating cost

subject to:

- Factory capacity constraints
- Warehouse capacity constraints
- Customer demand satisfaction
- Flow balance constraints

---

## Mathematical Formulation

### Decision Variables

- `x[i,j]`: Quantity transported from factory *i* to warehouse *j*
- `y[j,k]`: Quantity transported from warehouse *j* to customer *k*
- `z[j]`: Binary variable indicating whether warehouse *j* is opened

### Objective

Minimize the total logistics cost consisting of transportation and warehouse fixed operating costs.

### Constraints

- Factory capacity
- Warehouse capacity
- Demand satisfaction
- Flow conservation
- Binary warehouse opening decisions

---

## Technologies Used

- Python
- Gurobi Optimizer
- pandas
- NumPy
- matplotlib
- NetworkX
- Jupyter Notebook

---

## Results

The optimization model determines:

- Optimal warehouse locations
- Optimal shipment quantities
- Minimum total logistics cost

---

## Sensitivity Analysis

### Warehouse Capacity

Warehouse capacities were varied to evaluate their impact on the network configuration.

Observation:

- Increasing warehouse capacity reduced the number of warehouses required.
- Larger capacities enabled network consolidation and reduced total logistics cost.

### Fixed Cost

Warehouse fixed operating costs were varied.

Observation:

- The optimal warehouse configuration remained unchanged over the tested range.
- Transportation and capacity constraints dominated the facility selection decisions.

### Factory Capacity

Factory capacities were varied.

Observation:

- Capacity reductions below a threshold resulted in infeasible solutions.
- Factory production capacity is a critical feasibility constraint.
---

## Future Improvements

- Multi-period planning
- Stochastic demand
- Carbon emission constraints
- Multi-objective optimization
- Inventory decisions

---

## Author

**Swati Pattanaik**

Ph.D. in Industrial and Systems Engineering

Research Interests:
- Operations Research
- Supply Chain Optimization
- Machine Learning
- Digital Twins
- Industrial AI
