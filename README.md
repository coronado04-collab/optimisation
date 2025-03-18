# Optimisation & Analytics Course
The main topics of this course were:

- Introduction to the modeling process in decision-making problems. This will include an overview of the different types of optimization and simulation models, as well as the steps involved in the modeling process.
- Linear models: modeling, applications, and the simplex method. This will cover how to formulate linear programming problems, how to solve them using the simplex method, and how to interpret the results.
- Discrete models: applications, binary variables, logical constraints, and algorithms. This will cover how to formulate discrete optimization problems, how to solve them using various algorithms, and how to interpret the results.
- Nonlinear models: applications, optimality conditions, and machine learning algorithms. This will cover how to formulate nonlinear programming problems, how to solve them using various algorithms, and how to interpret the results.
- Case studies. This will include real-world examples of how optimization and simulation models have been used to solve business problems.

## Case Study 1
Multi-period production planning and distribution for a pharmaceutical company. 

The company needs to optimize the production, storage, and distribution of **four products** (Painkillers, Antibiotics, Vaccines, and Antivirals) through a supply chain consisting of **three laboratories** (Leganes, Zaragoza, Malaga) and **four pharmacies** (Madrid, Barcelona, Sevilla and Valencia) over the period of one year divided in **four quarters** (Q1, Q2, Q3, Q4).

The **objective** is to minimize the total cost, which will be divided into:
- Production Cost. It is the cost related to the production of the different products in each laboratory.
- Storage Cost. Cost of storing products over a quarter in every different pharmacy. 
- Transportation. Cost related to the transportation between laboratories and pharmacies for each quarter.

Moreover, we need to take into account a series of **constraints** to make the problem more realistic: laboratories have limited production capacities, while the pharmacies have constrained storage capacities. Demand for each product must be met at every pharmacy in every quarter. The inventory levels are defined as the quantity of products left at the end of each quarter, which have to take into account local demand.

Taking into account all these considerations the challenge becomes determining: the best quantities of production at each laboratory, the transportation quantities between laboratories and pharmacies, and the inventory levels maintained at pharmacies. All these needs to be computed while also taking into account the current time period, which will finally result into a total of **304 variables**. 

At every moment a **Data Creation Logic** has been followed to obtain the csv files containing the problem data:
- Transportation costs vary depending on the distance between laboratories and pharmacies (i.e., the cost of transport between Leganes and Madrid is smaller than Leganes to Barcelona, for example)
- Pharmacies represent endpoints with limited storage, allowing us to implement logistic constraints. Bigger cities have more storage capacity.
- Laboratories can produce and supply different pharmacies but are limited by capacity.<br></br>

The main critical question that comes to our mind with this optimization model aims is:

**How should the company allocate production, inventory, and transportation resources over time to minimize costs while meeting demand and respecting capacity constraints?**

## Case Study 2
1. ### Optimization of Resource Allocation of a Social Network

This problem focuses on optimizing the operations of a social network platform by strategically allocating resources through the deployment of data centers and the efficient routing of user data between these centers and designated user regions through the course of four time periods, quarters. 

* Each data center incurs a fixed setup cost and has a defined maximum capacity for handling requests.

* Energy costs vary based on the data center's location, and they are proportional to the amount of data processed.

* User regions generate specific request loads that must be served in full for each quarter. Each region also has an associated priority level, reflecting its criticality to the platform's operations for the different time periods. 

The objective is to minimize the total operational costs, including the setup costs for activating data centers and the energy costs associated with data routing for each quarter of a year.

The model will therefore determine; which data centers to activate for cost-effective operations and the optimal routing schema to minimize energy costs while ensuring all user regions are satisfied.

2. ### Introduction to the Non-Linear Optimization Project

Traffic Optimization in Urban Networks: Balancing Demand and Efficiency

The efficient management of urban traffic networks is a critical challenge for minimizing travel time, reducing congestion, and improving overall mobility. This project focuses on modeling and solving a Traffic Assignment Problem (TAP) using non-linear optimization techniques. We consider a simplified realistic city network with multiple routes connecting origin-destination pairs.

The project contains the following elements:

1. **Wardrop's Principle of Equilibrium**: A foundational concept in traffic modeling, ensuring that no user can reduce their travel time by switching routes.
2. **Non-linear travel cost functions**: These functions realistically capture the effects of congestion, where travel times increase as road capacities are approached.
3. **Capacitated arcs and budget constraints**: These constraints add complexity and realism, accounting for limited road capacities and investment limitations for infrastructure upgrades.

The primary objective of this project is to minimize total travel time across the network while meeting travel demand and exploring cost-effective upgrades to road capacities. This involves balancing short-term operational efficiency with long-term infrastructure investment strategies. 

Through this assignment, we want to show the application of advanced optimization techniques to urban planning, making the way for more effective and data-driven traffic management strategies.



I really encourage you to take a look at the Jupyter Notebooks since all the explanations are there.

