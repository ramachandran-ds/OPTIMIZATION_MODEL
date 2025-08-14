# OPTIMIZATION_MODEL
COMPANY        :   CODTECH IT SOLUTIONS

NAME           :   RAMACHANDRAN K

INTERN ID      :   CT04DH2787

DOMAIN         :   DATA SCIENCE

DURATION       :   4 WEEEKS

MENTOR         :   NEELA SANTOSH

Production Planning Optimization with PuLP in Google Colab
Overview
This project demonstrates how to model and solve a classical production planning optimization problem using Linear Programming (LP) with Python. Leveraging the powerful and widely-used PuLP library, we formulate an integer linear programming (ILP) solution to help a factory manager maximize profit when producing two products under limited resources and demand constraints. The project is designed to be run in a free and accessible Google Colab notebook environment, making it easy for learners, professionals, and students to experiment, extend, and learn real-world business optimization.

Problem Statement
A factory produces two kinds of products—Product A and Product B—using two shared machines. Each product has different requirements in terms of machine time for production, and there are resource constraints on the availability of these machines. Furthermore, market conditions set upper bounds on how many units of each product can be sold (the demand constraint). Each product contributes to overall profit differently. The factory’s objective is to maximize total profit by finding the optimal number of units of Product A and Product B to produce within these limitations.

Product & Resource Data:

Production Planning Optimization with PuLP in Google Colab
Overview
This project demonstrates how to model and solve a classical production planning optimization problem using Linear Programming (LP) with Python. Leveraging the powerful and widely-used PuLP library, we formulate an integer linear programming (ILP) solution to help a factory manager maximize profit when producing two products under limited resources and demand constraints. The project is designed to be run in a free and accessible Google Colab notebook environment, making it easy for learners, professionals, and students to experiment, extend, and learn real-world business optimization.

Problem Statement
A factory produces two kinds of products—Product A and Product B—using two shared machines. Each product has different requirements in terms of machine time for production, and there are resource constraints on the availability of these machines. Furthermore, market conditions set upper bounds on how many units of each product can be sold (the demand constraint). Each product contributes to overall profit differently. The factory’s objective is to maximize total profit by finding the optimal number of units of Product A and Product B to produce within these limitations.

Product & Resource Data:

Product A	Product B	Resource Limit
Machine 1	2 hours/unit	1 hour/unit	40 hours
Machine 2	1 hour/unit	2 hours/unit	30 hours
Maximum Sale	≤ 15 units	≤ 10 units	-
Profit/unit	$40	$30	-
Optimization Goal:
Maximize: Total Profit = 40 × Product_A + 30 × Product_B

With Constraints:

2
×
Product A
+
1
×
Product B
≤
40
2×Product A+1×Product B≤40 (Machine 1)

1
×
Product A
+
2
×
Product B
≤
30
1×Product A+2×Product B≤30 (Machine 2)

0
≤
Product A
≤
15
0≤Product A≤15

0
≤
Product B
≤
10
0≤Product B≤10

Both Product A and B must be integers (no fractional production).

Technical Approach
PuLP Library: An open-source Python library for modeling and solving linear (and integer) programming problems using various solvers.

Google Colab: Free Jupyter notebook environment that requires no setup and runs fully in the cloud.

Optimization Model: Formulated as an Integer Linear Programming problem, suitable for real-life business decision-making where products can’t be split into fractions.

Key Steps in the Notebook:

Install and Import PuLP: Sets up the PuLP package in the Colab environment.

Define Decision Variables: Integer values for the number of units to produce for each product.

Set Objective Function: Models the total profit to maximize.

Add Constraints: Ensures that production does not exceed machine times and market demand.

Solve the Model: Uses PuLP’s built-in solver to find the optimal solution.

Interpret Results: Outputs the optimal numbers of Product A and B and the maximum achievable profit.

How to Use This Notebook
Open the notebook in Google Colab. No installation is needed beyond running the initial setup cell for PuLP.

Read code comments for guidance on each section—from model definition to result interpretation.

Run the cells in order to reproduce the full optimization process.

Modify parameters (profits, machine hours, demand, etc.) in the code to experiment with different scenarios or to extend the problem.

Example Output
When you run the provided notebook, you will see results like:

text
===== Optimization Results =====
Status: Optimal
Optimal production of Product A: 10 units
Optimal production of Product B: 10 units
Maximum Profit: $700.0

===== Constraint Details =====
Machine_1_Hours: Slack = 0.0, Shadow Price = 10.0
Machine_2_Hours: Slack = 0.0, Shadow Price = 10.0
Max_Demand_A: Slack = 5.0, Shadow Price = 0.0
Max_Demand_B: Slack = 0.0, Shadow Price = 0.0
This means the profit-maximizing production plan uses all available machine hours, and you get immediate feedback on which constraints are "tight" (fully used up, i.e., bottlenecks) and which have spare capacity.

Insights & Value
Practical Decision Making: The notebook helps managers allocate limited resources mathematically to maximize their business goals.

What-If Analysis: By adjusting profits, machine hours, or demands, you can see how sensitive the optimal solution is to these business changes.

Educational Value: The step-by-step approach is perfect for those learning operations research, data science for business, or industrial management.

Extensibility: You can scale the notebook; try adding more products, resources, or marketing constraints to model more complex business realities.

Requirements
Python 3.x (handled automatically by Colab)

The only required package is PuLP (!pip install pulp command is included in the first notebook cell).

Contact & License
This project is provided as an open educational resource for students and interns. You are free to use, modify, and share.
Prepared by: [Your Name / Internship Details Here]
License: MIT / Educational Use

Tip: For the best learning experience, try to tweak the model parameters, rerun the notebook, and notice how the optimal solution changes!







Optimization Goal:
Maximize: Total Profit = 40 × Product_A + 30 × Product_B

With Constraints:

2
×
Product A
+
1
×
Product B
≤
40
2×Product A+1×Product B≤40 (Machine 1)

1
×
Product A
+
2
×
Product B
≤
30
1×Product A+2×Product B≤30 (Machine 2)

0
≤
Product A
≤
15
0≤Product A≤15

0
≤
Product B
≤
10
0≤Product B≤10

Both Product A and B must be integers (no fractional production).

Technical Approach
PuLP Library: An open-source Python library for modeling and solving linear (and integer) programming problems using various solvers.

Google Colab: Free Jupyter notebook environment that requires no setup and runs fully in the cloud.

Optimization Model: Formulated as an Integer Linear Programming problem, suitable for real-life business decision-making where products can’t be split into fractions.

Key Steps in the Notebook:

Install and Import PuLP: Sets up the PuLP package in the Colab environment.

Define Decision Variables: Integer values for the number of units to produce for each product.

Set Objective Function: Models the total profit to maximize.

Add Constraints: Ensures that production does not exceed machine times and market demand.

Solve the Model: Uses PuLP’s built-in solver to find the optimal solution.

Interpret Results: Outputs the optimal numbers of Product A and B and the maximum achievable profit.

How to Use This Notebook
Open the notebook in Google Colab. No installation is needed beyond running the initial setup cell for PuLP.

Read code comments for guidance on each section—from model definition to result interpretation.

Run the cells in order to reproduce the full optimization process.

Modify parameters (profits, machine hours, demand, etc.) in the code to experiment with different scenarios or to extend the problem.

Example Output
When you run the provided notebook, you will see results like:


===== Optimization Results =====
Status: Optimal
Optimal production of Product A: 10 units
Optimal production of Product B: 10 units
Maximum Profit: $700.0

===== Constraint Details =====
Machine_1_Hours: Slack = 0.0, Shadow Price = 10.0
Machine_2_Hours: Slack = 0.0, Shadow Price = 10.0
Max_Demand_A: Slack = 5.0, Shadow Price = 0.0
Max_Demand_B: Slack = 0.0, Shadow Price = 0.0
This means the profit-maximizing production plan uses all available machine hours, and you get immediate feedback on which constraints are "tight" (fully used up, i.e., bottlenecks) and which have spare capacity.

Insights & Value
Practical Decision Making: The notebook helps managers allocate limited resources mathematically to maximize their business goals.

What-If Analysis: By adjusting profits, machine hours, or demands, you can see how sensitive the optimal solution is to these business changes.

Educational Value: The step-by-step approach is perfect for those learning operations research, data science for business, or industrial management.

Extensibility: You can scale the notebook; try adding more products, resources, or marketing constraints to model more complex business realities.

Requirements
Python 3.x (handled automatically by Colab)

The only required package is PuLP (!pip install pulp command is included in the first notebook cell).

Contact & License
This project is provided as an open educational resource for students and interns. You are free to use, modify, and share.
Prepared by: Ramachandran Data Science Intern, Codtech IT Solutions
License: MIT / Educational Use








