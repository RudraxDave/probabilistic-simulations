
# **Probabilistic Simulations and Monte Carlo Experiments**

Welcome to the **Probabilistic Simulations and Monte Carlo Experiments** repository! This repository showcases various experiments that involve simulating probabilistic events and analyzing the results using Python. The simulations focus on biased coin flips and summation of uniform random variables, demonstrating key concepts in probability theory and stochastic processes.

### Monte Carlo Simulation Flow
```mermaid
graph TD;
    A[Start] --> B[Generate Random Points];
    B --> C{Inside Circle?};
    C -->|Yes| D[Increase Counter];
    C -->|No| E[Proceed to Next Point];
    D --> E;
    E --> F[Estimate Pi];
    F --> G[End];


## **Repository Overview**

This repository contains Python scripts that implement the following experiments:

1. **Q1: Biased Coin Flip Simulations**
   - **Q1-A**: Simulate 50 biased coin flips and calculate the number of heads and the longest streak of consecutive heads.
   - **Q1-B**: Perform multiple iterations of the 50 coin flip simulations to analyze the distribution of the number of heads.
   - **Q1-C**: Conduct a longer simulation to study the distribution of streak lengths of consecutive heads.

2. **Q2: Summation of Uniform Random Variables**
   - Simulate the process of summing uniform random variables until the sum exceeds a threshold, and analyze the number of draws required to achieve this.

## **Getting Started**

### **Prerequisites**

Make sure you have Python installed. You'll also need the following Python libraries:

```bash
pip install matplotlib
```

### **Running the Simulations**

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/probabilistic-simulations.git
   cd probabilistic-simulations
   ```

2. Run each Python script to see the simulations in action:

   - **Q1-A**: `python q1_a.py`
   - **Q1-B**: `python q1_b.py`
   - **Q1-C**: `python q1_c.py`
   - **Q2**: `python q2.py`

## **Explanation of Experiments**

### **Q1: Biased Coin Flip Simulations**

1. **Q1-A: Basic Coin Flip Simulation**
   - Simulates 50 trials of a biased coin (heads probability = 0.7).
   - Outputs the total number of heads and the longest streak of heads.

2. **Q1-B: Multiple Simulations with Varying Iterations**
   - Extends the basic simulation to run multiple experiments (e.g., 20, 100, 200, 1000 iterations).
   - Plots histograms to visualize the distribution of the number of heads across different iterations.

3. **Q1-C: Distribution of Head Streak Lengths**
   - Conducts 500 trials to analyze the distribution of the lengths of streaks of consecutive heads.
   - Visualizes the results using a histogram.

### **Q2: Summation of Uniform Random Variables**

- Simulates the process of summing random numbers until their sum exceeds a threshold (e.g., 4).
- Analyzes the number of draws required and plots the distribution of the number of draws needed to achieve the sum threshold.
- The expected number of draws is around 8-9, which aligns with theoretical expectations.

### **Additional Experiments**

1. **Simulating the Law of Large Numbers**
   - Demonstrates the Law of Large Numbers by simulating coin flips and observing how the sample mean converges to the expected value as the number of trials increases.

2. **Estimating Pi Using a Monte Carlo Method**
   - Estimates the value of π by simulating random points within a square and calculating the ratio of points that fall inside a quarter circle.

3. **Random Walk Simulation**
   - Simulates a 1D random walk and visualizes the position over time, demonstrating the concept of stochastic processes.

4. **Buffon's Needle Problem**
   - Estimates the value of π by simulating the dropping of a needle on a floor with parallel lines and counting the number of line crossings.


## **Results and Analysis**

The results of each experiment are visualized using histograms. These visualizations can be found in the `results/` directory, with the following interpretations:

- **Q1-B**: The histograms for different iterations (20, 100, 200, 1000) peak around the expected value of 35, confirming the central limit theorem's implications.
- **Q1-C**: The histogram shows the frequency distribution of streak lengths, providing insights into the behavior of the biased coin over long trials.
- **Q2**: The histogram of the number of draws required to exceed a sum of 4 demonstrates the expected value close to 8-9, aligning with theoretical predictions.

## **Future Work**

- Experiment with different probabilities in Q1 to observe the changes in distribution patterns.
- Increase the number of trials in Q1-C to study the behavior of longer streaks.
- Apply the summation concept in Q2 to real-world datasets or more complex probabilistic models.

## **Contributing**

Contributions are welcome! If you have any ideas for improvements or additional experiments, feel free to open an issue or submit a pull request.

## **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## **Contact**

For any questions or suggestions, feel free to reach out to [Rudy Dave](https://www.linkedin.com/in/rudydave/).
