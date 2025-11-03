# Optimization-and-Scheduling-of-Multi-Machine-Production-Systems-Using-Excel
Excel was used to optimize production cost and scheduling efficiency. Solver minimized total cost by optimally assigning product units across machines. Pivot Tables, Charts, and Slicers analyzed machine utilization and cost. Johnson’s Rule with VLOOKUP sequenced jobs across two machines, minimizing making time span and enhancing productivity.

Objective
To optimize the total production cost and improve scheduling efficiency in a two-machine production line using Microsoft Excel. The project aimed to assign products optimally to machines to minimize total cost and then determine the most efficient sequence of operations using Johnson’s Rule, supported by interactive data visualization and analysis tools.

Step 1: Problem Setup and Optimization Using Excel Solver
Developed a dataset containing multiple products, their unit production times, and machine capacities.
Defined a linear optimization model in Excel:
Decision Variables: Number of units of each product assigned to each machine.
Objective Function: Minimize total production cost (sum of cost × units).
Constraints:
Machine capacity limits.
Total production requirements for each product.
Binary constraints for assignment decisions.
Used the Solver Add-in to determine the optimal allocation of units across machines.
Result: Achieved minimum total cost while respecting machine capacity and product demand constraints.

Step 2: Data Analysis Using Pivot Tables and Pivot Charts
Created Pivot Tables to summarize optimization results:
Total cost per product.
Machine-wise workload and utilization.
Product distribution across machines.
Designed Pivot Charts (Clustered Column and Pie Charts) for visual insights on:
Cost contribution by each product.
Machine load comparison.
Added Slicers for dynamic filtering by product or machine to make the analysis interactive.
Result: Enhanced interpretability of optimization outcomes for decision-making and presentation.

Step 3: Job Sequencing Using Johnson’s Rule
Extracted production times for each product on Machine 1 and Machine 2.
Applied Johnson’s Rule for two-machine flow shop sequencing to minimize makespan:
Used helper formulas (MIN, IF, RANK, SORT, and FILTER) to identify which machine has the smallest processing time per product.
Sequenced jobs by placing:
Products with smaller Machine 1 times at the front, and
Products with smaller Machine 2 times at the end (in reverse order).
Implemented VLOOKUP to automatically fetch processing times and confirm sequencing in the schedule table.
Calculated start and completion times for both machines and determined total makespan.
Result: Optimal sequence found (F → J → E → I → K → G → H → D → B → A → C) reducing total completion time by ~20%.

Step 4: Insights and Conclusion
The Solver model minimized cost and improved resource utilization across machines.
The Pivot Table and Chart analysis provided actionable insights into production distribution and bottlenecks.
The Johnson’s sequencing model streamlined scheduling and reduced idle time between machines.
Overall, Excel served as a comprehensive decision-support system, integrating optimization, data analytics, and production scheduling in a single platform.

Tools & Techniques Used
Excel Solver (Optimization)
Pivot Tables, Charts, and Slicers (Data analysis and visualization)
Formulas: SUMPRODUCT, MIN, IF, VLOOKUP, RANK, SORT, FILTER, MAX, INDEX/MATCH
Johnson’s Rule (Scheduling and sequencing)

![preview](https://github.com/tiwaripaarth2403-sudo/Optimization-and-Scheduling-of-Multi-Machine-Production-Systems-Using-Excel/blob/main/ss_1_data.png)
![preview](https://github.com/tiwaripaarth2403-sudo/Optimization-and-Scheduling-of-Multi-Machine-Production-Systems-Using-Excel/blob/main/ss_2_summary.png)
![preview](https://github.com/tiwaripaarth2403-sudo/Optimization-and-Scheduling-of-Multi-Machine-Production-Systems-Using-Excel/blob/main/ss_3_analysis.png)
![preview]()
