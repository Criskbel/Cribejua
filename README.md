# Cribejua

Cribejua tackles the optimization of material transportation for construction projects within the Guadalajara Metropolitan Area, focusing on minimizing transportation costs of fine aggregates from two supply branches to multiple construction sites.

## Mathematical Model

The project formulates a **linear programming** problem where:

- Two supply branches \(C_1\) and \(C_2\) have fixed capacities of 35 and 80 tons respectively.
- Six projects \(P_1\) to \(P_6\) require specific amounts of fine aggregates.
- Transportation costs vary per ton between each supply branch and project.
- Decision variables \(x_1, \dots, x_{12}\) represent tons transported from each branch to each project.
- Constraints ensure branch capacity limits and project demand fulfillment.
- The objective function minimizes the total transportation cost:

$$
\min_{x_1, \dots, x_{12}} \quad 5000x_1 + 2000x_2 + 5000x_3 + 3000x_4 + 6000x_5 + 4000x_6 + 5000x_7 + 1000x_8 + 3000x_9 + 2000x_{10} + 4000x_{11} + 3000x_{12}
$$

## Technologies Used

- **Python**: programming language for modeling and solving the optimization problem.
- **NumPy**: handling arrays and numerical data efficiently.
- **SciPy**: to solve the linear programming problem using simplex method.
- **Jupyter Notebook**: interactive environment for code, equations, and results visualization.

## Results Summary

The optimization yields the optimal tons to transport from each branch to each project, fulfilling all demands at minimum cost. For example:

| Results (Tons) | P1 | P2 | P3 | P4 | P5 | P6 |
|----------------|----|----|----|----|----|----|
| C1 Fine        | 10 |  6 |  0 |  2 |  0 |  3 |
| C2 Fine        |  0 | 11 | 11 | 31 |  6 | 21 |

## Conclusion

The South branch \(C_1\) focuses on certain projects while the North branch \(C_2\) covers the remaining demands more effectively. The model shows how mathematical optimization coupled with Python tools can solve complex real-life logistics challenges in urban construction.

---

Explore the notebook for full code, formulas, and detailed analysis.
