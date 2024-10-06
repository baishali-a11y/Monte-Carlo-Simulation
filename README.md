# Monte-Carlo-Simulation
Monte Carlo simulation is a statistical technique used to model and understand the impact of risk and uncertainty in prediction and decision-making processes. It relies on repeated random sampling to generate possible outcomes in a probabilistic model, which helps estimate the likelihood of different results.

Applications:
Finance: Risk management, portfolio valuation, and options pricing.
Supply Chain: Forecasting demand fluctuations, inventory optimization, and project management.
Engineering: Reliability analysis, project cost estimation, and system performance.
Healthcare: Predicting the spread of diseases, medical outcomes, or treatment efficacy

To perform a Monte Carlo simulation in Excel, following these steps:

1. Set Up Your Model
Start by defining the problem and creating a deterministic model. For example, if you're simulating the profit of a business, you might calculate:
Profit = Revenue − Cost
In Excel, enter the basic formula or equation that you want to simulate.

2. Identify the Input Variables
Determine which variables are uncertain and assign a probability distribution to them. For example:
Sales volume
Unit price
Variable cost per unit
For each of these uncertain inputs, you will generate random values using appropriate Excel functions like RAND() or RANDBETWEEN().

3. Set Up Random Variables
Use Excel functions to simulate random values based on your identified distributions. For instance:
Uniform Distribution: Use RANDBETWEEN(min, max) for a simple range of values.
Normal Distribution: Use the formula NORMINV(RAND(), mean, standard_deviation) to generate values from a normal distribution.
Example:
Sales Volume: =RANDBETWEEN(100, 200) (if sales volume is between 100 and 200 units)
Unit Price: =NORMINV(RAND(), 50, 5) (mean price of 50 with a standard deviation of 5)

5. Run the Simulation
In Excel, create a table where each row represents one iteration of the simulation.
Copy your model with random inputs across multiple rows (e.g., 1000 rows) to simulate different scenarios.
Use formulas like =Profit in each row to calculate the result for each iteration.

7. Analyze the Results
Once you've completed the iterations, calculate key metrics, such as:
Mean: =AVERAGE(range) to get the average of your simulated outcomes.
Standard Deviation: =STDEV(range) to see the spread or risk.
Minimum/Maximum: =MIN(range) and =MAX(range) for the extreme outcomes.
Visualize Results: Use histograms or charts (e.g., a frequency distribution or cumulative distribution) to analyze the distribution of outcomes.
Insert a histogram by selecting your data and going to Insert → Charts → Histogram.
