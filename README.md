## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Binomial Model**
   - `Binomial.ipynb`: Contains the implementation of the Binomial option pricing model.

   The Binomial Option Pricing Model is a widely used method for valuing American options, which are options contracts that can be exercised at any point up until, and including, the expiration date. Option values in a binomial tree model are computed through backward induction. Beginning at terminal nodes (node n), final option values are determined based on the stock price at maturity. Moving backward, intermediate nodes calculate option values using expected future payoffs discounted at the risk-free rate, integrating probabilities from the binomial distribution for upward (u) and downward (d) movements. This process culminates at the starting node (node 0), yielding the initial option value and enabling the determination of the option's fair price.

2. **Trinomial Model**
   - `Trinomial.ipynb`: Contains the implementation of the Trinomial option pricing model.

   The Trinomial Option Pricing Model is an extension of the Binomial Model that incorporates an additional price movement option at each time step, creating a three-branch tree instead of two. In a trinomial tree model, option values are calculated using backward induction. Starting at terminal nodes (node n), final option values depend directly on the stock price at maturity. Progressing backward, intermediate nodes compute option values by discounting expected future payoffs at the risk-free rate. This approach integrates probabilities derived from the trinomial distribution, considering possible movement up (u), no movement (m), or movement down (d) of the stock price. The process concludes at the starting node (node 0), yielding the initial option value and enabling the determination of the option's fair price.

3. **Black-Scholes Model**
   - `BlackScholes.ipynb`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes Model is used for pricing European options, which are options contracts that can only be exercised at the expiration date. The model assumes that stock prices follow a geometric Brownian motion and that the risk-free interest rate and volatility are constant over the option's lifetime. The code implementation calculates both the theoretical price of a call and put option with the results being stored in a dataframe for future analysis.

4. **Bjerksund-Stensland Model**
   - `BjerksundStensland.ipynb`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is an extension of the Black-Scholes model that allows for the valuation of American options. It incorporates additional parameters such as the dividend yield, barrier levels, and cost of carrying the asset. The model is particularly useful for valuing options on assets that pay dividends or when there are constraints on when the option can be exercised. It takes into account the optimal exercise strategy for American options, which allows for the determination of whether early exercise is beneficial based on the underlying asset's price dynamics and the option's features. This model provides a more accurate valuation of American options compared to the Black-Scholes model, especially in the presence of dividends and pricing barriers.

5. **Whitepapers**
   - `BlackScholes_Huang2-3.pdf`: Pages 2-3 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Black-Scholes Model. 
   - `Binomial_Huang284-286.pdf`: Pages 284-286 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Binomial Model.
   - `BjerksundStensland_Huang104-106.pdf`: Pages `104-106 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Bjerksund-Stensland Model.
   - `Numerical-Methods-versus-Bjerksund-and-Stensland-Approximations-for-American-Options-Pricing-.pdf`: Comparative analysis of the Binomial, Trinomial, and Bjerksund-Stensland models with logic used to construct the Binomial/Trinomial Models.


