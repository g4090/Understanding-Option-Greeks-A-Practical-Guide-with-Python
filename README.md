# Understanding-Option-Greeks-A-Practical-Guide-with-Python
calculation of delta , gamma, vega, theta, rho
Comparison of Option Greeks in Python
After calculating and visualizing the Call Option Price and Greeks, here's what the results look like for the given parameters:

Stock Price (S): 120

Strike Price (X): 100

Risk-Free Rate (r): 0.05 (5%)

Time to Expiry (t): 1 year

Volatility (σ): 0.20 (20%)

Calculated Results from Python:
Call Option Price: 26.17

Delta (Δ): 0.90

Gamma (Γ): 0.0075

Vega (ν): 21.60

Theta (Θ): -6.23

Rho (ρ): 81.41

Insights from the Results:
Delta (Δ): The Delta value of 0.90 shows that for every $1 increase in the stock price, the call option’s price will increase by $0.90. This suggests that the option is relatively in-the-money and sensitive to stock price movements.

Gamma (Γ): The Gamma value of 0.0075 tells us that Delta is not changing drastically for small stock price movements. As expected, Gamma is low for options that are not extremely near the strike price.

Vega (ν): A Vega value of 21.60 shows that the option price is quite sensitive to volatility changes. A 1% increase in volatility would raise the option price by $21.60, which is substantial.

Theta (Θ): With a Theta of -6.23, the option will lose approximately $6.23 in value per day due to time decay. As expiration nears, this decay becomes more significant, especially for out-of-the-money options.

Rho (ρ): The Rho value of 81.41 indicates that the option is highly sensitive to interest rate changes. If the risk-free rate were to rise by 1%, the option price would increase by $81.41, reflecting a significant impact for long-term options.

Visualizing the Results: What the Graphs Tell Us
Through visualizing the Greeks in Python, I was able to observe and draw some key behavioral insights. Here’s what the results tell us:

1. Delta vs Stock Price
As the stock price increases, Delta approaches 1. This behavior is expected since Delta represents the rate of change of the option price relative to the underlying asset's price. For in-the-money options, Delta rises, indicating a strong sensitivity to stock price changes.

Key Takeaway:

Delta increases as the option becomes more in-the-money.

Out-of-the-money options have a lower Delta, meaning their price is less sensitive to small changes in the stock price.

2. Gamma vs Stock Price
Gamma shows how much Delta changes as the stock price moves. As the option becomes closer to at-the-money, Gamma peaks. This is because Gamma reflects the second-order effect: how Delta itself changes.

Key Takeaway:

Gamma is highest near the strike price (at-the-money), where small price changes have a larger impact on Delta.

Gamma decreases as the option moves deeper in-the-money or out-of-the-money.

3. Vega vs Stock Price
Vega shows how much the option price changes with volatility. As expected, Vega is highest when the option is at-the-money, where volatility has the most significant impact on potential price movement.

Key Takeaway:

Vega is more pronounced for at-the-money options and decreases as the option moves further in or out of the money.

Volatility increases the potential for larger price movements, and thus, Vega is key for options with longer expiration times or high uncertainty.

4. Theta vs Stock Price
As the option approaches expiration, Theta becomes more negative. Time decay accelerates as expiration nears, particularly for out-of-the-money options. The deeper the option is out-of-the-money, the faster it loses value.

Key Takeaway:

Theta is always negative, showing that the option’s price decreases over time.

Out-of-the-money options lose value faster as expiration approaches due to time decay.

5. Rho vs Stock Price
Rho measures the impact of interest rate changes on option prices. As interest rates increase, the price of call options increases, and the price of put options decreases.

Key Takeaway:

Rho has a more significant impact on long-term options and is less sensitive for shorter-term options.

Interest rates impact the cost of carrying an option, making Rho crucial for managing positions over a longer time horizon.


Conclusion: Insights from the Comparison
Through Python calculations and visualizations, we’ve gained a deeper understanding of how Option Greeks behave in relation to stock price movements, volatility changes, time decay, and interest rates.

Here are the critical takeaways from the visualizations:

Delta is the most sensitive to stock price changes.

Gamma helps assess the stability of Delta as stock prices change.

Vega is essential in times of high volatility, with the highest values near the strike price.

Theta emphasizes the importance of time in options trading, showing that time decay accelerates as expiration nears.

Rho is more important for long-term options, reflecting the impact of interest rates on option prices.

These insights help traders understand the risk/reward dynamics of options and how they can use the Greeks to manage their portfolios effectively.
