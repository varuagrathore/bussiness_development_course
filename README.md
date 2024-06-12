

## Transportation Problems in Excel 🚚

### Building the Spreadsheet Model 📊

1. **Create a Data Table:**
   - Add rows for each source and columns for each destination.
   - Fill in transportation costs (e.g., shipping cost, distance).
   - Include a column for source output (capacity) and a row for destination demand.

2. **Shipment Table:**
   - Copy the demand table and clear the numbers.
   - Decision variables (cost cells) are now green-colored.

3. **Formulas for Tracking:**
   - Use `SUM` functions for tracking units shipped from each source and to each destination.
   - Calculate total shipping cost using `SUMPRODUCT` with the data and shipment tables.

4. **Objective Function:**
   - Write the formula for the objective function (e.g., total cost) and color-code it gray.

### Using Solver in Excel 🧩

1. **Setting Up Solver:**
   - Solver is used for linear programming problems.
   - Ensure Solver is enabled (see below if not visible).

2. **Decision Variables:**
   - Select the rectangular array of decision variables (transportation costs).

3. **Constraints:**
   - Output constraints: Ensure shipped units from each source <= source capacity.
   - Demand constraints: Ensure shipped units to each destination >= destination demand.

4. **Solver Execution:**
   - Set the objective (minimize or maximize total cost).
   - Run Solver to find optimal shipment quantities.

### Other Excel Tools 🛠️

- **Data Table:**
  - Used for performing What-If analysis.
  - Helps visualize impact of changing variables (e.g., costs, capacities).

- **Goal Seek:**
  - Used to find input value required to achieve a specific goal.
  - Useful for scenarios where a specific outcome is desired.

- **Linear Programming:**
  - Solver can handle linear programming problems directly.
  - Models can include additional constraints or costs beyond transportation costs.

### Enabling Solver in Excel 🔍

If Solver is not visible:

1. **Enable Solver Add-In:**
   - Go to `File > Options > Add-Ins`.
   - Select `Solver Add-In` and click `Go`.
   - Check `Solver Add-In` and click `OK`.
   - Solver should now appear under `Data > Solver`.

2. **Solver Parameters:**
   - Set Solver parameters (objective, decision variables, constraints).
   - Ensure to specify Solver options (e.g., solving method, tolerance).

